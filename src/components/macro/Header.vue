<template>
  <header>
      <div class="container-lg">
          <nav>
                <img src="../../assets/img/logo.png" alt="Logo">
                <ul>
                    <li>
                        <a href="#">Products</a>
                    </li>
                    <li>
                        <a href="#">Customers</a>
                    </li>
                    <li>
                        <a href="#">Community</a>
                    </li>
                    <li>
                        <a href="#">Pricing</a>
                    </li>
                </ul>
                <ul>
                    <li>
                        <a href="#">Docs</a>
                    </li>
                    <li>
                        <a href="#">Support</a>
                    </li>
                    <li>
                        <a href="#">Login</a>
                    </li>
                    <li>
                        <a href="#">Sign Up</a>
                    </li>
                </ul>
                <button class="p-2" id="hamburger">
                    <i class="fas fa-bars"></i>
                </button>
          </nav>

      </div>
  </header>
</template>

<script>
export default {
    name: 'Header',
}
</script>

<style lang="scss" scoped>
    @import '../../assets/style/global.scss';

    header{
        padding: 15px 0;
    }
    nav { 
        > img {
           height: 30px; 
        }
        display: flex;
        justify-content: space-between;
        align-items: center;
        ul {
            margin: 0;
            list-style: none;
            display: none;
            align-items: center;
            li {
                display: flex;
                align-items: center;
                margin-left: 15px;
                &:first-child {
                    margin-left: 0;
                }
                a {
                    display: inline-block;
                    text-decoration: none;
                    color: black;
                }
            }
        }
        #hamburger {
            background: none;
            border: none;
            color: $blue-ocean;
            display: flex;
            align-items: center;
            justify-content: center;
            .fa-bars {
                font-size: 1.3rem;
            }
        }
    }
    
    @media screen and (min-width: 992px) {
        nav {
            ul {
                display: flex;
            }
        }
        #hamburger {
            display: none;
        }
    }

</style>