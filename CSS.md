/* Reseta os estilos globais para todos os elementos */
* {
    margin: 0; /* Remove as margens padrão */
    padding: 0; /* Remove o preenchimento padrão */
    box-sizing: border-box; /* Inclui preenchimento e borda na largura/altura total do elemento */
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; /* Define a família de fontes padrão */
}

/* Estilos do corpo */
body {
    background-color: #f0f0f0; /* Define um fundo cinza claro */
    overflow-x: hidden; /* Oculta a barra de rolagem horizontal */
}

/* Estilos do cabeçalho */
.cabecalho {
    background: linear-gradient(135deg, #740001 0%, #1a1a1a 100%); /* Gradiente de vermelho para preto */
    color: #eeba30; /* Cor do texto dourado */
    display: flex; /* Container flexível */
    justify-content: space-between; /* Espaço entre os itens do cabeçalho */
    align-items: center; /* Centraliza os itens verticalmente */
    padding: 20px 5%; /* Preenchimento em todos os lados */
    position: sticky; /* Posicionamento fixo na rolagem */
    top: 0; /* Fixa ao topo */
    z-index: 1000; /* Índice Z alto para permanecer no topo */
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.3); /* Efeito de sombra -> Horizontal, Vertical, Blur */
}

/* Container dos itens do cabeçalho */
.cabecalho-itens {
    display: flex; /* Container flexível */
    list-style: none; /* Remove os marcadores da lista */
    gap: 20px; /* Espaço entre os itens */
}

/* Itens da lista do cabeçalho */
.cabecalho-lista {
    display: inline-block; /* Exibição em linha com comportamento de bloco */
}

/* Links do cabeçalho */
.cabecalho-lista a {
    color: #eeba30; /* Cor do texto dourado */
    text-decoration: none; /* Remove o sublinhado */
    font-weight: bold; /* Texto em negrito */
    padding: 10px 15px; /* Preenchimento ao redor do texto */
    border-radius: 5px; /* Bordas arredondadas */
    transition: all 0.3s; /* Transição suave para efeitos de foco */
}

/* Efeito de foco nos links do cabeçalho */
.cabecalho-lista a:hover {
    background-color: rgba(238, 186, 48, 0.2); /* Fundo dourado semitransparente */
}

/* Imagem do cabeçalho */
.imagem-cabecalho {
    width: 120px; /* Largura fixa */
    height: auto; /* Altura automática para manter a proporção */
    filter: drop-shadow(0 0 5px rgba(238, 186, 48, 0.7)); /* Efeito de brilho Horizontal, Vertical, Blur*/
    transition: transform 0.3s ease; /* Transição suave da transformação */
}

/* Efeito de foco na imagem do cabeçalho */
.imagem-cabecalho:hover {
    transform: scale(1.05); /* Aumenta ligeiramente ao passar o mouse */
}

/* Seção da escola */
.escola {
    background-image: url('./Gifs/casa_hogwarts.gif'); /* Imagem de fundo */
    background-size: cover; /* Cobrir todo o elemento */
    background-position: center; /* Centralizar o fundo */
    background-repeat: no-repeat; /* Não repetir */
    display: flex; /* Container flexível */
    justify-content: center; /* Centralizar horizontalmente */
    align-items: center; /* Centralizar verticalmente */
    padding: 80px 5% 40px; /* Valores de preenchimento Topo, laterais, Base */
    position: relative; /* Posicionamento relativo */
    overflow: hidden; /* Ocultar o que estiver fora */
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.5); /* Efeito de sombra */
    color: #f0f0f0; /* Texto cinza claro */
    text-align: center; /* Centralizar o texto */
    min-height: auto; /* Altura mínima */
}

/* Sobreposição da seção da escola */
.escola::before {
    content: ""; /* Conteúdo vazio */
    position: absolute; /* Posicionamento absoluto */
    top: 0; /* Posicionar no topo */
    left: 0; /* Posicionar à esquerda */
    width: 100%; /* Largura total */
    height: 100%; /* Altura total */
    background: url('./Assets/Imagens/hogwarts-crest-white.png') center/contain no-repeat; /* Marca d'água do brasão */
    opacity: 0.1; /* Baixa opacidade */
    pointer-events: none; /* Ignorar eventos de ponteiro */
    border-radius: 15px; /* Bordas arredondadas */
}

