
# Análise acessibilidade mobile 

## Princípio 1: Perceptível

### 1.1 Tamanho de tela pequeno
Deve-se levar em consideração o tamanho da tela dos dispositivos móveis, o conteúdo deve ser projetado pensando no limite de espaço e na ordem que será apresentado as informações.

Segue abaixo algumas dicas recomendadas pela W3C para aproveitar ao máximo as telas pequenas:
- **Resumir o conteúdo:** focar cenários importantes para uso do celular, eliminar imagens desnecessárias ou informações secundárias que não impactam diretamente o objetivo principal;
- **Tamanho do texto e de elementos interativos:** idealmente o tamanho dos elementos interativos deve ser de no mínimo 44x44 pixeis porém, pode ser menor (até 24x24 pixéis) contanto que respeite alguns critérios de posicionamento e espaçamento da WCAG;
- **Varrimento horizontal:** evite apresentar mais de um conteúdo na linha horizontal, além de ser pouco espaço pode induzir a erros quando elementos estão muito próximos. Como por exemplo, um formulário deve ter seus campos apresentados verticalmente;
### 1.2 Zoom/Ampliação
Existem funcionalidades no sistema nativo dos celulares que permitem o usuário controlar o tamanho do conteúdo:
- Tamanho do texto;
- Tamanhos dos elementos da tela;
- Lente de ampliação (pelo dedo).
### 1.3 Contraste
Avaliar o contraste torna-se indispensável principalmente quando falamos de dispositivos móveis, pois diferente dos desktops eles podem ser utilizados em diferentes cenários e locais. 

As recomendações da WCAG para contraste são as seguintes:
- **1.4.3 Contraste (Mínimo) (Nível AA)** que requer um contraste de pelo menos 4,5:1 (ou 3:1 para texto em grande escala) e,
- **1.4.6 Contraste (Aprimorado) (Nível AAA)** que requer um contraste de pelo menos 7:1 (ou 4,5:1 para texto em grande escala).

## Princípio 2: Operável
### 2.1 Permitir diferentes entradas e dispositivos
Essa regra se aplica também aos dispositivos móveis. Hoje é possível utilizar dispositivos de teclado permitindo os usuários navegarem pelo conteúdo utilizando teclados externos (via bluetooh ou USB por exemplo).

