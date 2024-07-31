<script>
    import '../css/components/Header.scss';

    export default{
        data(){
            return{
                linksHeader: ['Home', 'Habilidades', 'Portfolio', 'Contato']
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
            <h1 class="titleName">Eu sou Caio Fortes</h1>
            <p class="text-descricao"> 
                Sou um desenvolvedor comprometido em proporcionar 
                ótimas experiências digitais, unindo a inovação e a 
                criatividade em cada projeto. 
            </p>
            <div id="iconsContainer">
                <a id="icons" href="https://www.linkedin.com/in/caio-fortes/" target="_blank" title="Linkedin">
                    <img src="/icons/linkedin.png" class="imageIcon"/>
                </a>
                <a id="icons" href="https://github.com/Caio-Fortes" target="_blank" title="Github">
                    <img src="/icons/github.png" class="imageIcon"/>
                </a>
            </div>
        </div>
        <div id="painelSeparator"></div>
        <div class="imageProfile">
            <img src="/images/myPhoto.png"/>
        </div>
    </div>
</template>