/* Container do conteúdo da seção da escola */
.escola-div-conteudo {
    width: 90%; /* 90% de largura */
    padding: 30px; /* Preenchimento interno */
    background-color: rgba(0, 0, 0, 0.6); /* Fundo preto semitransparente */
    border-radius: 10px; /* Bordas arredondadas */
    position: relative; /* Posicionamento relativo */
    z-index: 2; /* Ordem de empilhamento */
}

/* Título da escola */
.titulo-escola {
    padding: 20px 0; /* Preenchimento superior e inferior */
    color: #eeba30; /* Cor dourada */
    font-size: 36px; /* Tamanho da fonte grande */
    text-shadow: 3px 3px 5px rgba(0, 0, 0, 0.8); /* Sombra no texto */
    position: relative; /* Posicionamento relativo */
}

/* Sublinhado do título da escola */
.titulo-escola::after {
    content: ""; /* Conteúdo vazio */
    display: block; /* Exibição em bloco */
    width: 80px; /* Largura da linha */
    height: 3px; /* Altura da linha */
    background: #eeba30; /* Cor dourada */
    margin: 8px auto 0; /* Margem centralizada */
    border-radius: 2px; /* Ligeiramente arredondado */
}

/* Parágrafos de texto da escola */
.texto-um-escola,
.texto-dois-escola {
    padding: 10px 0; /* Preenchimento superior e inferior */
    color: #d3d3d3; /* Texto cinza claro */
    font-size: 16px; /* Tamanho da fonte médio */
    line-height: 1.5; /* Espaçamento entre linhas */
    text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5); /* Sombra sutil no texto */
}

/* Seção das casas */
.casas {
    padding: 40px 5%; /* Valores de preenchimento */
    background-color: #f9f5e8; /* Cor de pergaminho */
}

/* Título das casas */
.casas-titulo {
    text-align: center; /* Centralizar o texto */
    font-size: 36px; /* Tamanho da fonte grande */
    color: #5d2906; /* Cor marrom */
    margin-bottom: 30px; /* Margem inferior */
    position: relative; /* Posicionamento relativo */
}

/* Sublinhado do título das casas */
.casas-titulo::after {
    content: ""; /* Conteúdo vazio */
    display: block; /* Exibição em bloco */
    width: 120px; /* Largura da linha */
    height: 3px; /* Altura da linha */
    background: linear-gradient(to right, #740001, #d3a625); /* Gradiente */
    margin: 10px auto 0; /* Margem centralizada topo laterais base */
    border-radius: 2px; /* Ligeiramente arredondado */
}

/* Container das casas */
.casas-container {
    display: grid; /* Layout em grade */
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); /* Colunas responsivas */
    gap: 20px; /* Espaço entre os itens */
    max-width: 100%; /* Largura total */
    margin: 0 auto; /* Centralizado */
    padding: 0 10px; /* Preenchimento horizontal */
}

/* Cartão da casa */
.casa-card {
    background: rgba(255, 255, 255, 0.9); /* Branco semitransparente */
    border-radius: 15px; /* Bordas arredondadas */
    padding: 20px; /* Preenchimento interno */
    text-align: center; /* Centralizar o conteúdo */
    box-shadow: 0 8px 16px rgba(0, 0, 0, 0.1); /* Sombra */
    transition: all 0.3s ease; /* Transições suaves */
    border: 2px solid transparent; /* Borda invisível */
}

/* Efeito de foco no cartão da casa */
.casa-card:hover {
    transform: translateY(-5px); /* Levantar */
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2); /* Sombra mais forte */
}

/* Imagem da casa */
.casa-imagem {
    width: 80px; /* Largura fixa */
    height: 80px; /* Altura fixa */
    margin: 0 auto 15px; /* Centralizado com margem inferior */
    transition: transform 0.3s ease; /* Transição suave da transformação */
}

/* Efeito de foco na imagem da casa */
.casa-card:hover .casa-imagem {
    transform: scale(1.05); /* Aumentar ligeiramente */
}

/* Nome da casa */
.casa-card h3 {
    font-size: 20px; /* Tamanho da fonte médio */
    margin-bottom: 10px; /* Margem inferior */
    color: #5d2906; /* Cor marrom */
}

