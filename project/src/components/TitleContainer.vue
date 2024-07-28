<script>
    export default{
        props:{
            TitleOne:{
                typeof: String,
                required: true,
                default: 'text one'
            },
            TitleTwo:{
                typeof: String,
                required: true,
                default: 'text '
            }
        }
    }
</script>

<template>
   <div id="titleContainer">
        <h1 class="title-primary-text">
            {{ TitleOne }}
            <span class="title-second-text"> {{ TitleTwo }}</span>
        </h1>
   </div>
</template>
