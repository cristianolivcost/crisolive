<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Document</title>
</head>

<body>
      <div class="particulas"></div>



    <nav class="navegacao">
        <ul class="Menu">
            <li>
                <a href="#Início" class="menu-link">Início</a>
            </li>

            <li>
                <a href="#Sobre" class="menu-link">Sobre</a>
            </li>

            <li>
                <a href="#Projetos" class="menu-link">Projetos</a>
            </li>

            <li>
                <a href="#Contatos" class="menu-link">Contatos</a>
            </li>

        </ul>
    </nav>

    <main id="Início" class="cabecalho">

        <img src="./img/perfil.jpeg" alt="Foto de Cristian O Costa" class="foto-perfil">
        <h1>Cristian O Costa</h1>
        <p class="cabecalho-sub-titulo">Desenvolvedor Front-end</p>
    </main>

    <section id="Sobre" class="Sobre">
        <h2 class="Sobre-Titulo">Sobre Mim</h2>
        <div class="Sobre-caixa">
            <p class="Sobre-paragrafo">
                meu nome é Cristian e atualmente estou em transição de carreira pra programação full stack, atualmente estou no primeiro mês do aprendizado em busca de um estágio na programação, para mostra minhas habilidades e desenvolvê-las com foco no crescimento minha e da empresa.

            </p>
        </div>
    </section>

    <section id="Projetos" class="">
        <h2 class="Projetos-titulo"> Meus Projetos</h2>
        <div class="Projetos-caixa">

            <div class="Projetos-card">
                <img src="./img/Projeto1.png" alt="Projeto 1" class="Projetos-imagem">
                <div class="caixa-textos-protejtos">
                    <h3 class="info-projetos">Calculadora</h3>
                    <p class="paragrafo-projeto"> como meu primeiro projeto eu escolhi fazer uma Calculadora simplis afins de ter mais conhecimento </p>
                </div>
            </div>

            <div class="Projetos-card">
                <img src="./img/Pojeto2.png" alt="Projeto 1" class="Projetos-imagem">
                <div class="caixa-textos-protejtos">
                    <h3 class="info-projetos">Loja de Carros</h3>
                    <p class="paragrafo-projeto"> Projeto loja de carro desenvolvi com ajuda do dev club focando em mais aprendizado </p>
                </div>
            </div>

        </div>

    </section>



    <section id="Contatos" class="Contatos">
        <h2 class="Contatos-titulo">Entre em Contatos</h2>


        <form class="formulario-contato" id="fomulario" onsubmit="enviarWhats(event)">

            <div class="Grupo-form">
                <input placeholder="Nome" class="campo-form" id="nome" >
            </div>

            <div class="Grupo-form">
                <textarea class="campo-form" placeholder="Digite sua Mensagem" rows="6" id="Mensagem"></textarea>
            </div>

            <button type="submit" class="Botao-form">Enviar WhatsApp</button>
        </form>
    
    </section>

    <script>

        function enviarWhats(event) {
            event.preventDefault();
            
        const nome = document.getElementById('nome')value;
        const mensagem = document.getElementById('mensagem')value;
        const telefone = '5511985696710'

        const texto = `Olá, meu nome é ${nome}, ${mensagem}`;
        const msgformatada = encodeURIComponent(texto);

        const url =`https://wa.me/${telefone}?text=${msgformatada}`

        console.log(url);

        window.open(url, '_blank');


        }


    </script>

</body>

</html>
