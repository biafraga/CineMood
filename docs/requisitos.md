# Requisitos Funcionais (RF)

## O que o sistema deve fazer

**RF para o Usuário Visitante (Interface Pública)**
- **RF01**: O sistema deve exibir uma página inicial interativa, apresentando ao
usuário uma seleção de "moods" (estados de espírito) clicáveis.
- **RF02**: Ao clicar em um mood, o sistema deve redirecionar o usuário para uma
página que lista todos os filmes associados àquele mood.
- **RF03**: O sistema deve permitir que o usuário clique em um pôster de filme para
acessar uma página de detalhes.
- **RF04**: A página de detalhes do filme deve exibir informações completas, como:
título, pôster em destaque, sinopse, ano de lançamento, diretor, e a lista de
moods aos quais o filme pertence.
- **RF05**: O sistema deve possuir uma funcionalidade "Me Surpreenda!" que, ao
ser acionada, exibe a página de detalhes de um filme aleatório de todo o
catálogo.

**RF para o Administrador (Área Administrativa)**
- **RF06**: O sistema deve fornecer uma página de login segura, exclusiva para o
administrador.
- **RF07**: O sistema deve validar as credenciais do administrador e conceder
acesso a um painel de controle (dashboard) após o login bem-sucedido.
- **RF08**: No painel de controle, o administrador deve poder visualizar atalhos
para as principais operações de gerenciamento.
- **RF09**: O administrador deve poder realizar operações de CRUD (Criar, Ler,
Atualizar, Deletar) para os Filmes no catálogo.
- **RF10**: O formulário de criação/edição de um filme deve permitir ao
administrador inserir dados como título, sinopse, ano, diretor, URL do pôster e
uma frase de efeito.
- **RF11**: O formulário de criação/edição de um filme deve permitir ao
administrador associar um ou mais moods existentes ao filme.
- **RF12**: O administrador deve poder realizar operações de CRUD (Criar, Ler,
Atualizar, Deletar) para os Moods do sistema.

# Requisitos Não-Funcionais (RNF)
## Como o sistema deve ser, definindo suas qualidades, restrições e padrões de operação.

- **RNF01 - Usabilidade**: A interface do usuário deve ser intuitiva, limpa e
visualmente agradável, garantindo que um novo usuário consiga navegar e
descobrir filmes sem a necessidade de um tutorial.
- **RNF02 - Desempenho**: As páginas públicas do site devem ter um tempo de
carregamento completo inferior a 3 segundos em uma conexão de internet
banda larga padrão. As respostas da API não devem exceder 500ms.
- **RNF03 - Responsividade**: A aplicação deve ser totalmente responsiva,
adaptando-se e proporcionando uma boa experiência de uso em diferentes
tamanhos de tela (desktops, tablets e smartphones).
- **RNF04 - Compatibilidade**: O site deve ser compatível com as duas últimas
versões dos principais navegadores do mercado (Google Chrome, Mozilla
Firefox, Safari e Microsoft Edge).
- **RNF05 - Segurança**: A senha do administrador deve ser armazenada no
banco de dados utilizando um algoritmo de hash seguro. A área administrativa
só deve ser acessível por usuários autenticados.
- **RNF06 - Manutenibilidade**: O código-fonte (frontend e backend) deve ser bem
estruturado, comentado e seguir as melhores práticas de desenvolvimento para
facilitar futuras manutenções e atualizações.
- **RNF07 - Disponibilidade**: A aplicação deve visar uma disponibilidade de 99%
do tempo, excluindo-se janelas de manutenção planejadas.
