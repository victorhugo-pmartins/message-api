# REST API publicação e listagem de mensagens curtas

Aplicação desenvolvida em [Laravel 5.3](http://laravel.com) com intúito de aplicar para a vaga de Desenvolvedor PHP.

## API list
<pre>
+--------+-----------+------------------------+------------------+-------------------------------------------------+--------------+
| Domain | Method    | URI                    | Name             | Action                                          | Middleware   |
+--------+-----------+------------------------+------------------+-------------------------------------------------+--------------+
|        | POST      | api/messages           | messages.store   | App\Http\Controllers\MessagesController@store   | api          |
|        | GET|HEAD  | api/messages           | messages.index   | App\Http\Controllers\MessagesController@index   | api          |
|        | DELETE    | api/messages/{id}      | messages.destroy | App\Http\Controllers\MessagesController@destroy | api          |
|        | GET|HEAD  | api/messages/{id}      | messages.show    | App\Http\Controllers\MessagesController@show    | api          |
|        | PUT|PATCH | api/messages/{id}      | messages.update  | App\Http\Controllers\MessagesController@update  | api          |
+--------+-----------+------------------------+------------------+-------------------------------------------------+--------------+
</pre>

## Instalação

- PHP >=5.6;
- Clonar o repositório;
- No diretório do projeto instalar as dependências via composer;
<pre>composer install</pre>
- Copiar o arquivo .env.example para .env e configurar a base de dados;
<pre>cp .env.example .env</pre>
- Rodar as Migrations;
<pre>php artisan migrate</pre>
- Gerar a key da aplicação;
<pre>php artisan key:generate</pre>