Segue abaixo algumas recomendações da WCAG:
- [2.1.1 Teclado (Nível A)](https://www.w3.org/WAI/WCAG22/Understanding/keyboard.html)
- [2.1.2 Sem armadilha de teclado (Nível A)](https://www.w3.org/WAI/WCAG22/Understanding/no-keyboard-trap.html)
- [2.4.3 Ordem de Foco (Nível A)](https://www.w3.org/WAI/WCAG22/Understanding/focus-order.html)
- [2.4.7 Foco Visível (Nível AA)](https://www.w3.org/WAI/WCAG22/Understanding/focus-visible.html)


### 2.2 Tamanho dos elementos interativos
É necessário garantir que o tamanho dos elementos seja o suficiente para permitir a sua escolha. dealmente o tamanho dos elementos interativos deve ser de no mínimo 44x44 pixeis porém, pode ser menor (até 24x24 pixéis) contanto que respeite alguns critérios de posicionamento e espaçamento da WCAG;

### 2.3 Instruções de gestos sensíveis ao toque

Os dispositivos móveis fornecem recursos para serem operdos principalmente por meio de gestos ao toque que podem ser algo simples como um swipe (movimento da esquerda para direita ou vice versa) ou mais complexos, envolvendo vários dedos, vários toques e formas desenhadas.


Segue abaixo algumas boas práticas recomendadas:
- **Gestos simples:** sempre que possível utilize gestos simples de controle de ação. Gestos muito complexos além de causar dúvidas podem ser mais dificeis de executar por pessoas com mobilidade reduzida;
- **Fornecer instruções para gestos mais complexos:** se mesmo assim utilizar ações mais comlexas, tente exibir uma instrução de como executar tal ação;
- **Eventos mouseup e touchend:** utilizar esses eventos ajuda a evitar ações não intencionais, movendo para fora de um botão por exemplo. 


### 2.4 Gestos em diferentes entradas e dispositivos
Além de gestos, os dispositivos móveis permitem que controles possam ser acionados por manipulação física do objeto (inclinação ou agitação). Nesses casos, é necessário garantir que quando houver esses recursos seja disponível também outras opções alternativas pelo mouse e teclado.

### 2.5 Botões (ou qualquer elemento interativo) de fácil acesso

É necessário garantir que os elementos interativos sejam facilmente selecionados independente de sua posição.


## Princípio 3: Compreensível
### 3.1 Permitir mudança de orientação (vertical e horizontal)
É necessário garantir que o sistema/aplicação suportem ambas as visões. Essas mudanças de orientação devem ser expostas programaticamente para que o leitor de ecrã informe e detecte a mudança.

### 3.2 Layout deve ser consistente
Tanto na WEB como mobile é imprescindível garantir que os componentes que aparecem repetivos em outras páginas se comportem da mesma forma inclusive seu posicionamento.

Os critérios de sucesso das WCAG 2.0 que mais estão relacionados com a questão da consistência são:
- [3.2.3 Navegação Consistente (Nível AA)](https://www.w3.org/WAI/WCAG22/Understanding/consistent-navigation.html)
- [3.2.4 Identificação Consistente (Nível AA)](https://www.w3.org/WAI/WCAG22/Understanding/consistent-identification.html)

### 3.3 Posicionar elementos importantes antes da primeira rolagem
Isso permite que pessoas com baixa visão ou deficiência cognitiva encontrem as informações mais facilmente sem a necessidade de procurar por um varrimento no conteúdo.

### 3.4 Agrupar elementos que executam a mesma ação
Links, botões ou quaisquer elemento interativo que seja composto por mais de um elemento, como por exemplo, um link que possui texto e o seu ícone, devem estar agrupados. Isso faz com que a área clicável seja maior e evita redundâncias durante a leitura com o leitor de ecrã.

### 3.5 Elementos interativos devem parecer ser clicáveis
Tanto na WEB como em mobile, elementos devem estar visualmente destacadaos como algo que seja clicável.

### 3.6 Instruções 
As instruções devem ser fornecidas principalmente quando há comandos específicos de uso. Para ser eficiente  deve ser facilmente detectáveis ​​e acessíveis. As instruções também devem estar disponíveis sempre que o usuário precisar delas, não apenas na primeira utilização, embora na primeira utilização elas possam ficar mais aparentes através de destaque ou algum outro mecanismo.

Os critérios de sucesso das WCAG 2.0 que mais estão relacionados são:
- [3.3.2 Etiquetas ou Instruções (Nível AA)](https://www.w3.org/WAI/WCAG22/Understanding/labels-or-instructions.html)
- [3.3.5 Ajuda (Nível AAA)](https://www.w3.org/WAI/WCAG22/Understanding/help.html)


## Princípio 4: Robusto
### 4.1 Teclado virtual deve ser configurado de acordo com o tipo de entrada do campo
Tal configuração pode ser feita no celular como dispositivos externos.

### 4.2 Evite entrada de dados manuais (digitos)
Garantir que os campos necessários de preenchimento possma ser fornecido por outras entradas de campos, ao invés de campo de digitação se possível substituir com campos de seleção, caixas de seleção, radio buttons etc...

### 4.3 Utilize recursos disponíveis da plataforma
Os dispositivos móveis oferecem recursos que ajudam a garantir a acessibilidade, como legendas, aumento da fonte e elementos interativos porém, isso varia de dispositivo e versão do sistema operacional. Garantir que ao utilizar o aumento de fonte o texto não fique compacto (...) ou seja necessário um scroll horizontal por exemplo. 

