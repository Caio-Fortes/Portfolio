<script>
    import '../css/components/Header.scss';

    export default{
        data(){
            return{
                linksHeader: ['Home', 'Portfolio', 'Contato']
            }
        }
    }
</script>

<template>
    <div>
        <ul id="headerContainer"> 
            <li v-for="link in linksHeader" id="linksHeader">
                <a href=""> {{ link }} </a> 
            </li>
        </ul>
    </div>
    <div id="containerPainel">
        <div id="profileNameDescription">
            <h3 class="hello">Olá!</h3>
            <h1>Eu sou Caio Fortes</h1>
            <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. <br />
                Integer tellus est, finibus ut congue sed, faucibus ut dui.
            </p>
            <div id="iconsContainer">
                <a id="icons" href="https://www.linkedin.com/in/caio-fortes/" title="Linkedin">
                    <img src="/icons/linkedin.png" class="imageIcon"/>
                </a>
                <a id="icons" href="https://github.com/Caio-Fortes" title="Github">
                    <img src="/icons/github.png" class="imageIcon"/>
                </a>
            </div>
        </div>
        <div id="painelSeparator"></div>
        <div id="imageProfile">
            <img src="/images/profileTwo.png"/>
        </div>
    </div>
</template>
