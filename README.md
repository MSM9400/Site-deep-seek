<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>EcoConsciente 2025 | Preservação Ambiental e Sustentabilidade</title>
    <style>
        :root {
            --verde-principal: #2E7D32;
            --verde-claro: #81C784;
            --amarelo: #FFD600;
            --verde-escuro: #1B5E20;
            --fundo-claro: #E8F5E9;
            --texto: #333333;
            --branco: #FFFFFF;
            --vermelho-emergencia: #D32F2F;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Roboto', Arial, sans-serif;
        }

        body {
            background-color: var(--fundo-claro);
            color: var(--texto);
            line-height: 1.6;
        }

        /* Header */
        header {
            background-color: var(--verde-principal);
            color: var(--branco);
            padding: 15px 30px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            box-shadow: 0 3px 10px rgba(0,0,0,0.2);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .logo img {
            height: 50px;
        }

        .logo-texto h1 {
            font-size: 1.8rem;
            font-weight: 700;
        }

        .logo-texto p {
            font-size: 0.9rem;
            opacity: 0.9;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 5px;
        }

        nav a {
            color: var(--branco);
            text-decoration: none;
            padding: 10px 15px;
            border-radius: 5px;
            transition: all 0.3s;
            font-weight: 500;
        }

        nav a:hover {
            background-color: var(--verde-escuro);
            transform: translateY(-2px);
        }

        .botoes-header {
            display: flex;
            gap: 10px;
        }

        .botao {
            background-color: var(--amarelo);
            color: var(--texto);
            border: none;
            padding: 10px 15px;
            border-radius: 5px;
            cursor: pointer;
            font-weight: bold;
            transition: all 0.3s;
            display: flex;
            align-items: center;
            gap: 5px;
        }

        .botao:hover {
            background-color: #FFC107;
            transform: translateY(-2px);
            box-shadow: 0 2px 5px rgba(0,0,0,0.2);
        }

        .botao-emergencia {
            background-color: var(--vermelho-emergencia);
            color: var(--branco);
        }

        .botao-emergencia:hover {
            background-color: #B71C1C;
        }

        /* Conteúdo Principal */
        main {
            padding: 30px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .destaque {
            background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), url('https://images.unsplash.com/photo-1618221195710-dd6b41faaea6?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1400&q=80');
            background-size: cover;
            background-position: center;
            color: white;
            padding: 60px 30px;
            border-radius: 10px;
            margin-bottom: 30px;
            text-align: center;
        }

        .destaque h2 {
            font-size: 2.5rem;
            margin-bottom: 15px;
        }

        .destaque p {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto 25px;
        }

        .destaque a {
            display: inline-block;
            background-color: var(--branco);
            color: var(--verde-principal);
            text-decoration: none;
            padding: 12px 25px;
            border-radius: 5px;
            font-weight: bold;
            transition: all 0.3s;
        }

        .destaque a:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }

        .cards {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
            margin: 30px 0;
        }

        .card {
            background-color: var(--branco);
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }

        .card:hover {
            transform: translateY(-10px);
        }

        .card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .card-conteudo {
            padding: 20px;
        }

        .card h3 {
            color: var(--verde-principal);
            margin-bottom: 10px;
            font-size: 1.3rem;
        }

        .card p {
            margin-bottom: 15px;
            color: #555;
        }

        .card a {
            color: var(--verde-principal);
            font-weight: bold;
            text-decoration: none;
            display: inline-flex;
            align-items: center;
            gap: 5px;
        }

        .card a:hover {
            text-decoration: underline;
        }

        /* Seção de Denúncias */
        .denuncia {
            background-color: var(--branco);
            padding: 30px;
            border-radius: 10px;
            margin: 40px 0;
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
        }

        .denuncia h2 {
            color: var(--vermelho-emergencia);
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .contatos-emergencia {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .contato-item {
            background-color: var(--fundo-claro);
            padding: 15px;
            border-radius: 8px;
            display: flex;
            align-items: center;
            gap: 15px;
        }

        .contato-item img {
            width: 40px;
            height: 40px;
        }

        .contato-info h3 {
            margin-bottom: 5px;
            color: var(--verde-escuro);
        }

        /* Popups */
        .popup {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0,0,0,0.7);
            z-index: 2000;
            justify-content: center;
            align-items: center;
        }

        .popup-conteudo {
            background-color: var(--branco);
            width: 90%;
            max-width: 600px;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 20px rgba(0,0,0,0.3);
            animation: popupFade 0.3s;
        }

        @keyframes popupFade {
            from { opacity: 0; transform: translateY(-20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .popup-cabecalho {
            background-color: var(--verde-principal);
            color: var(--branco);
            padding: 15px 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .popup-cabecalho h2 {
            font-size: 1.5rem;
        }

        .fechar-popup {
            background: none;
            border: none;
            color: var(--branco);
            font-size: 1.5rem;
            cursor: pointer;
            padding: 5px;
        }

        .popup-corpo {
            padding: 20px;
            max-height: 70vh;
            overflow-y: auto;
        }

        /* Chatbot */
        .chat-mensagens {
            height: 300px;
            overflow-y: auto;
            border: 1px solid #ddd;
            border-radius: 8px;
            padding: 15px;
            margin-bottom: 15px;
            background-color: #f9f9f9;
        }

        .mensagem {
            margin-bottom: 15px;
            padding: 10px 15px;
            border-radius: 18px;
            max-width: 80%;
            word-wrap: break-word;
        }

        .mensagem-usuario {
            background-color: var(--verde-claro);
            color: var(--texto);
            margin-left: auto;
            border-bottom-right-radius: 5px;
        }

        .mensagem-bot {
            background-color: var(--verde-principal);
            color: var(--branco);
            margin-right: auto;
            border-bottom-left-radius: 5px;
        }

        .chat-input {
            display: flex;
            gap: 10px;
        }

        .chat-input input {
            flex: 1;
            padding: 12px 15px;
            border: 1px solid #ddd;
            border-radius: 25px;
            outline: none;
            font-size: 1rem;
        }

        .chat-input button {
            border-radius: 50%;
            width: 50px;
            height: 50px;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .comandos-chat {
            margin-top: 20px;
        }

        .comandos-chat h3 {
            margin-bottom: 10px;
            color: var(--verde-escuro);
        }

        .lista-comandos {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 10px;
        }

        .comando-item {
            background-color: var(--fundo-claro);
            padding: 10px;
            border-radius: 8px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .comando-item button {
            padding: 5px 10px;
            font-size: 0.8rem;
        }

        /* Quiz */
        .quiz-pergunta {
            font-size: 1.2rem;
            margin-bottom: 20px;
            font-weight: 500;
        }

        .quiz-opcoes {
            display: grid;
            grid-template-columns: 1fr;
            gap: 10px;
            margin-bottom: 20px;
        }

        .quiz-opcao {
            padding: 12px 15px;
            background-color: var(--fundo-claro);
            border-radius: 8px;
            cursor: pointer;
            transition: all 0.3s;
            border: 2px solid transparent;
        }

        .quiz-opcao:hover {
            background-color: var(--verde-claro);
            border-color: var(--verde-principal);
        }

        .quiz-opcao.selecionada {
            background-color: var(--verde-principal);
            color: var(--branco);
            border-color: var(--verde-escuro);
        }

        .quiz-opcao.correta {
            background-color: #4CAF50;
            color: white;
            border-color: #2E7D32;
        }

        .quiz-opcao.incorreta {
            background-color: #F44336;
            color: white;
            border-color: #D32F2F;
        }

        .quiz-controles {
            display: flex;
            justify-content: space-between;
        }

        .quiz-resultado {
            text-align: center;
            font-size: 1.2rem;
            margin: 20px 0;
            font-weight: bold;
            color: var(--verde-escuro);
        }

        /* Rodapé */
        footer {
            background-color: var(--verde-escuro);
            color: var(--branco);
            padding: 30px;
            text-align: center;
        }

        .rodape-conteudo {
            max-width: 1200px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            text-align: left;
        }

        .rodape-coluna h3 {
            margin-bottom: 15px;
            font-size: 1.2rem;
        }

        .rodape-coluna ul {
            list-style: none;
        }

        .rodape-coluna li {
            margin-bottom: 8px;
        }

        .rodape-coluna a {
            color: var(--branco);
            text-decoration: none;
            opacity: 0.8;
            transition: opacity 0.3s;
        }

        .rodape-coluna a:hover {
            opacity: 1;
            text-decoration: underline;
        }

        .redes-sociais {
            display: flex;
            gap: 15px;
            margin-top: 15px;
        }

        .redes-sociais a img {
            width: 40px;
            height: 40px;
            opacity: 0.8;
            transition: all 0.3s;
        }

        .redes-sociais a:hover img {
            opacity: 1;
            transform: translateY(-3px);
        }

        .copyright {
            margin-top: 30px;
            padding-top: 20px;
            border-top: 1px solid rgba(255,255,255,0.1);
            opacity: 0.8;
        }

        /* Responsivo */
        @media (max-width: 768px) {
            header {
                flex-direction: column;
                gap: 15px;
                text-align: center;
            }
            
            nav ul {
                flex-wrap: wrap;
                justify-content: center;
            }
            
            .botoes-header {
                width: 100%;
                justify-content: center;
            }
            
            .lista-comandos {
                grid-template-columns: 1fr;
            }
            
            .destaque h2 {
                font-size: 2rem;
            }
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
</head>
<body>
    <!-- Cabeçalho -->
    <header>
        <div class="logo">
            <img src="https://cdn-icons-png.flaticon.com/512/3369/3369973.png" alt="Logo EcoConsciente">
            <div class="logo-texto">
                <h1>EcoConsciente</h1>
                <p>Preservando hoje para viver amanhã</p>
            </div>
        </div>
        
        <nav>
            <ul>
                <li><a href="#inicio"><i class="fas fa-home"></i> Início</a></li>
                <li><a href="#reciclagem"><i class="fas fa-recycle"></i> Reciclagem</a></li>
                <li><a href="#sustentabilidade"><i class="fas fa-leaf"></i> Sustentabilidade</a></li>
                <li><a href="#denuncias"><i class="fas fa-bullhorn"></i> Denúncias</a></li>
                <li><a href="#noticias"><i class="far fa-newspaper"></i> Notícias 2025</a></li>
                <li><a href="#contato"><i class="fas fa-envelope"></i> Contato</a></li>
            </ul>
        </nav>
        
        <div class="botoes-header">
            <button class="botao" id="botao-chat">
                <i class="fas fa-robot"></i> EcoChat
            </button>
            <button class="botao" id="botao-quiz">
                <i class="fas fa-gamepad"></i> EcoQuiz
            </button>
            <button class="botao botao-emergencia" id="botao-denuncia">
                <i class="fas fa-exclamation-triangle"></i> Denúncia
            </button>
        </div>
    </header>

    <!-- Conteúdo Principal -->
    <main>
        <!-- Seção Destaque -->
        <section id="inicio" class="destaque">
            <h2>Juntos por um planeta mais verde em 2025!</h2>
            <p>Descubra como pequenas ações do seu dia a dia podem fazer uma grande diferença para o meio ambiente e para as futuras gerações.</p>
            <a href="https://www.ibama.gov.br" target="_blank" rel="noopener noreferrer">
                <i class="fas fa-seedling"></i> Comece Agora
            </a>
        </section>

        <!-- Cartões de Informação -->
        <section id="reciclagem">
            <h2 style="color: var(--verde-principal); margin-bottom: 20px; display: flex; align-items: center; gap: 10px;">
                <i class="fas fa-recycle"></i> Reciclagem em 2025
            </h2>
            <div class="cards">
                <div class="card">
                    <img src="https://images.unsplash.com/photo-1584977046800-b1eef0306d49?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" alt="Coleta seletiva">
                    <div class="card-conteudo">
                        <h3>Novas Regras de Coleta Seletiva</h3>
                        <p>Em 2025, novas normas federais tornaram obrigatória a separação de resíduos em 5 categorias. Saiba como se adaptar.</p>
                        <a href="https://www.gov.br/mma/pt-br/assuntos/residuos/reciclagem" target="_blank" rel="noopener noreferrer">
                            Ver mais <i class="fas fa-arrow-right"></i>
                        </a>
                    </div>
                </div>
                
                <div class="card">
                    <img src="https://images.unsplash.com/photo-1606787366850-de6330128bfc?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" alt="Pontos de coleta">
                    <div class="card-conteudo">
                        <h3>Pontos de Coleta em Sua Cidade</h3>
                        <p>Encontre os ecopontos mais próximos e saiba quais materiais são aceitos em cada um deles.</p>
                        <a href="https://www.reciclasampa.com.br/ecopontos" target="_blank" rel="noopener noreferrer">
                            Buscar agora <i class="fas fa-map-marker-alt"></i>
                        </a>
                    </div>
                </div>
                
                <div class="card">
                    <img src="https://images.unsplash.com/photo-1550246140-5119ae4790b8?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" alt="Inovação em reciclagem">
                    <div class="card-conteudo">
                        <h3>Tecnologias de Reciclagem</h3>
                        <p>Conheça as inovações tecnológicas que estão revolucionando a reciclagem de plásticos e eletrônicos em 2025.</p>
                        <a href="https://www.brasil.gov.br/noticias/meio-ambiente/2023/05/tecnologias-inovadoras-impulsionam-reciclagem-no-brasil" target="_blank" rel="noopener noreferrer">
                            Descobrir <i class="fas fa-lightbulb"></i>
                        </a>
                    </div>
                </div>
            </div>
        </section>

        <!-- Seção Sustentabilidade -->
        <section id="sustentabilidade" style="margin-top: 50px;">
            <h2 style="color: var(--verde-principal); margin-bottom: 20px; display: flex; align-items: center; gap: 10px;">
                <i class="fas fa-leaf"></i> Vida Sustentável
            </h2>
            <div class="cards">
                <div class="card">
                    <img src="https://images.unsplash.com/photo-1486401899868-0e435ed85128?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" alt="Energia renovável">
                    <div class="card-conteudo">
                        <h3>Energia Limpa em Casa</h3>
                        <p>Guia completo para reduzir sua conta de luz e sua pegada de carbono com energia solar e eólica residencial.</p>
                        <a href="https://www.epe.gov.br/pt/energia-limpa" target="_blank" rel="noopener noreferrer">
                            Economizar <i class="fas fa-solar-panel"></i>
                        </a>
                    </div>
                </div>
                
                <div class="card">
                    <img src="https://images.unsplash.com/photo-1517649763962-0c623066013b?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" alt="Consumo consciente">
                    <div class="card-conteudo">
                        <h3>Consumo Consciente</h3>
                        <p>Como fazer escolhas de compra que beneficiam o meio ambiente e ainda economizam dinheiro.</p>
                        <a href="https://www.akatu.org.br/temas/consumo-consciente/" target="_blank" rel="noopener noreferrer">
                            Aprender <i class="fas fa-shopping-basket"></i>
                        </a>
                    </div>
                </div>
                
                <div class="card">
                    <img src="https://images.unsplash.com/photo-1534957753291-64d667ce2927?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" alt="Mobilidade urbana">
                    <div class="card-conteudo">
                        <h3>Mobilidade Urbana Verde</h3>
                        <p>As melhores opções de transporte sustentável nas grandes cidades brasileiras em 2025.</p>
                        <a href="https://www.gov.br/mdr/pt-br/assuntos/transporte-ativo-e-mobilidade-urbana" target="_blank" rel="noopener noreferrer">
                            Explorar <i class="fas fa-bicycle"></i>
                        </a>
                    </div>
                </div>
            </div>
        </section>

        <!-- Seção de Denúncias Ambientais -->
        <section id="denuncias" class="denuncia">
            <h2><i class="fas fa-exclamation-triangle"></i> Denúncias Ambientais</h2>
            <p>Você presenciou algum crime ambiental? Poluição, desmatamento ilegal, maus-tratos a animais? Denuncie! Sua ação pode ajudar a preservar nosso ecossistema.</p>
            
            <div class="contatos-emergencia">
                <div class="contato-item">
                    <img src="https://cdn-icons-png.flaticon.com/512/2785/2785696.png" alt="IBAMA">
                    <div class="contato-info">
                        <h3>Linha Verde do IBAMA</h3>
                        <p><i class="fas fa-phone"></i> 0800 61 8080</p>
                        <p><i class="fas fa-globe"></i> <a href="https://www.gov.br/ibama" target="_blank" rel="noopener noreferrer">www.gov.br/ibama</a></p>
                    </div>
                </div>
                
                <div class="contato-item">
                    <img src="https://cdn-icons-png.flaticon.com/512/3176/3176272.png" alt="Disque Denúncia">
                    <div class="contato-info">
                        <h3>Disque Denúncia Ambiental</h3>
                        <p><i class="fas fa-phone"></i> 181 (em todo Brasil)</p>
                        <p><i class="fas fa-envelope"></i> disquedenuncia.ssp@gov.br</p>
                    </div>
                </div>
                
                <div class="contato-item">
                    <img src="https://cdn-icons-png.flaticon.com/512/1995/1995519.png" alt="Ministério Público">
                    <div class="contato-info">
                        <h3>Ministério Público Federal</h3>
                        <p><i class="fas fa-phone"></i> 127 (capitais e regiões metropolitanas)</p>
                        <p><i class="fas fa-globe"></i> <a href="https://www.mpf.mp.br" target="_blank" rel="noopener noreferrer">www.mpf.mp.br</a></p>
                    </div>
                </div>
            </div>
            
            <div style="margin-top: 30px; background-color: var(--fundo-claro); padding: 20px; border-radius: 8px;">
                <h3 style="color: var(--vermelho-emergencia); margin-bottom: 15px;">Como fazer uma denúncia eficiente:</h3>
                <ol style="padding-left: 20px; display: grid; gap: 10px;">
                    <li>Registre fotos ou vídeos do local (se for seguro)</li>
                    <li>Anote data, horário e local exato (coordenadas GPS se possível)</li>
                    <li>Descreva com detalhes o que está ocorrendo</li>
                    <li>Mantenha sigilo sobre sua denúncia para sua segurança</li>
                </ol>
            </div>
        </section>

        <!-- Notícias 2025 -->
        <section id="noticias" style="margin-top: 50px;">
            <h2 style="color: var(--verde-principal); margin-bottom: 20px; display: flex; align-items: center; gap: 10px;">
                <i class="far fa-newspaper"></i> Notícias Ambientais 2025
            </h2>
            
            <div class="cards">
                <div class="card">
                    <img src="https://images.unsplash.com/photo-1615834751896-42f7155d0c5a?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" alt="Acordo climático">
                    <div class="card-conteudo">
                        <h3>Novo Acordo Climático Brasileiro</h3>
                        <p>Brasil se compromete a reduzir em 50% as emissões de carbono até 2030 com novas políticas industriais e energéticas.</p>
                        <a href="https://www.gov.br/mma/pt-br/noticias/brasil-anuncia-novas-metas-ambientais-para-2030" target="_blank" rel="noopener noreferrer">
                            Ler mais <i class="fas fa-book-open"></i>
                        </a>
                    </div>
                </div>
                
                <div class="card">
                    <img src="https://images.unsplash.com/photo-1542600176-4bf7d964ecb2?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" alt="Tartarugas marinhas">
                    <div class="card-conteudo">
                        <h3>Recuperação de Espécies Ameaçadas</h3>
                        <p>Programa de conservação mostra aumento de 30% na população de tartarugas marinhas no litoral brasileiro.</p>
                        <a href="https://www.icmbio.gov.br/portal/ultimas-noticias/20-geral/12471-populacao-de-tartarugas-marinhas-cresce-30-no-brasil" target="_blank" rel="noopener noreferrer">
                            Ver detalhes <i class="fas fa-fish"></i>
                        </a>
                    </div>
                </div>
                
                <div class="card">
                    <img src="https://images.unsplash.com/photo-1508514177221-188b1cf16e9d?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1472&q=80" alt="Tecnologia verde">
                    <div class="card-conteudo">
                        <h3>Startup Brasileira Cria Plástico 100% Biodegradável</h3>
                        <p>Material feito de algas marinhas se decompõe em 30 dias e pode revolucionar a indústria de embalagens.</p>
                        <a href="https://revistapegn.globo.com/Startups/noticia/2023/06/startup-brasileira-desenvolve-plastico-100-biodegradavel.html" target="_blank" rel="noopener noreferrer">
                            Conhecer <i class="fas fa-flask"></i>
                        </a>
                    </div>
                </div>
            </div>
        </section>

        <!-- Seção de Contato -->
        <section id="contato" style="margin-top: 50px;">
            <h2 style="color: var(--verde-principal); margin-bottom: 20px; display: flex; align-items: center; gap: 10px;">
                <i class="fas fa-envelope"></i> Fale Conosco
            </h2>
            
            <div class="cards">
                <div class="card">
                    <img src="https://images.unsplash.com/photo-1542744173-8e7e53415bb0?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" alt="Equipe">
                    <div class="card-conteudo">
                        <h3>Nosso Time</h3>
                        <p>Conheça a equipe por trás do EcoConsciente e nossa missão de promover a sustentabilidade.</p>
                        <a href="mailto:equipe@ecoconsciente.org.br">
                            Contatar <i class="fas fa-users"></i>
                        </a>
                    </div>
                </div>
                
                <div class="card">
                    <img src="https://images.unsplash.com/photo-1551434678-e076c223a692?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" alt="Parcerias">
                    <div class="card-conteudo">
                        <h3>Parcerias</h3>
                        <p>Se sua organização quer colaborar com nossos projetos, entre em contato conosco.</p>
                        <a href="mailto:parcerias@ecoconsciente.org.br">
                            Propor parceria <i class="fas fa-handshake"></i>
                        </a>
                    </div>
                </div>
                
                <div class="card">
                    <img src="https://images.unsplash.com/photo-1521791055366-0d553872125f?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1469&q=80" alt="Voluntariado">
                    <div class="card-conteudo">
                        <h3>Voluntariado</h3>
                        <p>Junte-se ao nosso time de voluntários e faça a diferença em sua comunidade.</p>
                        <a href="mailto:voluntarios@ecoconsciente.org.br">
                            Ser voluntário <i class="fas fa-heart"></i>
                        </a>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- Popup do Chatbot -->
    <div class="popup" id="popup-chat">
        <div class="popup-conteudo">
            <div class="popup-cabecalho">
                <h2><i class="fas fa-robot"></i> EcoChat - Assistente Ambiental</h2>
                <button class="fechar-popup">&times;</button>
            </div>
            <div class="popup-corpo">
                <div class="chat-mensagens" id="chat-mensagens">
                    <div class="mensagem mensagem-bot">
                        Olá! Sou o EcoBot, seu assistente de sustentabilidade. Como posso ajudar você hoje? Digite /ajuda para ver os comandos disponíveis.
                    </div>
                </div>
                
                <div class="chat-input">
                    <input type="text" id="chat-input" placeholder="Digite sua mensagem...">
                    <button class="botao" id="chat-enviar">
                        <i class="fas fa-paper-plane"></i>
                    </button>
                </div>
                
                <div class="comandos-chat">
                    <h3><i class="fas fa-list"></i> Comandos Rápidos</h3>
                    <div class="lista-comandos" id="lista-comandos">
                        <!-- Comandos serão inseridos aqui pelo JavaScript -->
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Popup do Quiz -->
    <div class="popup" id="popup-quiz">
        <div class="popup-conteudo">
            <div class="popup-cabecalho">
                <h2><i class="fas fa-gamepad"></i> EcoQuiz - Teste Seu Conhecimento</h2>
                <button class="fechar-popup">&times;</button>
            </div>
            <div class="popup-corpo">
                <div id="quiz-container">
                    <div class="quiz-pergunta" id="quiz-pergunta"></div>
                    <div class="quiz-opcoes" id="quiz-opcoes"></div>
                    <div class="quiz-resultado" id="quiz-resultado"></div>
                    <div class="quiz-controles">
                        <button class="botao" id="quiz-anterior" style="display: none;">
                            <i class="fas fa-arrow-left"></i> Anterior
                        </button>
                        <button class="botao" id="quiz-proximo" style="display: none;">
                            Próxima <i class="fas fa-arrow-right"></i>
                        </button>
                        <button class="botao" id="quiz-finalizar" style="display: none;">
                            <i class="fas fa-check-circle"></i> Finalizar
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Rodapé -->
    <footer>
        <div class="rodape-conteudo">
            <div class="rodape-coluna">
                <h3>EcoConsciente</h3>
                <p>Promovendo a conscientização ambiental desde 2020. Juntos por um futuro sustentável para todos.</p>
                <div class="redes-sociais">
                    <a href="https://facebook.com/ecoconsciente" target="_blank" rel="noopener noreferrer"><img src="https://cdn-icons-png.flaticon.com/512/733/733547.png" alt="Facebook"></a>
                    <a href="https://twitter.com/ecoconsciente" target="_blank" rel="noopener noreferrer"><img src="https://cdn-icons-png.flaticon.com/512/733/733579.png" alt="Twitter"></a>
                    <a href="https://instagram.com/ecoconsciente" target="_blank" rel="noopener noreferrer"><img src="https://cdn-icons-png.flaticon.com/512/733/733558.png" alt="Instagram"></a>
                    <a href="https://youtube.com/ecoconsciente" target="_blank" rel="noopener noreferrer"><img src="https://cdn-icons-png.flaticon.com/512/2111/2111463.png" alt="YouTube"></a>
                </div>
            </div>
            
            <div class="rodape-coluna">
                <h3>Links Rápidos</h3>
                <ul>
                    <li><a href="#inicio">Início</a></li>
                    <li><a href="#reciclagem">Guia de Reciclagem</a></li>
                    <li><a href="#sustentabilidade">Dicas Sustentáveis</a></li>
                    <li><a href="#denuncias">Denúncias Ambientais</a></li>
                    <li><a href="#noticias">Notícias 2025</a></li>
                </ul>
            </div>
            
            <div class="rodape-coluna">
                <h3>Recursos</h3>
                <ul>
                    <li><a href="https://www.ibama.gov.br/calculadora-pegada-ecologica" target="_blank" rel="noopener noreferrer">Calculadora de Pegada Ecológica</a></li>
                    <li><a href="https://www.reciclasampa.com.br/ecopontos" target="_blank" rel="noopener noreferrer">Mapa de Ecopontos</a></li>
                    <li><a href="https://www.akatu.org.br" target="_blank" rel="noopener noreferrer">Guia de Consumo Consciente</a></li>
                    <li><a href="https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l12305.htm" target="_blank" rel="noopener noreferrer">Legislação Ambiental</a></li>
                    <li><a href="https://www.mma.gov.br/informma/item/152-glossario-ambiental.html" target="_blank" rel="noopener noreferrer">Glossário Ecológico</a></li>
                </ul>
            </div>
            
            <div class="rodape-coluna">
                <h3>Contato</h3>
                <ul>
                    <li><i class="fas fa-envelope"></i> contato@ecoconsciente.org.br</li>
                    <li><i class="fas fa-phone"></i> (11) 4002-8922</li>
                    <li><i class="fas fa-map-marker-alt"></i> São Paulo - SP, Brasil</li>
                </ul>
            </div>
        </div>
        
        <div class="copyright">
            <p>&copy; 2025 EcoConsciente - Todos os direitos reservados</p>
        </div>
    </footer>

    <script>
        // Controle dos Popups
        document.getElementById('botao-chat').addEventListener('click', function() {
            document.getElementById('popup-chat').style.display = 'flex';
        });

        document.getElementById('botao-quiz').addEventListener('click', function() {
            document.getElementById('popup-quiz').style.display = 'flex';
            iniciarQuiz();
        });

        document.getElementById('botao-denuncia').addEventListener('click', function() {
            window.location.href = '#denuncias';
        });

        document.querySelectorAll('.fechar-popup').forEach(btn => {
            btn.addEventListener('click', function() {
                this.closest('.popup').style.display = 'none';
            });
        });

        // Fechar popup ao clicar fora
        window.addEventListener('click', function(event) {
            if (event.target.classList.contains('popup')) {
                event.target.style.display = 'none';
            }
        });

        // Chatbot
        const comandosChat = [
            { comando: "/reciclagem", descricao: "Informações sobre reciclagem" },
            { comando: "/sustentabilidade", descricao: "Dicas de vida sustentável" },
            { comando: "/denuncia", descricao: "Como denunciar crimes ambientais" },
            { comando: "/consumo", descricao: "Dicas para consumo consciente" },
            { comando: "/energia", descricao: "Como economizar energia" },
            { comando: "/agua", descricao: "Dicas para economizar água" },
            { comando: "/noticias", descricao: "Últimas notícias ambientais" },
            { comando: "/ajuda", descricao: "Mostra todos os comandos" }
        ];

        // Preencher lista de comandos
        const listaComandos = document.getElementById('lista-comandos');
        comandosChat.forEach(cmd => {
            const item = document.createElement('div');
            item.className = 'comando-item';
            item.innerHTML = `
                <span>${cmd.comando}</span>
                <button class="botao" data-comando="${cmd.comando}">Usar</button>
            `;
            listaComandos.appendChild(item);
        });

        // Adicionar eventos aos botões de comando
        document.querySelectorAll('[data-comando]').forEach(btn => {
            btn.addEventListener('click', function() {
                const comando = this.getAttribute('data-comando');
                document.getElementById('chat-input').value = comando;
                document.getElementById('chat-enviar').click();
            });
        });

        // Funções do chat
        const chatMensagens = document.getElementById('chat-mensagens');
        const chatInput = document.getElementById('chat-input');
        const chatEnviar = document.getElementById('chat-enviar');

        function adicionarMensagem(autor, mensagem, isBot = false) {
            const msgDiv = document.createElement('div');
            msgDiv.className = `mensagem ${isBot ? 'mensagem-bot' : 'mensagem-usuario'}`;
            msgDiv.textContent = mensagem;
            chatMensagens.appendChild(msgDiv);
            chatMensagens.scrollTop = chatMensagens.scrollHeight;
        }

        chatEnviar.addEventListener('click', enviarMensagem);
        chatInput.addEventListener('keypress', function(e) {
            if (e.key === 'Enter') enviarMensagem();
        });

        function enviarMensagem() {
            const mensagem = chatInput.value.trim();
            if (mensagem) {
                adicionarMensagem('Você', mensagem);
                chatInput.value = '';
                responderChatbot(mensagem);
            }
        }

        function responderChatbot(mensagem) {
            let resposta = "Desculpe, não entendi. Digite /ajuda para ver os comandos disponíveis.";
            
            if (mensagem.toLowerCase().includes('oi') || mensagem.toLowerCase().includes('olá')) {
                resposta = "Olá! Sou o EcoBot, seu assistente de sustentabilidade. Como posso ajudar você hoje?";
            } 
            else if (mensagem === '/reciclagem' || mensagem.toLowerCase().includes('reciclagem')) {
                resposta = "📌 Em 2025, a reciclagem no Brasil segue novas regras:\n\n" +
                          "🔷 SEPARAÇÃO OBRIGATÓRIA em 5 categorias:\n" +
                          "1️⃣ Orgânicos\n2️⃣ Papel/papelão\n3️⃣ Plásticos\n4️⃣ Metais\n5️⃣ Vidros\n\n" +
                          "♻️ Novos ecopontos inteligentes estão disponíveis em todas as capitais.\n" +
                          "🔍 Use nosso mapa de coleta seletiva: ecoconsciente.org.br/mapa";
            }
            else if (mensagem === '/sustentabilidade' || mensagem.toLowerCase().includes('sustentável')) {
                resposta = "🌱 DICAS PARA UMA VIDA SUSTENTÁVEL EM 2025:\n\n" +
                          "🏠 CASA:\n- Telhados verdes reduzem temperatura em até 5°C\n" +
                          "- Sistemas de reaproveitamento de água são obrigatórios em novas construções\n\n" +
                          "🛒 CONSUMO:\n- Prefira produtos com selo 'Carbono Neutro'\n" +
                          "- Aplicativos como 'EcoCompra' ajudam a encontrar alternativas sustentáveis\n\n" +
                          "🚗 TRANSPORTE:\n- Programa 'Carro Zero' incentiva veículos elétricos com descontos";
            }
            else if (mensagem === '/denuncia' || mensagem.toLowerCase().includes('denúncia')) {
                resposta = "⚠️ DENÚNCIAS AMBIENTAIS - 2025:\n\n" +
                          "Se presenciar crimes ambientais, contate:\n\n" +
                          "📞 IBAMA: 0800 61 8080 (24h)\n" +
                          "📱 App 'Denúncia Ambiental' (disponível para Android e iOS)\n" +
                          "🌐 Ministério Público: www.mpf.mp.br/denuncia\n\n" +
                          "ℹ️ Lembre-se: fotos, vídeos e localização exata ajudam nas investigações.";
            }
            else if (mensagem === '/consumo' || mensagem.toLowerCase().includes('consumo')) {
                resposta = "🛍️ CONSUMO CONSCIENTE EM 2025:\n\n" +
                          "✅ Compre de marcas com logística reversa\n" +
                          "✅ Prefira embalagens retornáveis ou biodegradáveis\n" +
                          "✅ Utilize apps de compartilhamento de produtos\n" +
                          "✅ Participe de feiras de trocas em sua cidade\n\n" +
                          "💰 Bônus: Consumidores sustentáveis recebem descontos no IPVA em vários estados.";
            }
            else if (mensagem === '/energia' || mensagem.toLowerCase().includes('energia')) {
                resposta = "💡 ECONOMIA DE ENERGIA - NOVIDADES 2025:\n\n" +
                          "⚡ Tarifa branca: energia mais barata das 10h às 17h\n" +
                          "☀️ Painéis solares têm isenção de impostos em 23 estados\n" +
                          "🏢 Edifícios com certificação 'Energia Zero' ganham redução no IPTU\n\n" +
                          "🔌 Dica: Use dispositivos inteligentes para desligar aparelhos automaticamente.";
            }
            else if (mensagem === '/agua' || mensagem.toLowerCase().includes('água')) {
                resposta = "💧 CUIDADOS COM A ÁGUA EM 2025:\n\n" +
                          "🌧️ Sistemas de captação de água da chuva são obrigatórios em SP, RJ e MG\n" +
                          "🚿 Redutores de vazão reduzem consumo em até 60%\n" +
                          "🏡 Novas tecnologias permitem reuso de água até 5 vezes na mesma residência\n\n" +
                          "⚠️ Atenção: Multas por desperdício aumentaram em 300% desde 2023.";
            }
            else if (mensagem === '/noticias' || mensagem.toLowerCase().includes('notícia')) {
                resposta = "📰 ÚLTIMAS NOTÍCIAS AMBIENTAIS - 2025:\n\n" +
                          "1. Brasil atinge meta de 30% de energia renovável\n" +
                          "2. Nova lei proíbe plásticos de uso único em todo território nacional\n" +
                          "3. População de araras-azuis cresce 25% no Pantanal\n" +
                          "4. Startup brasileira cria bioplástico que se decompõe em 15 dias\n\n" +
                          "Leia mais em: ecoconsciente.org.br/noticias";
            }
            else if (mensagem === '/ajuda') {
                resposta = "🛟 COMANDOS DISPONÍVEIS:\n\n" + 
                          comandosChat.map(c => `🔹 ${c.comando} - ${c.descricao}`).join('\n') +
                          "\n\nTambém posso responder perguntas sobre meio ambiente em geral!";
            }
            
            // Simular digitação
            setTimeout(() => {
                adicionarMensagem("EcoBot", resposta, true);
            }, 800);
        }

        // Quiz
        const quizPerguntas = [
            {
                pergunta: "Qual desses materiais NÃO pode ser reciclado em 2025 segundo as novas normas?",
                opcoes: [
                    "Embalagens de salgadinho metalizadas",
                    "Copos descartáveis de papel",
                    "Garrafas PET transparentes",
                    "Frascos de vidro colorido"
                ],
                resposta: 0
            },
            {
                pergunta: "Qual é a penalidade para empresas que não cumprirem a logística reversa em 2025?",
                opcoes: [
                    "Multa de até R$ 50 mil",
                    "Suspensão das atividades por 30 dias",
                    "Multa de até R$ 500 mil",
                    "Nenhuma, é apenas uma recomendação"
                ],
                resposta: 2
            },
            {
                pergunta: "Qual destas ações reduz MAIS a pegada de carbono individual?",
                opcoes: [
                    "Usar transporte público 3 vezes por semana",
                    "Reduzir consumo de carne vermelha pela metade",
                    "Instalar 2 painéis solares em casa",
                    "Plantar 5 árvores nativas por ano"
                ],
                resposta: 1
            },
            {
                pergunta: "Qual tecnologia está revolucionando a reciclagem em 2025?",
                opcoes: [
                    "Robôs separadores com inteligência artificial",
                    "Plásticos que mudam de cor quando contaminados",
                    "Lixeiras que pesam o lixo e dão descontos",
                    "Todas as alternativas anteriores"
                ],
                resposta: 3
            },
            {
                pergunta: "Qual cidade brasileira foi eleita a mais sustentável em 2025?",
                opcoes: [
                    "Curitiba - PR",
                    "Belo Horizonte - MG",
                    "Florianópolis - SC",
                    "João Pessoa - PB"
                ],
                resposta: 0
            },
            {
                pergunta: "Qual porcentagem de energia elétrica do Brasil vem de fontes renováveis em 2025?",
                opcoes: [
                    "45%",
                    "60%",
                    "75%",
                    "90%"
                ],
                resposta: 1
            },
            {
                pergunta: "Qual destes NÃO é um benefício do novo selo 'Carbono Neutro' para produtos?",
                opcoes: [
                    "Desconto no IPI",
                    "Prioridade nas prateleiras",
                    "Isenção de ICMS",
                    "Redução no frete"
                ],
                resposta: 3
            },
            {
                pergunta: "Quantos litros de água uma família pode economizar por ano com o novo sistema de reuso obrigatório?",
                opcoes: [
                    "20 mil litros",
                    "50 mil litros",
                    "100 mil litros",
                    "200 mil litros"
                ],
                resposta: 2
            },
            {
                pergunta: "Qual animal saiu da lista de espécies ameaçadas em 2025?",
                opcoes: [
                    "Arara-azul",
                    "Mico-leão-dourado",
                    "Boto-cor-de-rosa",
                    "Tamanduá-bandeira"
                ],
                resposta: 1
            },
            {
                pergunta: "Qual foi a redução média no desmatamento da Amazônia em 2025 comparado a 2020?",
                opcoes: [
                    "20%",
                    "40%",
                    "60%",
                    "80%"
                ],
                resposta: 2
            }
        ];

        let quizAtual = 0;
        let respostasUsuario = [];
        let pontuacao = 0;

        function iniciarQuiz() {
            quizAtual = 0;
            respostasUsuario = [];
            pontuacao = 0;
            mostrarPergunta();
            
            document.getElementById('quiz-anterior').style.display = 'none';
            document.getElementById('quiz-proximo').style.display = 'inline-block';
            document.getElementById('quiz-finalizar').style.display = 'none';
            document.getElementById('quiz-resultado').textContent = '';
        }

        function mostrarPergunta() {
            const pergunta = quizPerguntas[quizAtual];
            document.getElementById('quiz-pergunta').textContent = `${quizAtual + 1}. ${pergunta.pergunta}`;
            
            const opcoesContainer = document.getElementById('quiz-opcoes');
            opcoesContainer.innerHTML = '';
            
            pergunta.opcoes.forEach((opcao, index) => {
                const opcaoElement = document.createElement('div');
                opcaoElement.className = 'quiz-opcao';
                opcaoElement.textContent = opcao;
                opcaoElement.dataset.indice = index;
                opcaoElement.addEventListener('click', selecionarResposta);
                opcoesContainer.appendChild(opcaoElement);
            });
            
            // Atualizar controles
            document.getElementById('quiz-anterior').style.display = quizAtual > 0 ? 'inline-block' : 'none';
            document.getElementById('quiz-proximo').style.display = quizAtual < quizPerguntas.length - 1 ? 'inline-block' : 'none';
            document.getElementById('quiz-finalizar').style.display = quizAtual === quizPerguntas.length - 1 ? 'inline-block' : 'none';
            
            // Mostrar resposta selecionada anteriormente, se houver
            if (respostasUsuario[quizAtual] !== undefined) {
                const opcoes = document.querySelectorAll('.quiz-opcao');
                opcoes[respostasUsuario[quizAtual]].classList.add('selecionada');
            }
        }

        function selecionarResposta(e) {
            const opcoes = document.querySelectorAll('.quiz-opcao');
            opcoes.forEach(opcao => opcao.classList.remove('selecionada'));
            
            e.target.classList.add('selecionada');
            respostasUsuario[quizAtual] = parseInt(e.target.dataset.indice);
        }

        document.getElementById('quiz-anterior').addEventListener('click', function() {
            if (quizAtual > 0) {
                quizAtual--;
                mostrarPergunta();
            }
        });

        document.getElementById('quiz-proximo').addEventListener('click', function() {
            if (respostasUsuario[quizAtual] === undefined) {
                alert('Por favor, selecione uma resposta antes de continuar.');
                return;
            }
            
            if (quizAtual < quizPerguntas.length - 1) {
                quizAtual++;
                mostrarPergunta();
            }
        });

        document.getElementById('quiz-finalizar').addEventListener('click', finalizarQuiz);

        function finalizarQuiz() {
            if (respostasUsuario[quizAtual] === undefined) {
                alert('Por favor, selecione uma resposta antes de finalizar.');
                return;
            }
            
            // Calcular pontuação
            pontuacao = 0;
            for (let i = 0; i < quizPerguntas.length; i++) {
                if (respostasUsuario[i] === quizPerguntas[i].resposta) {
                    pontuacao++;
                }
            }
            
            // Mostrar resultado
            const resultado = document.getElementById('quiz-resultado');
            resultado.innerHTML = `
                <h3>Quiz Concluído!</h3>
                <p>Sua pontuação: ${pontuacao}/${quizPerguntas.length}</p>
                <p>${pontuacao >= 8 ? '🎉 Excelente! Você é um expert em sustentabilidade!' : 
                   pontuacao >= 5 ? '👍 Bom trabalho! Continue aprendendo sobre meio ambiente!' : 
                   '🌱 Você pode melhorar! Aproveite para explorar nosso site e aprender mais!'}</p>
                <button class="botao" id="quiz-reiniciar" style="margin-top: 15px;">
                    <i class="fas fa-redo"></i> Fazer Novamente
                </button>
            `;
            
            document.getElementById('quiz-reiniciar').addEventListener('click', iniciarQuiz);
            
            // Esconder controles
            document.getElementById('quiz-anterior').style.display = 'none';
            document.getElementById('quiz-proximo').style.display = 'none';
            document.getElementById('quiz-finalizar').style.display = 'none';
        }
    </script>
</body>
</html>
