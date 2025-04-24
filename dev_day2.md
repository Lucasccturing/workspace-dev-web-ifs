**Instruções Gerais:** Para cada questão abaixo, desenvolva os arquivos HTML e CSS necessários para atender aos requisitos especificados. Utilize boas práticas de codificação, HTML5 semântico e CSS3 moderno.

---

**Questão 1: Página de Apresentação Simples**

-   **Objetivo:** Criar uma página web estática básica de boas-vindas.
-   **Cenário:** Um pequeno negócio (padaria "Pão & Prosa") necessita de uma presença online inicial mínima.
-   **Requisitos do Solicitante:**
    -   Um título principal exibindo "Bem-vindo à Pão & Prosa!", que deve estar centralizado na página, em negrito e com uma cor marrom (sugestão: `#A0522D`).
    -   Abaixo do título, um parágrafo de texto: "O lugar perfeito para seu café da manhã e lanche da tarde. Venha provar nossos pães artesanais e bolos caseiros!". Este texto deve usar a cor preta padrão e uma fonte comum sem serifa (ex: Arial, Helvetica, sans-serif).
    -   O fundo da página deve ser branco.
-   **Tarefa Técnica:** Estruturar o conteúdo usando `<h1>` e `<p>`. Aplicar estilos via CSS externo (`style.css`) para cores (`color`), alinhamento (`text-align`), peso da fonte (`font-weight`) e família de fontes (`font-family`).

**Questão 2: Cartão de Visita Digital**

-   **Objetivo:** Desenvolver uma página que funcione como um cartão de visita online.
-   **Cenário:** Um fotógrafo autônomo (Carlos Almeida) deseja uma página simples para apresentar suas informações de contato.
-   **Requisitos do Solicitante:**
    -   O nome "Carlos Almeida" deve aparecer em destaque (fonte maior e em negrito).
    -   Logo abaixo, a profissão "Fotógrafo de Paisagens" em tamanho normal.
    -   Abaixo da profissão, uma imagem quadrada representando o fotógrafo (utilizar um placeholder de 150x150 pixels).
    -   Abaixo da imagem, as informações de contato: E-mail "carlos.foto@email.com" e Telefone "(11) 98765-4321", cada um em sua linha.
    -   Todo este conjunto (nome, profissão, foto, contatos) deve estar visualmente agrupado dentro de uma caixa com uma borda cinza fina (`solid 1px #cccccc`).
    -   Deve haver um espaçamento interno (padding) entre o conteúdo e a borda da caixa (sugestão: 20 pixels).
    -   A caixa inteira deve estar centralizada horizontalmente na página.
    -   O fundo da página (fora da caixa) deve ter uma cor cinza muito clara (sugestão: `#f0f0f0`).
-   **Tarefa Técnica:** Utilizar HTML para estruturar semanticamente as informações (ex: `<div>` ou `<section>` para o cartão, `<h2>`, `<p>`, `<img>`, `<a>` para email/tel). Aplicar CSS para estilização: Box Model (`border`, `padding`, `margin` para centralização), `text-align`, `background-color` e controle de dimensões da imagem.

**Questão 3: Lista de Serviços Estilizada**

-   **Objetivo:** Criar uma página que apresente uma lista de serviços com estilo customizado.
-   **Cenário:** Uma empresa de jardinagem ("Jardim Feliz Ltda.") quer listar seus serviços de forma mais atraente que uma lista padrão.
-   **Requisitos do Solicitante:**
    -   Um título "Nossos Serviços de Jardinagem".
    -   Uma lista vertical com os seguintes itens: "Corte de Grama", "Poda de Árvores", "Adubação e Controle de Pragas", "Design de Jardins".
    -   Remover os marcadores padrão (bolinhas/números) da lista.
    -   Adicionar um pequeno ícone de folha (ex: emoji 🌱 ou caractere Unicode U+1F331) antes de cada item da lista.
    -   Quando o cursor do mouse passar sobre um item da lista, o fundo desse item deve mudar suavemente para uma cor verde clara (sugestão: `#90EE90`).
    -   Deve haver um espaçamento vertical ligeiramente maior entre os itens da lista.
-   **Tarefa Técnica:** Utilizar lista não ordenada (`<ul>`, `<li>`). Em CSS, remover marcadores (`list-style: none;`), adicionar ícone via pseudo-elemento `::before` com a propriedade `content`, aplicar efeito de `background-color` no estado `:hover` e ajustar `margin` ou `padding` nos itens `<li>` para espaçamento. Introduzir `transition` para a suavidade da mudança de cor.

**Questão 4: Formulário de Contato Básico com Validação**

