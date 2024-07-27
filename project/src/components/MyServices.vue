<script>
    import '../css/components/MyServices.scss';

    export default{
        data(){
            return{
                skills:[
                    {
                        imageIcon: '/icons/html-skills.png',
                        title:'Aplicativos Web',
                        description: 'teste'
                    },
                    {
                        imageIcon: '/icons/android-skills.png',
                        title:'Aplicativos Mobile',
                        description: 'teste'
                    },
                    {
                        imageIcon: '/icons/design-skills.png',
                        title:'Design UX | UI',
                        description: 'teste'
                    },
                    {
                        imageIcon: '/icons/front-end-skills.png',
                        title:'Front-End',
                        description: 'teste'
                    },
                    {
                        imageIcon: '/icons/back-end-skills.png',
                        title:'Back-End',
                        description: 'teste'
                    },
                    {
                        imageIcon: '/icons/github-skills.png',
                        title:'Versionamento',
                        description: 'teste'
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
                <p>
                    {{ skill.description }}
                </p>
            </div>
        </div>
   </div>
</template>
