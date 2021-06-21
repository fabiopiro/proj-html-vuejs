<template>
    <nav class="nav d-flex d-flex justify-content-between align-items-center">
        <div class="nav-left d-flex align-items-center">
            <div class="logo">
                <img src="../assets/img/logo.png" alt="">
            </div>
            <ul class="list d-flex">
                <li
                v-for="(links, index) in navLinks"
                :key="index"
                >
                <a href="">{{links.name}}</a>
                </li>
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
    props: {
        navLinks: {
            type: Array,
            required: true,
        },
    }
}
</script>

<style lang="scss" scoped>
// variables import
@import '../style/variables.scss';

.nav {
    height: 150px;
    background-color: $color-two;

    .nav-left {
        
        .logo {
            height: 55px;
            width: 55px;
            img {
            height: 100%;
            width: 100%; 
            }
        }

        .list {
            list-style: none;
            margin: 0;
            padding: 0;
            li {
                margin-left: 10px;
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
                // &:nth-child(3)::after {
                //     font-family: "Font Awesome 5 Free";
                //     font-weight: 900; content: "\f078";
                //     padding-left: 10px;
                //     color: $color-one;
                // }
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