-   **Objetivo:** Implementar um formulário HTML funcional para coleta de dados de contato.
-   **Cenário:** Uma ONG ("Mão Amiga") precisa de um meio para que visitantes do site possam enviar mensagens.
-   **Requisitos do Solicitante:**
    -   O formulário deve solicitar: Nome Completo (campo de texto), E-mail (campo específico para email), Assunto (campo de texto) e Mensagem (área de texto maior).
    -   Cada campo deve ter uma etiqueta clara ("Nome Completo:", "E-mail:", etc.) posicionada logo acima dele.
    -   Os campos "Nome Completo" e "E-mail" são obrigatórios; o usuário não pode enviar o formulário sem preenchê-los.
    -   Deve haver um botão no final com o texto "Enviar Mensagem".
    -   O layout deve ser limpo, com cada par de etiqueta/campo disposto verticalmente, um abaixo do outro, e alinhados à esquerda.
-   **Tarefa Técnica:** Utilizar a tag `<form>` e os elementos `<label>`, `<input type="text">`, `<input type="email">`, `<textarea>` e `<button type="submit">`. Associar labels aos inputs usando o atributo `for`. Implementar validação básica do lado do cliente usando o atributo `required` do HTML5. Utilizar CSS para layout (ex: `display: block` ou Flexbox/Grid para alinhamento vertical) e espaçamento (`margin-bottom`).

**Questão 5: Estrutura Semântica de Blog Post**

-   **Objetivo:** Definir a estrutura HTML semântica e o estilo básico para um artigo de blog.
-   **Cenário:** Um blogueiro de viagens ("Blog Viajante") precisa de um template padrão para seus posts.
-   **Requisitos do Solicitante:**
    -   **Cabeçalho da Página:** Conter o título do blog "Blog Viajante", consistentemente no topo.
    -   **Conteúdo Principal:**
        -   O título específico do post (ex: "Minha Aventura na Patagônia") deve ser o elemento mais proeminente nesta seção.
        -   Abaixo do título, a data de publicação (ex: "Publicado em 20 de Maio de 2024").
        -   O corpo do texto do artigo, contendo múltiplos parágrafos e, opcionalmente, subtítulos para dividir o conteúdo.
    -   **Rodapé da Página:** Exibir uma nota de direitos autorais (ex: "© 2024 Blog Viajante"), de forma discreta no final da página.
    -   Deve haver uma clara separação visual (espaçamento) entre o cabeçalho, o conteúdo principal do artigo e o rodapé.
-   **Tarefa Técnica:** Empregar tags semânticas do HTML5: `<header>`, `<nav>` (se aplicável no header), `<main>`, `<article>`, `<h1>`, `<h2>`, `<p>`, `<time>`, `<footer>`. Utilizar CSS para definir margens e/ou preenchimentos (`margin`, `padding`) para criar a separação visual desejada e estilizar a tipografia básica.

**Questão 6: Galeria de Imagens Responsiva (Flexbox/Grid)**

-   **Objetivo:** Criar uma galeria de imagens que se ajuste a diferentes tamanhos de tela.
-   **Cenário:** Um restaurante ("Sabor Divino") deseja exibir fotos de seus pratos principais em uma grade flexível.
-   **Requisitos do Solicitante:**
    -   Exibir 3 imagens (usar placeholders ou imagens genéricas de comida).
    -   Abaixo de cada imagem, uma legenda curta (ex: "Prato Principal 1", "Sobremesa Especial", "Entrada da Casa").
    -   **Layout Desktop:** As 3 imagens (com suas legendas) devem ser exibidas lado a lado, em uma única linha, com espaçamento igual entre elas.
    -   **Layout Mobile:** Em telas menores (como de smartphones), as 3 imagens devem se empilhar verticalmente, uma abaixo da outra, centralizadas.
    -   As imagens devem ter uma altura consistente ou serem cortadas de forma a manter o alinhamento visual na visualização desktop.
-   **Tarefa Técnica:** Utilizar elementos `<figure>` e `<figcaption>` para cada item da galeria. Empregar CSS Flexbox (`display: flex`, `flex-wrap: wrap`, `justify-content: space-around` ou `center`, `gap`) ou CSS Grid Layout (`display: grid`, `grid-template-columns`, `gap`) para controlar o posicionamento. Utilizar Media Queries (`@media`) para alterar o layout (ex: mudar `flex-direction` para `column` ou `grid-template-columns` para `1fr`) em telas menores. Controlar o tamanho/aspecto das imagens (`height`, `object-fit`).

**Questão 7: Layout de Duas Colunas Responsivo**

-   **Objetivo:** Criar uma página com um layout principal de duas colunas que se adapta a telas menores.
-   **Cenário:** Uma página de produto simples que precisa mostrar uma imagem e a descrição lado a lado no desktop, mas empilhados no mobile.
-   **Requisitos do Solicitante:**
    -   A página deve ter uma área principal dividida em duas colunas quando vista em telas largas (computadores).
    -   **Coluna Esquerda (Desktop):** Exibir uma imagem grande do produto (placeholder).
    -   **Coluna Direita (Desktop):** Conter o nome do produto (título), uma descrição detalhada (parágrafos) e um botão "Comprar Agora".
    -   **Layout Mobile:** Em telas estreitas, a imagem deve aparecer primeiro, ocupando a largura total. Abaixo da imagem, o nome, a descrição e o botão devem seguir, também ocupando a largura disponível e centralizados ou alinhados à esquerda.
    -   Deve haver um espaçamento adequado entre as colunas no desktop e entre os elementos empilhados no mobile.
