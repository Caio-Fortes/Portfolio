<script>
    import '../css/components/Profile.scss';

    export default{
        data(){
            return{
            }
        }
    }
</script>

<template>
    <div id="containerPrincipal">
        <div id="imageProfile">
            <img src="/images/profileCinza.png"/>
        </div>
        <div id="profileNameDescription">
            <h3>Sobre mim</h3>
            <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer tellus est,
                finibus ut congue sed, faucibus ut dui. Sed congue nisl dolor, id dapibus
                leo elementum posuere. Ut aliquam metus quis laoreet elementum. 
            </p>
            <p> <strong>Email:</strong> caiofortesprofissional@gmail.com</p>
            <p> <strong>Contato:</strong> (35) 99849-8003</p>
            <button id="btnDownloadCv">
                Download Cv
            </button>
        </div>
    </div>
</template>
