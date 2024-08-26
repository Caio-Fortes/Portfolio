<script>
    export default {
        data(){
            return{
                linksHeader: ['Inicio', 'Sobre', 'Portfolio', 'Feedbacks', 'Contato']
            }
        },
        mounted(){
            this.setLayoutOnScroll();
        },
        methods:{
            setLayoutOnScroll(){
                window.addEventListener('scroll', () => {
                    const body = document.body;
                    const profile = document.getElementById('profileContainer');
                    if (window.scrollY > 50) {
                        body.classList.add('scrolled');
                        profile.classList.add('show');
                    } else {
                        body.classList.remove('scrolled');
                        profile.classList.remove('show');
                    }
                });
            }
        }
    }
</script>

<template>
    <div id="headerContainer">
        <ul class="flex"> 
            <li v-for="link in linksHeader" class="linksHeader">
                <a href=""> {{ link }} </a> 
            </li>
        </ul>
        <div class="flex" id="profileContainer"> 
            <li class="linksHeader">
                <li class="linksHeader">
                    <a> Caio Fortes </a>
                </li>
                <div id="profileIcon">
                    <img src="/images/profileIcon.png"/>
                </div>
            </li>
        </div>
    </div>
    
    <div id="flexCenter">
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
    </div>

    <div id="flexCenter">
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
    </div>


</template>