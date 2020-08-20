# Anotações curso de Laravel 
***
### 1. Laravel Developer(Apresentação do curso)
1. Laravel Developer
2. Convite Especial Telegram
3. Framework vs CMS
4. Ecossistema Laravel
5. Versões do Framework
6. [UPDATE] Novo sistema de versões
7. Abstração da aplicação
8. Documentação
### 2. Preparando ambiente
1. Preparando ambiente
2. Instalação Global do PHP 
3. Instalação Global do Composer
4. Instalação do NodeJS
	- *No (Laravel Mix) é usado node para trabalhar com webpack* [Laravel Mix](https://laravel.com/docs/7.x/mix) - [iMasters](https://imasters.com.br/css/gerenciando-assets-com-laravel-mix)
5. Instalação do Laravel via terminal
6. Arquitetura de Pastas
7. Configurando Projeto
### 3. Primeiro contato
1. Primeiro Contato
2. Definindo Rota
	- 1 Cadastro de um Imóvel
	- 2 Single e Listagem
3. 1Adicionando URL amigável
4. 1Edição do Imóvel
5. 1Remoção de registros
6. Adicionando camada Model
7. Método create e save
8. Estruturando view master
9. 1Formatando páginas

### 4.  Dominando rotas
1. Trabalhando com requisições
2. Projeto e ponto de partida
3. 1Entendendo a Verbalização
4. 2Verbos de Atualização
5. 1Verbo de Deleção e Options
6. 1Rotas Resource
7. 2Tipos de Chamada
8. 1Tratamento de Parâmetros
9. 1Inspecionamento
10. Agrupamento
11. 1Route Caching

### 5.  Migrations, Seeders e Factory
1. Versionamento de banco de dados
2. Criando a primeira migration
3. 1[SCHEMA] Modelando uma tabela completa
4. 1[SCHEMA] Relacionamentos
5. 1[DATA] Inserindo usuário de Administrador
6. 1Controle de Migrações
7. [SEEDER] Criando a primeira Seeder
8. 1[FACTORY] Gerando informações com Faker

### 6.  Eloquent ORM
1. Mapeando objetos relacionais
1. Parametrização do Projeto
1. Parametrização do modelo
1. 1Obtenção de registros e coleções
1. 2Inserção de modelos
1. 2Atualização de modelos
1. 2Exclusão de modelos
1. Soft Deletes
### 7.  Recursos avançados de modelo
1. Modelos inteligentes
1. Parametrização do projeto
1. 1Relacionamento UM-PARA-UM
1. 2Gestão de Relacionamentos
1. 1Relacionamento UM-PARA-N
1. 1Relacionamento através De
1. Relacionamento N-PARA-N
1. 1Gestão de Tabela Pivo
1. 1Relacionamento Polimorfico
1. 1Definindo Escopos
1. Accessor e Mutator
1. Filtro de Collections
1. Serialização de Modelo
### 8.  Query Builder e Paginação
1. Construtor de consultas
1. Parametrização do Projeto
1. Construtor de Query
1. 1Consulta Bruta (Raw)
1. 1Compreendendo o Chunk
1. Cláusula WHERE com ParseString
1. 1Trabalhando com JOIN SQL
1. 1Cadastro, Atualização e Deleção
1. Paginando resultados
### 9.  Serviços Essenciais
1. Gerenciamento de serviços
1. Geração e Controle de Log
1. 2Driver e Sessão I:O
1. 2Armazenando sessão com Redis
1. 1Enviando E-mail
1. 3Fila de Processamento e Jobs
1. 1Gestão de arquivo e diretórios
1. 2Upload através do formulário
1. 2Definição de Middleware
### 10. Visão Orquestrada
1. Visão Orquestrada
1. Desmistificando o Blade
1. 1Condições no Blade
1. 1Laços de Repetição
1. 1Compondo Página Master
1. 2Lapidando Página Master
1. 1Criando um componente
1. 1NPM e Laravel Mix
1. 2Minificação e Versionamento
### 11. Validação de Requisições
1. Recursos e Validações
1. Construindo Aplicação
1. 1Validando com Request
1. 2Validando com Injeção de Dependência
1. Validando com Facade
### 12. Projeto: Website Desafio
1. Aplicando Conhecimento
1. Criando um cenário
1. 1Fatiando o Layout e Controlando Rotas
1. 2SEO com componente Externo [FSPHP]
1. 2Parametrizando Laravel Mix pt1
1. 1Parametrizando o Laravel Mix pt2
1. 1Personalizando o Tema
1. Instalando o Template e Helper
1. 1Desenvolvendo Recursos
1. 1Aplicando Recursos
1. 2Alimentando Blog e Single
1. 1Disparando E-mail
1. 1Um desafio para você
### 13. Projeto: Sistema Imobiliário
1. Seu projeto prático começa agora
1. Configuração do Projeto
1. 1Compreendendo a Aplicação e Modelagem
1. 3Adequando Layout ao Laravel
1. 1Configurando Laravel Mix
1. 1Laravel Mix [Dashboard]
1. 1Login com AJAX
1. 1Tratando requisição de Login
1. 2Ação de Logout
1. Helper menu ativo
1. Refatorando Login e Últimos Ajustes
### 14. Desenvolvendo Recursos
1. Desenvolvendo solução do projeto
1. Desenvolvendo Recursos [Usuário]
1. 1 Cadastro de Usuário
1. 1Validação dos campos
1. 3Tratamento de Dados
1. 2Persistência dos Dados
1. 2Listagem e Formulário de Edição
1. 2Tratamento de Dados [Output]
1. 2Upload de Mídia do Usuário
1. 2Gatilhos JS e Refatoração
1. 3Desenvolvendo Recursos [Company]
1. 3Tratamento de Dados
1. 3Gatilho Cliente - Empresa
1. 1Desenvolvendo Recursos [Imóvel]
1. 1Migration da entidade de imóveis
1. 1Fix Tinymce e Persistência
1. 2Tratamento das informações
1. 3Persistência de Proprietário e views
1. 2Desenvolvendo Recursos [Imagens]
1. 2Alimentando Imagens e disparando gatilho
1. 2Gestão de mídias
1. 2Desenvolvendo Recursos [Contrato]
1. 2Gatilhos Ajax
1. 3Gatilhos Ajax pt2
1. 1Gatilhos Ajax pt3
1. 2Persistência das Informações Ajax
1. 3Tratamento das informações do Contrato
1. 3Listagem e Termos do Contrato
1. 3Fluxo dos Imóveis
1. 2Alimentando Dashboard
1. 1Refatoração da Aplicação
### 15. Projeto: Website Imobiliário
1. Bem vindo ao Site Imobiliário
1. Overview do Tema
1. 1Rota, Controlador e Visão
1. 1Parametrização do Laravel Mix
1. 2Ajustes do Tema
1. 1Aprimorando Imóveis
1. 1[Home] Dobra Venda/Locação
1. 2[Interna] Elementos Dinâmicos
1. 1[Interna] Google Maps
1. 1[Filtro] Organização do Componente
1. 3[Filtro] Gatilhos Javascript
1. 1[Filtro] Aplicando Regra
1. 2[Filtro] Aplicando Regra pt2
1. 3[Filtro] Listando Registros
1. 1[Filtro] Reutilizando Motor JS
1. 1[Alugar/Comprar] Desenvolvendo Listagem
1. 2[Home] Desenvolvendo Experiência
1. 2SEO/SEM Compartilhando informação certa
1. 3Ajustes Essenciais
### 16. Projeto: API REST e JWT
1. Criando API com JWT
1. Conhecendo Estrutura
1. 1Instalando Componente JWT
1. 2Protegendo Rotas de API
### 17. Laradev em Produção
1. Colocando o sistema em ambiente de Produção
1. Deploy em Ambiente Compartilhado
1. 3Testes Ambiente Compartilhado
1. 1Deploy em Ambiente Privado
1. 2Testes Ambiente Privado
### 18. BugFix e Atualizações
1. BugFix e Atualizações
1. Bug fix projeto final
1. 9Fix Finalidade do Contrato
1. 2Atualização pra 5.8
1. Atualização para 6.x




(\d) min.(\s)*$\nNunca Acessou.*(\s)*$\nNão Abriu(\s)*$\n
(\d) min.(\s)*$\n(\d){2}/(\d){2}/(\d){4}.*(\s)*$\nNão Abriu(\s)*$\n