/* Descrição da casa */
.casa-card p {
    color: #555; /* Texto cinza escuro */
    line-height: 1.5; /* Espaçamento entre linhas */
    font-size: 14px; /* Tamanho da fonte pequeno */
}

/* Seção dos estudantes */
.estudantes {
    background-color: #f5f5f5; /* Cinza claro */
    padding: 40px 5%; /* Valores de preenchimento */
}

/* Título dos estudantes */
.estudante-título {
    text-align: center; /* Centralizar o texto */
    padding: 15px 0 30px; /* Valores de preenchimento */
    font-size: 36px; /* Tamanho da fonte grande */
    color: #5d2906; /* Cor marrom */
    text-transform: uppercase; /* Texto em maiúsculas */
    letter-spacing: 1px; /* Espaçamento entre letras */
    position: relative; /* Posicionamento relativo */
}

/* Sublinhado do título dos estudantes */
.estudante-título::after {
    content: ""; /* Conteúdo vazio */
    display: block; /* Exibição em bloco */
    width: 120px; /* Largura da linha */
    height: 3px; /* Altura da linha */
    background: linear-gradient(to right, #740001, #d3a625); /* Gradiente */
    margin: 10px auto 0; /* Margem centralizada */
    border-radius: 2px; /* Ligeiramente arredondado */
}

/* Container de todos os estudantes */
.estudantes-todos {
    display: grid; /* Layout em grade */
    grid-template-columns: repeat(auto-fit, minmax(150px, 1fr)); /* Colunas responsivas */
    grid-template-rows: auto; /* Linhas automáticas */
    gap: 15px; /* Espaço entre os itens */
    max-width: 100%; /* Largura total */
    margin: 0 auto; /* Centralizado */
    padding: 0 10px; /* Preenchimento horizontal */
}

/* Container do estudante */
.estudante-container {
    position: relative; /* Posicionamento relativo */
    display: flex; /* Container flexível */
    flex-direction: column; /* Layout em coluna */
    align-items: center; /* Centralizar os itens */
    gap: 8px; /* Espaço entre os itens */
    padding: 15px; /* Preenchimento interno */
    background-color: rgba(255, 255, 255, 0.9); /* Branco semitransparente */
    border-radius: 15px; /* Bordas arredondadas */
    box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2); /* Sombra */
    transition: all 0.3s ease, transform 0.3s ease; /* Transições suaves */
    border: 1px solid #d3a625; /* Borda dourada */
    transform-style: preserve-3d; /* Espaço 3D */
}

/* Efeito de foco no container do estudante */
.estudante-container:hover {
    transform: translateY(-5px) rotateY(5deg) rotateX(-3deg); /* Inclinação 3D */
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3); /* Sombra mais forte */
}

/* Imagem do estudante */
.imagem-estudante {
    width: 100px; /* Largura fixa */
    height: 100px; /* Altura fixa */
    object-fit: cover; /* Cobrir a área */
    border-radius: 50%; /* Circular */
    border: 3px solid #d3a625; /* Borda dourada */
    cursor: pointer; /* Cursor de ponteiro */
    transition: all 0.3s ease; /* Transições suaves */
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); /* Sombra */
}

/* Efeito de foco na imagem do estudante */
.imagem-estudante:hover {
    border-color: #740001; /* Borda vermelha */
    transform: scale(1.03); /* Aumentar ligeiramente */
}

/* Nome do estudante */
.estudante-nome {
    font-size: 16px; /* Tamanho da fonte médio */
    font-weight: bold; /* Texto em negrito */
    color: #5d2906; /* Cor marrom */
    text-align: center; /* Centralizar o texto */
    margin-top: 5px; /* Margem superior */
}

/* Logo da casa do estudante */
.estudante-casa {
    width: 30px; /* Largura fixa */
    height: 30px; /* Altura fixa */
    transition: transform 0.3s ease; /* Transição suave da transformação */
}

/* Efeito de foco no logo da casa do estudante */
.estudante-casa:hover {
    transform: scale(1.1); /* Aumentar ligeiramente */
}