-   **Tarefa Técnica:** Estruturar o HTML com um container principal e elementos para cada coluna/seção. Utilizar CSS Flexbox ou Grid para criar o layout de duas colunas (ex: `grid-template-columns: 1fr 1fr;` ou `display: flex;`). Aplicar Media Queries para mudar o layout para uma única coluna em telas menores (ex: `grid-template-columns: 1fr;` ou `flex-direction: column;`) e ajustar larguras (`width: 100%`) e espaçamentos (`gap`, `margin`).

**Questão 8: Efeitos Visuais Sutis com Transições CSS**

-   **Objetivo:** Aplicar efeitos de interação suaves a elementos clicáveis.
-   **Cenário:** Melhorar a experiência do usuário em botões ou links de uma página existente (pode-se usar o botão da Questão 4 ou 7 como base).
-   **Requisitos do Solicitante:**
    -   Selecionar um botão ou link na página.
    -   Quando o cursor do mouse passar sobre este elemento (hover):
        -   A cor de fundo deve mudar suavemente para uma tonalidade diferente (ex: de azul para azul escuro).
        -   O elemento deve aumentar ligeiramente de tamanho (ex: escalar para 105% do original) de forma suave.
    -   Quando o cursor sair do elemento, ele deve retornar ao estado original também de forma suave.
    -   O efeito deve ser rápido, mas perceptível (duração da transição em torno de 0.3 segundos).
-   **Tarefa Técnica:** Aplicar a propriedade `transition` do CSS ao elemento base, especificando as propriedades a serem animadas (`background-color`, `transform`) e a duração (`transition-duration`). Definir os estilos desejados no estado `:hover` (a nova `background-color` e `transform: scale(1.05)`).

**Questão 9: Componente "Card" Reutilizável com Sombra e Cantos Arredondados**

-   **Objetivo:** Desenvolver um componente de "card" estilizado que possa ser reutilizado para exibir diferentes conteúdos.
-   **Cenário:** Uma loja online ("Artesanato Criativo") quer exibir vários produtos ou destaques usando um formato visual consistente de "cartão".
-   **Requisitos do Solicitante:**
    -   Criar o design de um "card" individual. Este card deve conter espaço para: uma imagem no topo, um título, um breve texto descritivo e um botão/link na parte inferior.
    -   O card deve ter cantos levemente arredondados.
    -   Deve haver uma sombra sutil projetada atrás do card, dando uma impressão de elevação.
    -   O conteúdo dentro do card deve ter um espaçamento interno (padding) das bordas.
    -   Demonstrar o uso deste card criando 2 ou 3 instâncias dele na página, lado a lado em telas maiores e empilhados em telas menores (similar à Questão 6, mas focando no estilo do card).
-   **Tarefa Técnica:** Criar uma classe CSS (ex: `.card`) para o container do card. Aplicar `border-radius` para os cantos, `box-shadow` para a sombra e `padding` para o espaçamento interno. Estruturar o HTML interno do card (ex: `<img>`, `<h2>`, `<p>`, `<button>`). Utilizar Flexbox ou Grid e Media Queries para o layout geral da página que contém múltiplos cards.

**Questão 10: Menu de Navegação Fixo no Topo com Indicador de Seção Ativa**

-   **Objetivo:** Implementar um menu de navegação persistente no topo da página que indique visualmente a seção atual.
-   **Cenário:** Uma agência de design ("INOVA") necessita de um menu principal que permaneça visível durante a rolagem da página e destaque o link da seção atual.
-   **Requisitos do Solicitante:**
    -   Um menu de navegação horizontal deve ser posicionado fixamente no topo da janela do navegador.
    -   O menu deve conter links para seções da página (ex: 'Home', 'Serviços', 'Portfólio', 'Contato').
    -   Mesmo quando o usuário rolar a página para baixo, o menu deve permanecer visível no topo.
    -   O item de menu correspondente à seção que está atualmente visível (ou que foi clicada) deve ter uma aparência diferente dos outros itens (ex: texto em negrito, cor de fundo diferente ou uma linha abaixo). Para este exercício, pode-se simular a seção ativa adicionando manualmente uma classe específica a um dos links no HTML.
    -   A página deve conter conteúdo de exemplo suficiente abaixo do menu para tornar a rolagem necessária e testar a fixação.
-   **Tarefa Técnica:** Utilizar `<header>` e `<nav>` para o menu. Aplicar CSS `position: sticky; top: 0;` ou `position: fixed; top: 0; width: 100%;` ao container do menu (considerar implicações de layout com `fixed`). Adicionar `z-index` se necessário. Definir uma classe CSS (ex: `.active-link`) e estilizá-la para destacar o item ativo. Aplicar manualmente esta classe a um dos `<a>` tags do menu no HTML. Adicionar conteúdo de preenchimento (`<section>` com `id`s correspondentes aos links e bastante texto `Lorem Ipsum`) para habilitar a rolagem.