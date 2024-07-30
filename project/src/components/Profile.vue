<script>
    import '../css/components/Profile.scss';

    export default{
        methods:{
            downloadCv() {
                const pdfPath = '/Caio Fortes - CV.pdf';
                const link = document.createElement('a');
                link.href = pdfPath;
                link.download = 'CaioFortesCv.pdf';
                document.body.appendChild(link);
                link.click();
                document.body.removeChild(link);
            }
        }
    }
</script>

<template>
    <div id="containerPrincipal">
        <div id="imageProfile">
            <img src="/images/myPhotoCinza.png"/>
        </div>
        <div id="profileNameDescription">
            <h3>Sobre mim</h3>
            <p>
                Meu nome é Caio Fortes dos Santos e possuo 2 anos de experiência no mercado de 
                trabalho como desenvolvedor web, além de 8 anos de experiência acadêmica adquirida 
                em cursos técnicos e profissionalizantes. Sou graduado em Análise e Desenvolvimento de 
                Sistemas e venho aprimorando minhas habilidades em tecnologia desde 2016, 
                quando iniciei minha formação em cursos técnicos na área.
            </p>
            <p> <strong>Email:</strong> caiofortesprofissional@gmail.com</p>
            <p> <strong>Contato:</strong> (35) 99849-8003</p>
            <button id="btnDownloadCv" @click="downloadCv">
                Download Cv
            </button>
        </div>
    </div>
</template>
