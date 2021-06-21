<template>
    <nav class="nav d-flex d-flex justify-content-between align-items-center">
        <div class="nav-left d-flex">
            <div class="logo">
                <img src="../assets/img/logo.png" alt="">
            </div>
            <ul class="list d-flex align-items-center">
                <li
                v-for="(links, index) in navLinks"
                :key="index"
                @click="setActive(index)"
                :class="(isActive == index) ? 'active' : ''"
                >
                <a :href="links.link">{{links.name}}</a>
                </li>
                <!-- <li class="active"><a href="">ciao</a></li>
                <li><a href="">bello</a></li>
                <li><a href="">ciao</a></li>
                <li><a href="">bello</a></li>
                <li><a href="">ciao</a></li>
                <li><a href="">bello</a></li> -->
                
            </ul>
        </div>
        <div class="nav-right d-flex align-items-center">
            <span class="phone-number">1.800.123.4567</span>
            <span class="button-one">Get a free consultation</span>
        </div>
    </nav>
</template>

<script>
export default {
    name: 'Nav',
    data: function () {
      return {
        navLinks: [
          {
            name: 'home',
            link: '#'
          },
          {
            name: 'about',
            link: '#'
          },
          {
            name: 'services',
            link: '#'
          },
          {
            name: 'journal',
            link: '#'
          },
          {
            name: 'contacts',
            link: '#'
          },
        ],
        isActive: '0',
      }
    },
    methods: {
        setActive(i) {
            this.isActive = i;
        }
    }
}
</script>

<style lang="scss" scoped>
// variables import
@import '../style/variables.scss';

.nav {
    height: 150px;
    background-color: red;
    padding: 0 5%;

    .nav-left {
        
        .logo {
            height: 55px;
            width: 55px;
            margin-right: 20px;
            img {
            height: 100%;
            width: 100%; 
            }
        }

        .list {
            list-style: none;
            margin: 0px;
            li {
                display: flex;
                align-items: center;
                height: 100%;
                margin-left: 30px;
                &.active {
                    border-bottom: 2px solid $color-one;
                }
                a {
                    text-decoration: none;
                    color: $color-one;
                    font-weight: bold;
                    text-transform: capitalize;
                    cursor: pointer;
                }
                &:nth-child(3)::after {
                    font-family: "Font Awesome 5 Free";
                    font-weight: 900; content: "\f078";
                    padding-left: 10px;
                    color: $color-one;
                }
            }
        }

    }

    .nav-right {
        .phone-number {
            font-weight: bold;
            color: $color-one;
            margin-right: 40px;
            &::before {
                font-family: "Font Awesome 5 Free";
                font-weight: 900; content: "\f879";
                padding-right: 10px;
            }
            
        }
    }
}

</style>