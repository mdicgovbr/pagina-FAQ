# FAQ SISCOSERV
Este repositório apresenta um [site estático](https://mdicgovbr.github.io/pagina-FAQ/) para perguntas e respostas(FAQ) do SISCOSREV, que é um sistema informatizado para acompanhamento e aferição das políticas públicas relacionadas a serviços. Sendo assim, pessoas domiciliadas no Brasil que realizem comercialização com pessoas domiciliadas no exterior podem ter que registrar seus serviços dependendo, por exemplo, do custo do serviço em questão. 

# Ferramentas Utilizadas
Para o desenvolvimentodo do site, foi convertido as páginas pdf já existentes no [FAQ do SISCOSREV](http://www.mdic.gov.br/comercio-servicos/a-secretaria-de-comercio-e-servicos-scs-15/estatisticas-6) para arquivos **Markdown**, que você pode encontrar facilmente analisando se o documento termina com ".md" disponíveis aqui no github. A próxima etapa é entender como poderíamos transformar esses arquivos markdown em um site, a resposta é simples: um gerador de site para conteúdos estáticos, no caso o **Jekyll**. Agora, já temos o conteúdo e a ferramenta que trabalha por trás do GitHub para gerar o site, só precisamos então configurar nosso GithubPages para que possa ocorrer a publicação das informações. Na configuração basta escolher um  

## Etapa 1 - Construção do Markdown
Converter os PDFs para markdown usando uma hashtag '#' para títulos e a tag "blockquote" para citações. Para entender melhor sua sintaxe  acesse a [documentação markdown](https://www.markdownguide.org/basic-syntax) .
  
## Etapa 2 - Entendendo o Jekyll
Jekyll é uma biblioteca escrita em ruby que recebe como entradas arquivos markdown (.md) e gera como saída arquivos estáticos **html**. É possível incluir os conteúdos html gerados em algum template pré definido. Basta que o header.html e o footer.html estejam em uma pasta chamada **\_includes**. Ao executar o Jekyll os arquivos de saída serão armazenados em uma pasta chamada **\_site**. As explicações fornecidas sobre o Jekyll são a título de curiosidade, tendo em vista que publicação com o GitHub Pages o Jekyll é usado no background do Git, automatizando esta atividade. Para mais curiosidades do Jekyll visite os seguintes sites:  
- https://jekyllrb.com/
- https://jekyllrb.com/docs/  
- https://jekyllrb.com/docs/structure/  
  
Também é possível instalar o Jekyll com container docker:  
- https://hub.docker.com/r/jekyll/jekyll/  
Para visualizar um exemplo, olhe a página: https://github.com/mdicgovbr/pagina-estatisticas a qual contem um arquivo docker-compose com o container do Jekyll.
  
## Etapa 3 - Configuração do GithubPages
**Passo 1:** Para configurar o GithubPages vá em configurações:
![Imgur](https://i.imgur.com/lbjgSAM.png)

**Passo 2:** Acesse o quinto subtítulo chamado "GithubPages": 
![Imgur](https://i.imgur.com/L8ouoyc.png)

**Passo 3:** [Nesta seção escolha seu tema](https://github.com/mdicgovbr/pagina-FAQ/settings/pages/themes?utf8=%E2%9C%93&select=slate&source=master) ou apenas clique em: Change theme. Para escolher tema clique em cima do seu tema favorito e depois clique em "Select Theme". Em seguida você receberá a menssagem "Jekyll theme set to 'Slate'." em um campo azul superior da tela. Além disso, será adicionado um arquivo .yml, o qual vai setar o tema escolhido.
