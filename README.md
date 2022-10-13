# Search Movies

- Utilizar algum framework CSS (Bootstrap, Materialize, Foundation, Material UI) ou algum pré-processador de CSS (SASS, LESS, Stylus);
- Utilizar algum framework/lib JS (Angular, React, Vue, NextJS, etc.);
- Utilização opcional de algum gerenciador de estado (Ex: Redux);
- Layout livre. Faça com que sua página tenha uma ótima experiência para o usuário, independente do dispositivo que ele esteja usando;

# Funcionalidades
## Tela inicial
- Formulário de busca posicionado no meio da tela com campo de texto com placeholder “Procure seu Filme” e um botão “Buscar”;

- Após o usuário preencher o campo (não pode ser vazio) e clicar no botão “Buscar” (ou pressionar o “Enter”), esse formulário 
deve ser movido para o topo da tela usando css animate chamando a tela de listagem enviando o parâmetro inserido na caixa de texto;

## Tela Listagem
- Deve ser feito uma busca na url http://omdbapi.com/ ?s={nome_do_filme} (documentação da api: http://www.omdbapi.com/) 
e o retorno dessa chamada será uma lista de filmes com os campos (Title, Year, Type, imdbID, Poster);

- A partir dessa chamada devem ser listados esses filmes mostrando apenas o poster do filme. Ao passar o mouse em cima do poster deve 
ser carregado uma “tooltip”, com as informações restantesEssa “tooltip”, deve conter também um botão “+ info” que levará o usuário para
uma tela de detalhes do filme;

- Essa tela deve mostrar apenas os 6 primeiros resultados e deve possuir paginação infinita mostrando de 6 em 6 itens;
Tela Detalhes:• A partir do resultado retornado na chamada anterior, deve ser feita uma chamada para http://omdbapi.com/?i={imbd_id} 
que retorna os campos (Title, Year, Rated, Released, Genre, Director, Writer, Actors, Plot, Language, Country, Awards, Poster, Metascore, 
imdbRating, imdbVotes, imdbiD, Type).• A partir desse retorno deve-se montar uma tela onde apareçam todas essas informações. 
Essa tela deve ter um botão para voltar para resultados da busca, que manda o usuário de volta para o topo dos resultados da busca
