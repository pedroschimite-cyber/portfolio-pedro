
<!DOCTYPE html>
<html lang="pt-BR">
    <style>

/* ==========================================
   PORTFÓLIO DE FOTOGRAFIA
   Estilos gerais
========================================== */

/* CORES DO SITE */
:root {
    --azul: #2396aa;
    --azul-escuro: #123b45;
    --azul-claro: #dceff0;
    --fundo: #f7f8f6;
    --branco: #ffffff;
    --texto: #26383c;
    --texto-suave: #68777a;
}

/* CONFIGURAÇÕES GERAIS */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
    scroll-padding-top: 90px;
}

body {
    background-color: var(--fundo);
    color: var(--texto);
    font-family: Arial, Helvetica, sans-serif;
    line-height: 1.6;
}

img {
    display: block;
    width: 100%;
}

a {
    color: inherit;
    text-decoration: none;
}

section {
    scroll-margin-top: 85px;
}


/* ==========================================
   CABEÇALHO E MENU
========================================== */

.cabecalho {
    width: 100%;
    min-height: 78px;
    padding: 18px 7%;
    background-color: var(--branco);

    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 25px;

    position: sticky;
    top: 0;
    z-index: 100;

    box-shadow: 0 2px 15px rgba(18, 59, 69, 0.06);
}

.logo {
    color: var(--azul-escuro);
    font-size: 1.05rem;
    font-weight: 800;
    letter-spacing: 2px;
    white-space: nowrap;
}

.logo span {
    color: var(--azul);
}

.menu {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 28px;
    flex-wrap: wrap;
}

.menu a {
    color: var(--texto);
    font-size: 0.9rem;
    font-weight: 700;
    transition: color 0.3s;
}

.menu a:hover {
    color: var(--azul);
}


/* ==========================================
   TEXTOS E TÍTULOS
========================================== */

.etiqueta {
    color: var(--azul);
    font-size: 0.75rem;
    font-weight: 800;
    letter-spacing: 3px;
    margin-bottom: 16px;
}

.titulo-secao {
    margin-bottom: 42px;
}

.titulo-secao h2,
.sobre h2,
.contato h2 {
    color: var(--azul-escuro);
    font-size: clamp(2.3rem, 5vw, 4rem);
    line-height: 1.1;
    margin-bottom: 18px;
}

.titulo-secao h2 span,
.sobre h2 span {
    color: var(--azul);
}

.descricao-secao {
    color: var(--texto-suave);
    max-width: 10000px;
    font-size: 1.2rem;
}

/* ==========================================
   BOTÕES
========================================== */

.botao {
    display: inline-block;
    padding: 14px 25px;
    border-radius: 4px;
    background-color: var(--azul);
    color: var(--branco);
    font-size: 0.9rem;
    font-weight: 700;

    transition: background-color 0.3s, transform 0.3s;
}

.botao:hover {
    background-color: var(--azul-escuro);
    transform: translateY(-3px);
}

.botao-claro {
    background-color: var(--branco);
    color: var(--azul-escuro);
}

.botao-claro:hover {
    background-color: var(--azul-claro);
    color: var(--azul-escuro);
}


/* ==========================================
   INÍCIO / CAPA
========================================== */

.inicio {
    min-height: 620px;
    padding: 85px 7%;

    display: grid;
    grid-template-columns: 1.1fr 0.9fr;
    align-items: center;
    gap: 55px;

    background-color: var(--azul-claro);
}

.inicio-conteudo h1 {
    color: var(--azul-escuro);
    font-size: clamp(3rem, 6vw, 5.5rem);
    line-height: 1.05;
    margin-bottom: 22px;
}

.inicio-conteudo h1 span {
    color: var(--azul);
}

.texto-inicio {
    color: var(--texto-suave);
    max-width: 480px;
    margin-bottom: 30px;
}

.inicio-imagem {
    height: 430px;
    background-color: #c5dfe1;
    overflow: hidden;
    border-radius: 8px;
}

.inicio-imagem img {
    height: 100%;
    object-fit: cover;
}


/* ==========================================
   SOBRE MIM
========================================== */