/* Cartão GIF (oculto por padrão) */
.gif-card {
    display: none; /* Oculto */
    position: absolute; /* Posicionamento absoluto */
    top: 0; /* Posicionar no topo */
    left: 0; /* Posicionar à esquerda */
    width: 100%; /* Largura total */
    height: 100%; /* Altura total */
    justify-content: center; /* Centralizar horizontalmente */
    align-items: center; /* Centralizar verticalmente */
    z-index: 100; /* Ordem de empilhamento */
    pointer-events: none; /* Ignorar eventos de ponteiro */
    background-color: rgba(0, 0, 0, 0.85); /* Preto semitransparente */
    border-radius: 15px; /* Bordas arredondadas */
    border: 2px solid #d3a625; /* Borda dourada */
    animation: fadeIn 0.3s ease; /* Animação de fadeIn */
    transform-style: preserve-3d; /* Espaço 3D */
}

/* Animação de fadeIn */
@keyframes fadeIn {
    from {
        opacity: 0; /* Começar invisível */
    }
    to {
        opacity: 1; /* Terminar visível */
    }
}

/* Imagem GIF */
.gif-imagem {
    max-width: 90%; /* Largura máxima */
    max-height: 90%; /* Altura máxima */
    object-fit: contain; /* Ajustar mantendo a proporção */
    border-radius: 10px; /* Ligeiramente arredondado */
}

