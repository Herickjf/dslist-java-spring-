# dslist - Java Spring

## Projeto de manipulação e acesso a um BD de Jogos
<p>
  Um projeto simples de preenchimento, manipulação e acesso de informações em um banco de dados H2. Disso obtém-se uma API, que, a partir do método GET "/games" retorna uma versão reduzida de cada um dos jogos do banco de dados.
</p>

<br>
<hr>
<br>

### Como Funciona?

  A interface GameRepository herda de JpaRepository, que disponibiliza o método `findAll()`, usamos esse método para buscar, no banco de dados, uma Lista do tipo `Game` (que, por sua vez, é uma tabela do BD). Esse retorno é convertido numa lista do tipo `GameMinDTO` (um `Data Tranfer Object` de Game, que reduz o objeto a apenas o que se espera dele no Client, a fim de minimizar o tempo de espera). 
<br>
  Assim, ao acessar a rota `localhost:8080/games` com o método `GET`, obtém-se a lista minimizada das informações de cada jogo armazenado no banco de dados.

<br>
<hr>
<br>

## Visualização:

