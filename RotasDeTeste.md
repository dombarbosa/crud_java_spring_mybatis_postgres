# ROTAS EXPORTADAS COMO COMANDO DE CURL

### Rota de POST

```
curl --request POST \
  --url http://localhost:8080/livros \
  --header 'Content-Type: application/json' \
  --data '{
	"titulo": "O Senhor dos Anéis - O retorno do Rei",
	"autor": "J. R. R. Tolkien",
	"isbn": "1234567891013",
	"editora": "Sextante",
	"edicao": 1
}'
```
#

### Rota de PUT

```
curl --request PUT \
  --url http://localhost:8080/livros \
  --header 'Content-Type: application/json' \
  --header 'livroid: 2' \
  --data '{
	"livroId": 2,
	"titulo": "O Senhor dos Anéis - O retorno do Rei",
	"autor": "J. R. R. Tolkien",
	"isbn": "1234567891013",
	"editora": "Nova terra",
	"edicao": 1
}'
```
#

### Rota de DELETE

```
curl --request DELETE \
  --url http://localhost:8080/livros/2
```
#

### Rota de GET

```
curl --request GET \
  --url http://localhost:8080/livros \
  --header 'livroid: 2'
```
#

#
#### Defina o ID de acordo com o registro na tabela livros da sua database
#
#

