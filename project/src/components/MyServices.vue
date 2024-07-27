<script>
    import '../css/components/MyServices.scss';

    export default{
        data(){
            return{
                skills:[
                    {
                        imageIcon: '/icons/html-skills.png',
                        title:'Aplicativos Web',
                        description: `
                            Desenvolvimento de aplicações web eficientes e 
                            responsivas.
                        `
                    },
                    {
                        imageIcon: '/icons/android-skills.png',
                        title:'Aplicativos Mobile',
                        description: `
                            Desenvolvimento de aplicativos móveis híbridos 
                            com foco em ótimas experiências digitais.
                        ` 
                    },
                    {
                        imageIcon: '/icons/design-skills.png',
                        title:'Design UX | UI',
                        description: `
                            Habilidades em Design de interfaces e experiência do usuário.
                        `
                    },
                    {
                        imageIcon: '/icons/front-end-skills.png',
                        title:'Front-End', 
                        description: `
                            Construção de interfaces interativas
                            utilizando frameworks modernos.
                        `
                    },
                    {
                        imageIcon: '/icons/back-end-skills.png',
                        title:'Back-End',
                        description: `
                            Desenvolvimento de servidores e APIs, assegurando funcionalidade e 
                            segurança.
                        `
                    },
                    {
                        imageIcon: '/icons/github-skills.png',
                        title:'Versionamento',
                        description: ' Habilidades em controle de versão para garantir a integridade do código.'
                    },
                ]
            }
        }
    }
</script>

<template>
   <div id="titleContainer">
        <h1 class="title">
            <span>Minhas</span>
            <span class="title-habilidades"> Habilidades</span>
        </h1>
        <div id="rowSeparator"></div>
   </div>
   <div id="SkillsContainer">
        <div class="widgets" v-for="skill in skills">
            <div class="circle-icon">
                <img :src="skill.imageIcon" />
            </div>
            <div class="circle-title">
                {{ skill.title }}
            </div>
            <div class="circle-description">
                <p class="text-description">
                    {{ skill.description }}
                </p>
            </div>
        </div>
   </div>
</template>