/* Rodapé */
.rodape {
    background: linear-gradient(135deg, #1a1a1a 0%, #740001 100%); /* Gradiente */
    text-align: center; /* Centralizar o conteúdo */
    padding: 20px 0; /* Preenchimento superior e inferior */
    position: relative; /* Posicionamento relativo */
}

/* Borda superior do rodapé */
.rodape::before {
    content: ""; /* Conteúdo vazio */
    position: absolute; /* Posicionamento absoluto */
    top: 0; /* Posicionar no topo */
    left: 0; /* Posicionar à esquerda */
    width: 100%; /* Largura total */
    height: 2px; /* Linha fina */
    background: linear-gradient(to right, #d3a625, #740001, #d3a625); /* Gradiente */
}

/* Imagem do rodapé */
.imagem-rodape {
    width: 150px; /* Largura fixa */
    padding: 10px 0; /* Preenchimento superior e inferior */
    filter: brightness(0) invert(1); /* Tornar branco */
    opacity: 0.8; /* Ligeiramente transparente */
    transition: opacity 0.3s ease; /* Transição suave da opacidade */
}

/* Efeito de foco na imagem do rodapé */
.imagem-rodape:hover {
    opacity: 1; /* Totalmente visível */
}

/* Container social do rodapé */
.rodape div {
    display: flex; /* Container flexível */
    justify-content: center; /* Centralizar horizontalmente */
    align-items: center; /* Centralizar verticalmente */
    margin-top: 10px; /* Margem superior */
}

/* Ícones sociais do rodapé */
.rodape div img {
    width: 25px; /* Largura fixa */
    margin: 0 8px; /* Margem horizontal */
    transition: transform 0.3s ease; /* Transição suave da transformação */
}

/* Efeito de foco nos ícones sociais do rodapé */
.rodape div img:hover {
    transform: scale(1.1); /* Aumentar ligeiramente */
}

/* Texto do rodapé */
.rodape-texto {
    color: #eeba30; /* Cor dourada */
    font-size: 14px; /* Tamanho da fonte pequeno */
    margin-left: 8px; /* Margem esquerda */
    text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5); /* Sombra no texto */
}

/* Sobreposição da carta (oculta por padrão) */
.carta-overlay {
    position: fixed; /* Posicionamento fixo */
    top: 0; /* Posicionar no topo */
    left: 0; /* Posicionar à esquerda */
    width: 100%; /* Largura total */
    height: 100%; /* Altura total */
    background-color: rgba(0, 0, 0, 0.8); /* Preto semitransparente */
    display: flex; /* Container flexível */
    justify-content: center; /* Centralizar horizontalmente */
    align-items: center; /* Centralizar verticalmente */
    z-index: 9999; /* Ordem de empilhamento muito alta */
    display: none; /* Oculto por padrão */
    animation: aparecer 0.5s ease-out; /* Animação de aparecer */
}

/* Animação de aparecer */
@keyframes aparecer {
    from {
        opacity: 0; /* Começar invisível */
    }
    to {
        opacity: 1; /* Terminar visível */
    }
}

/* GIF da carta */
.carta-gif {
    max-width: 90%; /* Largura máxima */
    max-height: 90%; /* Altura máxima */
    object-fit: contain; /* Ajustar mantendo a proporção */
    animation: voar 2s ease-in-out; /* Animação de voar */
}

/* Animação de voar */
@keyframes voar {
    0% {
        transform: translateY(-100px) rotate(-15deg) scale(0.5); /* Posição inicial */
        opacity: 0; /* Começar invisível */
    }
    70% {
        transform: translateY(20px) rotate(5deg) scale(1.1); /* Posição intermediária */
        opacity: 1; /* Visível */
    }
    100% {
        transform: translateY(0) rotate(0) scale(1); /* Posição final */
        opacity: 1; /* Visível */
    }
}

/* Estilos responsivos para tablets e menores */
@media (max-width: 768px) {
    .escola {
        padding: 60px 5% 30px; /* Preenchimento ajustado */
    }

    .titulo-escola {
        font-size: 30px; /* Fonte menor */
    }

    .casas-titulo {
        font-size: 30px; /* Fonte menor */
        margin-bottom: 25px; /* Margem menor */
    }

    .casas-container {
        grid-template-columns: repeat(auto-fit, minmax(180px, 1fr)); /* Colunas ajustadas */
        gap: 15px; /* Espaço menor */
    }

    .casa-card h3 {
        font-size: 18px; /* Fonte menor */
    }

    .estudante-título {
        font-size: 30px; /* Fonte menor */
        padding: 10px 0 20px; /* Preenchimento ajustado */
    }

    .estudantes-todos {
        grid-template-columns: repeat(auto-fit, minmax(120px, 1fr)); /* Colunas ajustadas */
        gap: 10px; /* Espaço menor */
    }

    .imagem-estudante {
        width: 80px; /* Imagem menor */
        height: 80px; /* Imagem menor */
    }

    .estudante-nome {
        font-size: 14px; /* Fonte menor */
    }

    .estudante-casa {
        width: 25px; /* Ícone menor */
        height: 25px; /* Ícone menor */
    }
}

/* Forçar 2 colunas em tablets muito pequenos */
@media (max-width: 600px) {
    .casas-container {
        grid-template-columns: repeat(2, 1fr); /* Forçar 2 colunas */
    }
}

/* Estilos responsivos para telefones celulares */
@media (max-width: 480px) {
    .escola {
        padding: 40px 5% 20px; /* Preenchimento menor */
    }

    .titulo-escola {
        font-size: 24px; /* Fonte menor */
    }

    .texto-um-escola,
    .texto-dois-escola {
        font-size: 14px; /* Fonte menor */
    }

    .casas-titulo {
        font-size: 24px; /* Fonte menor */
        margin-bottom: 20px; /* Margem menor */
    }

    .casas-container {
        grid-template-columns: repeat(auto-fit, minmax(100px, 1fr)); /* Colunas ajustadas */
        grid-template-columns: 1fr; /* Forçar 1 coluna */
        gap: 10px; /* Espaço menor */
    }

    .casa-card {
        padding: 15px; /* Preenchimento menor */
    }

    .casa-card h3 {
        font-size: 16px; /* Fonte menor */
    }

    .casa-card p {
        font-size: 12px; /* Fonte menor */
    }

    .estudante-título {
        font-size: 24px; /* Fonte menor */
        padding: 5px 0 15px; /* Preenchimento menor */
    }

    .estudantes-todos {
        grid-template-columns: repeat(auto-fit, minmax(80px, 1fr)); /* Colunas ajustadas */
        gap: 8px; /* Espaço menor */
    }

    .imagem-estudante {
        width: 60px; /* Imagem menor */
        height: 60px; /* Imagem menor */
    }

    .estudante-nome {
        font-size: 12px; /* Fonte menor */
    }

    .rodape-texto {
        font-size: 12px; /* Fonte menor */
    }

    .cabecalho {
        padding: 15px 5%; /* Preenchimento menor */
    }

    .cabecalho-lista {
        gap: 10px; /* Espaço menor */
    }

    .cabecalho-lista a {
        padding: 8px 10px; /* Preenchimento menor */
        font-size: 14px; /* Fonte menor */
    }

    .imagem-cabecalho {
        width: 80px; /* Imagem menor */
    }
}