.secao {
    padding: 100px 7%;
}

.sobre {
    display: grid;
    grid-template-columns: 0.85fr 1.15fr;
    align-items: center;
    gap: 75px;

    background-color: var(--branco);
}

.sobre-imagem {
    height: 430px;
    background-color: var(--azul-claro);
    overflow: hidden;
    border-radius: 8px;
}

.sobre-imagem img {
    height: 100%;
    object-fit: cover;
}

.sobre-conteudo p:not(.etiqueta) {
    color: var(--texto-suave);
    margin-bottom: 18px;
    max-width: 650px;
}


/* ==========================================
   VISÃO E MISSÃO
========================================== */

.valores {
    background-color: var(--fundo);
}

.valores-grade {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 25px;
}

.valor {
    background-color: var(--branco);
    padding: 38px;
    border-radius: 8px;
    border-top: 5px solid var(--azul);
}

.valor-numero {
    color: var(--azul-claro);
    font-size: 2.5rem;
    font-weight: 800;
}

.valor h3 {
    color: var(--azul-escuro);
    font-size: 1.6rem;
    margin: 12px 0;
}

.valor p {
    color: var(--texto-suave);
}


/* ==========================================
   EXPERIÊNCIAS
========================================== */

.experiencias {
    background-color: var(--azul-claro);
}

.experiencias-grade {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 28px;
}

.experiencia {
    background-color: var(--branco);
    border-radius: 8px;
    overflow: hidden;
}

.experiencia-foto {
    height: 80%;
    width: 100%;
    background-color: #c5dfe1;
}

.experiencia-foto img {
    width: 80%;
    height: 100%;
    object-fit: cover;
}

.experiencia-texto {
    padding: 28px;
}

.categoria {
    color: var(--azul);
    font-size: 0.72rem;
    font-weight: 800;
    letter-spacing: 2px;
}

.experiencia-texto h3 {
    color: var(--azul-escuro);
    font-size: 1.5rem;
    margin: 10px 0;
}

.experiencia-texto p:last-child {
    color: var(--texto-suave);
}


/* ==========================================
   PROJETOS / GALERIA
========================================== */

.projetos {
    background-color: var(--branco);
}

.galeria {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 22px;
}

.foto-galeria {
    aspect-ratio: 3 / 4; /* Formato vertical */
    height: auto;
    overflow: hidden;
    border-radius: 6px;
    background-color: var(--azul-claro);
    position: relative;
}

.foto-galeria img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.4s;
}

.foto-galeria:hover img {
    transform: scale(1.06);
}

.foto-galeria figcaption {
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;

    padding: 15px;
    color: var(--branco);
    background: linear-gradient(transparent, rgba(0, 0, 0, 0.7));

    font-size: 0.9rem;
    font-weight: 700;
}


/* ==========================================
   CONTATO
========================================== */

.contato {
    padding: 90px 7%;
    text-align: center;
    background-color: var(--azul-escuro);
    color: var(--branco);
}

.contato h2 {
    color: var(--branco);
}

.contato > p:not(.etiqueta) {
    margin-bottom: 25px;
    color: #dceff0;
}

.contato .etiqueta {
    color: #80d2df;
}


/* ==========================================
   RODAPÉ
========================================== */

.rodape {
    padding: 25px 7%;
    background-color: #0b2930;
    color: var(--branco);

    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 20px;
    flex-wrap: wrap;
}

.rodape p {
    font-size: 0.85rem;
}

.rodape a {
    color: #80d2df;
    font-size: 0.85rem;
}


/* ==========================================
   RESPONSIVIDADE PARA TABLETS E CELULARES
========================================== */

@media (max-width: 900px) {

    .cabecalho {
        flex-direction: column;
    }

    .menu {
        gap: 15px;
    }

    .inicio {
        grid-template-columns: 1fr;
    }

    .inicio-imagem {
        height: 350px;
    }

    .sobre {
        grid-template-columns: 1fr;
        gap: 35px;
    }

    .sobre-imagem {
        height: 350px;
    }

    .galeria {
        grid-template-columns: repeat(2, 1fr);
    }
}


