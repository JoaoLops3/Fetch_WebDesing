# Lista de Animais

Este é um projeto simples de uma página HTML que consome uma API para listar e cadastrar animais. Utiliza HTML, JavaScript e a biblioteca Axios para realizar requisições HTTP.

## Funcionalidades

- **Listar Animais**: Ao carregar a página, é feita uma requisição GET para obter a lista de animais cadastrados, que são exibidos em uma lista.
- **Cadastrar Animal**: O usuário pode cadastrar um novo animal ao clicar no botão "Cadastrar Animal". A aplicação envia uma requisição POST com informações de um animal pré-definido ("Tisto", 6 anos, raça "gato") para a API e, em seguida, atualiza a lista.

## Tecnologias Utilizadas

- **HTML**: Estrutura básica da página.
- **JavaScript**: Lógica para consumir a API e manipular o DOM.
- **Axios**: Biblioteca para realizar requisições HTTP.
- **MockAPI**: API externa utilizada para armazenar dados fictícios de animais.

## Como Usar

1. **Pré-requisitos**: Nenhum pré-requisito específico. A aplicação utiliza a biblioteca Axios via CDN, então uma conexão com a internet é necessária para seu funcionamento.

2. **Execução**:
   - Abra o arquivo `index.html` em qualquer navegador.
   - A lista de animais cadastrados será carregada automaticamente.
   - Clique no botão "Cadastrar Animal" para adicionar um novo animal à lista. O animal cadastrado é "Tisto", com idade 6 e raça "gato".

3. **API Utilizada**: 
   - A aplicação interage com a API `https://6724d3eac39fedae05b2e551.mockapi.io/usuario/Animal` para obter e cadastrar dados.

## Estrutura do Código

- **HTML**: Define a estrutura da página com um título, lista de animais e botão para cadastrar.
- **JavaScript**:
  - `carregarAnimais`: Realiza uma requisição GET para obter a lista de animais e exibi-la.
  - `cadastrarAnimal`: Realiza uma requisição POST para cadastrar um novo animal na API e atualizar a lista de animais.
  - Eventos:
    - Carrega a lista de animais quando a página é aberta.
    - Cadastra um animal ao clicar no botão.

## Possíveis Melhorias

- Adicionar um formulário para permitir que o usuário insira os dados de um novo animal, em vez de cadastrar dados fixos.
- Implementar validação de dados para evitar erros ao cadastrar um animal.
- Tratar e exibir mensagens de erro no DOM em vez de apenas logá-los no console.

## Exemplo de Uso

Ao abrir a página, a lista de animais é carregada automaticamente:

```plaintext
1 - Rex (2 anos) – cachorro
2 - Tisto (6 anos) – gato
