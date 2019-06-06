<template>
    <div id="app">
        <div id="nav">
            <ul>
                <li>
                    <router-link to="/">Home</router-link>
                </li>
                <li>
                    <router-link to="/about">About</router-link>
                </li>
                <li>
                    <router-link to="/contact">Contact</router-link>
                </li>
                <li>
                    <router-link to="/menu">Menu</router-link>
                </li>
            </ul>
        </div>
        <router-view/>
    </div>
</template>

<style lang="scss">
    @import url('https://fonts.googleapis.com/css?family=Roboto:400,700&display=swap');

    body {
        padding: 0;
        margin: 0;
    }

    #app {
        font-family: 'Lato', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
        height: 100vh;
        position: relative;

    }

    #nav {


        ul {
            padding: 0;
            margin: 0;

            li {
                display: inline-block;
            }
        }

        a {
            font-weight: bold;
            color: #2c3e50;

            &.router-link-exact-active {
                color: #42b983;
            }
        }
    }
</style>
