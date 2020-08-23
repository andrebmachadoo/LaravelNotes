# Anotações curso de Laravel 
***
### 1. Laravel Developer(Apresentação do curso)
1. ~~Laravel Developer~~
2. ~~Convite Especial Telegram~~
3. ~~Framework vs CMS~~
4. [Ecossistema Laravel](https://laravel.com/)
	-	Vapor - Serverless Plataform
	-	**Forge** - Server Management
	-	Envoyer - Zero Downtime Deployment, gerenciamento de deploy
	-	Horizon - Queue Monitoring, Load balance
	-	Nova - Administration Panel
	-	Echo - Realtime Events
	-	**Lumem** - Micro-Framework, muito util para api
	-	Homestead - Pre-Packaged Vagrant Box
	-	Spark - Saas App Scaffolding
	-	Valet - Dev Eviroment for Macs
	-	Mix - Webpack Asset Compilation
	-	Cashier - Subscription Billing Integration
	-	Dusk - Browser Testing and Automation 
	-	**Passport** - Painless OAuth2 Implementation 
	-	Scout - Full-Text-Search 
	-	Socialite-OAuth Autentication
	-	Telescope - Debug Assistant 
	-	**Tinker** - Interactive REPL 
5. ~~Versões do Framework~~
	- *paradigm.major.minor*
6. [UPDATE] Novo sistema de versões
7. Abstração da aplicação
8. [Documentação](https://laravel.com/docs/master)
### 2. Preparando ambiente
1. ~~Preparando ambiente~~
2. ~~Instalação Global do PHP~~
3. [Instalação Global do Composer]( https://getcomposer.org/download/  )
	```shell
		$ composer global require laravel/installer 
	```
	- Variaveis de ambiente 
		- macOS: $HOME/.composer/vendor/bin
		- Windows: %USERPROFILE%\AppData\Roaming\Composer\vendor\bin
4. Instalação do NodeJS
	- *No (Laravel Mix) é usado node para trabalhar com webpack* [Laravel Mix](https://laravel.com/docs/7.x/mix) - [iMasters](https://imasters.com.br/css/gerenciando-assets-com-laravel-mix)
5. Instalação do Laravel ( Criando projeto) via terminal [artisan](https://laravel-docs-pt-br.readthedocs.io/en/5.0/artisan/ )
	- laravel new blog --> Cria um projeto na versão do laravel instalada
	- Composer create-project --prefer-dist laravel/laravel nome_projeto
	- composer create-project laravel/laravel your-project-name 5.8 --> _Cria projeto na Versao desejada_
		- Depois de criado o projeto entra na pasta e executa o comando CLI para subir um servico http via PHP
		- ```Shell    
			$ php artisan serve 
			$ php artisan serve --host=localhost --port=8080	```
6. Arquitetura de Pastas
	- **/apps**  _Os Models são criados nessa pasta mas podem ser organizados numa subpasta_
		-  **/Http/Controller** Camada de controle da aplicação que interage com a view
			- ```Shell
				$ php artisan make:controller NomeDoController	
				```
		-  **/Http/Middleware** Pode ser usado por exemplo como um interceptador entre rota-controller
			- ```Shell
				$ php artisan make:middleware NomeDoMiddleware	
				```
	- **/config**  _Onde o sistema carrega/ configuraçoes da aplicaçao e muitas são setadas no arquivo .env_
	- **/database**  _Onde ficam as migrations(Versionamento do banco) e seeders( Inserção de dados para teste)_
		- ```Shell
			$ php artisan make:migration create_users_table
			$ php artisan make:seeder TableNameTableSeeder
			```
	- **/resourses**  _Arquivos de tradução e views_
	- **/routes**  _web.php(Rotas para web view), api.php(Rotas da api)_
	- **/storage**  _Arquivos externos como uploads, logs, bkps..._
	- **/.env**  _Arquivo de configuracoes do framew..._
7. Configurando Projeto
	- Alterando o namespace da app.
	- ```shell 
		$ php artisan app:name NomeDaAplicação
		```
	- Alterando ***timezone*** em ***/config/app.php***
		```PHP
			'timezone'=>'America/Sao_Paulo'
		```
	- Tradução das mensagens do Laravel [Upinside](https://github.com/andrebmachadoo/laravel-pt-BR)
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
2. Parametrização do Projeto
4. Parametrização do modelo
5. 1Obtenção de registros e coleções
6. 2Inserção de modelos
7. 2Atualização de modelos
8. 2Exclusão de modelos
9. Soft Deletes
### 7.  Recursos avançados de modelo
1. Modelos inteligentes
2. Parametrização do projeto
3. 1Relacionamento UM-PARA-UM
4. 2Gestão de Relacionamentos
5. 1Relacionamento UM-PARA-N
6. 1Relacionamento através De
7. Relacionamento N-PARA-N
8. 1Gestão de Tabela Pivo
9. 1Relacionamento Polimorfico
10. 1Definindo Escopos
11. Accessor e Mutator
12. Filtro de Collections
13. Serialização de Modelo
### 8.  Query Builder e Paginação
1. Construtor de consultas
2. Parametrização do Projeto
3. Construtor de Query
4. 1Consulta Bruta (Raw)
5. 1Compreendendo o Chunk
6. Cláusula WHERE com ParseString
7. 1Trabalhando com JOIN SQL
8. 1Cadastro, Atualização e Deleção
9. Paginando resultados
### 9.  Serviços Essenciais
1. Gerenciamento de serviços
2. Geração e Controle de Log
3. 2Driver e Sessão I:O
4. 2Armazenando sessão com Redis
5. 1Enviando E-mail
6. 3Fila de Processamento e Jobs
7. 1Gestão de arquivo e diretórios
8. 2Upload através do formulário
9. 2Definição de Middleware
### 10. Visão Orquestrada
1. Visão Orquestrada
2. Desmistificando o Blade
3. 1Condições no Blade
4. 1Laços de Repetição
5. 1Compondo Página Master
6. 2Lapidando Página Master
7. 1Criando um componente
8. 1NPM e Laravel Mix
9. 2Minificação e Versionamento
### 11. Validação de Requisições
1. Recursos e Validações
2. Construindo Aplicação
3. 1Validando com Request
4. 2Validando com Injeção de Dependência
5. Validando com Facade
### 12. Projeto: Website Desafio
1. Aplicando Conhecimento
2. Criando um cenário
3. 1Fatiando o Layout e Controlando Rotas
4. 2SEO com componente Externo [FSPHP]
5. 2Parametrizando Laravel Mix pt1
6. 1Parametrizando o Laravel Mix pt2
7. 1Personalizando o Tema
8. Instalando o Template e Helper
9. 1Desenvolvendo Recursos
10. 1Aplicando Recursos
11. 2Alimentando Blog e Single
12. 1Disparando E-mail
13. 1Um desafio para você
### 13. Projeto: Sistema Imobiliário
1. Seu projeto prático começa agora
2. Configuração do Projeto
3. 1Compreendendo a Aplicação e Modelagem
4. 3Adequando Layout ao Laravel
5. 1Configurando Laravel Mix
6. 1Laravel Mix [Dashboard]
7. 1Login com AJAX
8. 1Tratando requisição de Login
9. 2Ação de Logout
10. Helper menu ativo
11. Refatorando Login e Últimos Ajustes
### 14. Desenvolvendo Recursos
1. Desenvolvendo solução do projeto
2. Desenvolvendo Recursos [Usuário]
3. 1 Cadastro de Usuário
4. 1Validação dos campos
5. 3Tratamento de Dados
6. 2Persistência dos Dados
7. 2Listagem e Formulário de Edição
8. 2Tratamento de Dados [Output]
9. 2Upload de Mídia do Usuário
10. 2Gatilhos JS e Refatoração
11. 3Desenvolvendo Recursos [Company]
12. 3Tratamento de Dados
13. 3Gatilho Cliente - Empresa
14. 1Desenvolvendo Recursos [Imóvel]
15. 1Migration da entidade de imóveis
16. 1Fix Tinymce e Persistência
17. 2Tratamento das informações
18. 3Persistência de Proprietário e views
19. 2Desenvolvendo Recursos [Imagens]
20. 2Alimentando Imagens e disparando gatilho
21. 2Gestão de mídias
22. 2Desenvolvendo Recursos [Contrato]
23. 2Gatilhos Ajax
24. 3Gatilhos Ajax pt2
25. 1Gatilhos Ajax pt3
26. 2Persistência das Informações Ajax
27. 3Tratamento das informações do Contrato
28. 3Listagem e Termos do Contrato
29. 3Fluxo dos Imóveis
30. 2Alimentando Dashboard
31. 1Refatoração da Aplicação
### 15. Projeto: Website Imobiliário
1. Bem vindo ao Site Imobiliário
2. Overview do Tema
3. 1Rota, Controlador e Visão
4. 1Parametrização do Laravel Mix
5. 2Ajustes do Tema
6. 1Aprimorando Imóveis
7. 1[Home] Dobra Venda/Locação
8. 2[Interna] Elementos Dinâmicos
9. 1[Interna] Google Maps
10. 1[Filtro] Organização do Componente
11. 3[Filtro] Gatilhos Javascript
12. 1[Filtro] Aplicando Regra
13. 2[Filtro] Aplicando Regra pt2
14. 3[Filtro] Listando Registros
15. 1[Filtro] Reutilizando Motor JS
16. 1[Alugar/Comprar] Desenvolvendo Listagem
17. 2[Home] Desenvolvendo Experiência
18. 2SEO/SEM Compartilhando informação certa
19. 3Ajustes Essenciais
### 16. Projeto: API REST e JWT
1. Criando API com JWT
2. Conhecendo Estrutura
3. 1Instalando Componente JWT
4. 2Protegendo Rotas de API
### 17. Laradev em Produção
1. Colocando o sistema em ambiente de Produção
2. Deploy em Ambiente Compartilhado
3. 3Testes Ambiente Compartilhado
4. 1Deploy em Ambiente Privado
5. 2Testes Ambiente Privado
### 18. BugFix e Atualizações
1. BugFix e Atualizações
2. Bug fix projeto final
3. 9Fix Finalidade do Contrato
4. 2Atualização pra 5.8
5. Atualização para 6.x
