<template>
    <section id="jumbotron">
        <div class="container-lg">
            <div class="title">
            <h1>
                The simplest cloud platform for developers & teams
            </h1>
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Mollitia fuga, tempore ad praesentium maxime sapiente quod voluptas laudantium sed consectetur est eum corrupti voluptatem rerum veniam quo deleniti voluptatibus unde? Lorem, ipsum dolor sit amet consectetur adipisicing elit. Delectus numquam atque maxime necessitatibus quaerat? Velit ipsam pariatur possimus!
            </p>

        </div>
        <div class="singup p-3">
            <h2>
                Deploy your app in seconds.
            </h2>
            <h2 class="blue-ocean">
                Get started now.
            </h2>
            <input class="p-2 rounded" type="text" placeholder="Email">
            <input class="p-2 rounded" type="text" placeholder="Password">
            <a class="create-account-btn p-2 rounded" href="#">Create your account</a>
            <a class="google-btn shadow-sm rounded p-2" href="#">
                <img class="google-icon" src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/53/Google_%22G%22_Logo.svg/2048px-Google_%22G%22_Logo.svg.png" alt="google">
                Sing up with google
            </a>
            <p>By signing up you agree to the <a href="#">Terms of Service</a>.</p>

        </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Jumbotron'
}
</script>

<style lang="scss" scoped>
    @import '../../assets/style/global.scss';
    .blue-ocean {
        color: $blue-ocean;
    }
    #jumbotron {
        background-image: url(../../assets/img/bg-banner-home.jpg);
        padding-top: 50px;
        padding-bottom: 50px;
        background-size: cover;
        background-position: center;
        .container-lg {
            display: flex;
            flex-direction: column;
            .title {
                color: white;
            }
            .singup {
                text-align: center;
                background-color: white;
                border-radius: 10px;
                display: flex;
                flex-direction: column;
                gap: 10px;
                > input {
                    font-weight: 600;
                    border: 2px solid lightgray;
                }
                > a {
                    text-decoration: none;
                    display: inline-block;
                    font-weight: 600;
                }
                .create-account-btn {
                    background-color: $blue-ocean;
                    color: white;
                }
                .google-btn {
                    color: #444;
                    position: relative;
                    .google-icon {
                        height: 1.3rem;
                        position: absolute;
                        top: 50%;
                        transform: translateY(-50%);
                        left: 15px;
                    }
                }
            }
        }
        
    }
    @media screen and (min-width: 768px) {
        #jumbotron > .container-lg {
            flex-direction: row;
            align-items: center;
            gap: 30px;
            .singup {
                width: 50%;            
            }
            .title {
                width: 50%;
            }
        }
    }

</style>