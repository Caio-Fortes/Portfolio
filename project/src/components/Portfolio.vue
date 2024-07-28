<script>
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
                ]
            }
        }
    }
</script>

<template>
   <Title TitleOne="Meu" TitleTwo="Portfolio" />
   <div id="widgetContainer">
        <div class="widgets" v-for="skill in skills">
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

<script setup>
    import Title from './TitleContainer.vue';
  
</script>