/* CELULARES */
@media (max-width: 600px) {

    .cabecalho {
        padding: 18px 5%;
    }

    .menu {
        gap: 12px;
    }

    .menu a {
        font-size: 0.78rem;
    }

    .inicio {
        padding: 65px 6%;
        gap: 35px;
    }

    .inicio-conteudo h1 {
        font-size: 2.8rem;
    }

    .inicio-imagem {
        height: 280px;
    }

    .secao {
        padding: 65px 6%;
    }

    .sobre-imagem {
        height: 300px;
    }

    .valores-grade,
    .experiencias-grade,
    .galeria {
        grid-template-columns: 1fr;
    }

    .valor {
        padding: 28px;
    }

  .foto-galeria {
    aspect-ratio: 3 / 4;
    height: auto;
}
    .contato {
        padding: 65px 6%;
    }

    .rodape {
        flex-direction: column;
        text-align: center;
    }
}


    </style>

<head>
    <!-- Configurações da página -->
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Portfólio de fotografia de Pedro H. Schimite.">
    <title>Pedro H. Schimite | Portfólio</title>

    <!-- Conexão com o arquivo CSS -->
    <link rel="stylesheet" href="style.css">
</head>

<body>

    <!-- CABEÇALHO E MENU -->
    <header class="cabecalho">
        <a class="logo" href="#inicio">PEDRO H. <span>SCHIMITE</span></a>

        <nav class="menu">
            <a href="#inicio">Início</a>
            <a href="#sobre">Sobre mim</a>
            <a href="#vm">V/M</a>
            <a href="#experiencias">Experiências</a>
            <a href="#projetos">Projetos</a>
        </nav>
    </header>

    <main>

        <!-- 1. INÍCIO -->
        <section id="inicio" class="inicio">

            <div class="inicio-conteudo">
                <p class="etiqueta">PORTFÓLIO DE FOTOGRAFIA</p>

                <h1>
                    Transformando<br>
                    <span>momentos em imagens.</span>
                </h1>

                <p class="texto-inicio">
                    Fotografia, criatividade e histórias registradas através das lentes.
                </p>

                <a class="botao" href="#projetos">
                    Conheça meus projetos
                </a>
            </div>

            <!-- Foto principal -->
            <div class="inicio-imagem">
                <img src="img/Blue Minimalist Creative Portfolio Presentation.png" alt="Fotografia de destaque">
            </div>

        </section>


        <!-- 2. SOBRE MIM -->
        <section id="sobre" class="secao sobre">

            <div class="sobre-imagem">
                <img src="img/Image_A7DD7BF2-9E3C-4F40-A663-6D6425E46EBB.jpeg" alt="Foto de apresentação">
            </div>

            <div class="sobre-conteudo">
                <p class="etiqueta">QUEM ESTÁ POR TRÁS DA CÂMERA</p>

                <h2>Sobre <span>mim</span></h2>

                <p>
                    Olá! Meu nome é Pedro H. Schimite, sou estudante do curso
                    de Multimídias do SENAI e fotógrafo profissional.
                </p>

                <p>
                    Neste portfólio, apresento um pouco do meu trabalho,
                    da minha criatividade e do meu olhar por trás das lentes.
                    Meu objetivo é registrar momentos, transmitir emoções
                    e contar histórias por meio da fotografia.
                </p>
            </div>

        </section>


        <!-- 3. VISÃO E MISSÃO -->
        <section id="vm" class="secao valores">

            <div class="titulo-secao">
                <p class="etiqueta">MEU PROPÓSITO</p>
                <h2>Visão <span>&</span> Missão</h2>
            </div>

            <div class="valores-grade">

                <article class="valor">
                    <span class="valor-numero">01</span>

                    <h3>Visão</h3>

                    <p>
                        Ser reconhecido pela criatividade, qualidade e
                        autenticidade dos meus trabalhos, evoluindo
                        constantemente na fotografia e criando imagens
                        que transmitam emoções e contem histórias.
                    </p>
                </article>

                <article class="valor">
                    <span class="valor-numero">02</span>

                    <h3>Missão</h3>

                    <p>
                        Registrar momentos e expressar emoções por meio
                        da fotografia, utilizando técnica, criatividade
                        e sensibilidade para valorizar cada detalhe.
                    </p>
                </article>

            </div>
        </section>


        <!-- 4. EXPERIÊNCIAS -->
        <section id="experiencias" class="secao experiencias">

            <div class="titulo-secao">
                <p class="etiqueta">MINHA TRAJETÓRIA</p>

                <h2>Experiências</h2>

                <p class="descricao-secao">
                    Alguns eventos e trabalhos que fizeram parte da minha caminhada.
                </p>
            </div>

            <div class="experiencias-grade">

                <!-- EXPERIÊNCIA 1 -->
                <article class="experiencia">

                    <div class="experiencia-foto">
                        <img src="img/55.JPG"
                             alt="Fotografia da prova de três tambores">
                    </div>

                    <div class="experiencia-texto">
                        <p class="categoria">FOTOGRAFIA ESPORTIVA</p>

                        <h3>Prova de três tambores</h3>

                        <p>
                            Cobertura fotográfica de uma prova de três tambores,
                            registrando a velocidade, a técnica e a emoção da competição.
                            Também produzi um vídeo reunindo fotos e gravações do evento.
                        </p>
                    </div>

                </article>


                <!-- EXPERIÊNCIA 2 -->
                <article class="experiencia">

                    <div class="experiencia-foto">
                        <img src="img/ed (8).JPG"
                             alt="Fotografia da corrida beneficente">
                    </div>

                    <div class="experiencia-texto">
                        <p class="categoria">COBERTURA DE EVENTO</p>

                        <h3>Corrida beneficente</h3>

                        <p>
                            Cobertura fotográfica de uma corrida beneficente,
                            registrando os participantes, a energia e os momentos
                            marcantes do evento. Também realizei a produção de um vídeo.
                        </p>
                    </div>

                </article>

            </div>
        </section>


        <!-- 5. PROJETOS E GALERIA -->
        <section id="projetos" class="secao projetos">

            <div class="titulo-secao">
                <p class="etiqueta">MEUS TRABALHOS</p>

                <h2>Projetos <span>fotográficos</span></h2>

                <p class="descricao-secao">
                    Uma seleção de imagens e momentos registrados por mim.
                </p>
            </div>

            <div class="galeria">

                <figure class="foto-galeria">
                    <img src="img/1.JPG" alt="Projeto fotográfico 1">
                    <figcaption>Projeto fotográfico</figcaption>
                </figure>

                <figure class="foto-galeria">
                    <img src="img/3.JPG" alt="Projeto fotográfico 2">
                    <figcaption>Projeto fotográfico</figcaption>
                </figure>

                <figure class="foto-galeria">
                    <img src="img/55.JPG" alt="Projeto fotográfico 3">
                    <figcaption>Projeto fotográfico</figcaption>
                </figure>

                <figure class="foto-galeria">
                    <img src="img/2.JPG" alt="Projeto fotográfico 4">
                    <figcaption>Projeto fotográfico</figcaption>
                </figure>

                <figure class="foto-galeria">
                    <img src="img/12.JPG" alt="Projeto fotográfico 5">
                    <figcaption>Projeto fotográfico</figcaption>
                </figure>

                <figure class="foto-galeria">
                    <img src="img/31.JPG" alt="Projeto fotográfico 6">
                    <figcaption>Projeto fotográfico</figcaption>
                </figure>

            </div>
        </section>


        <!-- 6. CONTATO -->
        <section id="contato" class="contato">

            <p class="etiqueta">VAMOS CONVERSAR?</p>

            <h2>Entre em contato</h2>

            <p>
                (17) 98807-6580 ou @pedroshschimite_fotografias
            </p>



        </section>

    </main>


    <!-- RODAPÉ -->
    <footer class="rodape">

        <p>© 2026 Pedro H. Schimite — Portfólio de Fotografia</p>

        <a href="#inicio">Voltar ao início ↑</a>

    </footer>

</body>
</html>
