
Criar uma API Rest em C++

Podem utilizar as biliotecas que preferirem 

O objectivo será uma API rest que irá fazer o CRUD de Colaboradores
para isso terá estes endpoints:

GET /colaboradores

que terá de response uma lista em json de todos os colaboradores

Get /colaboradores/{{id}}

que terá de response 1  colaborador com esse id

POST /colaboradores

Onde enviamos um json com as informacoes necessaria para 1 novo colaborador

PATCH /colaboradores/{{id}}

Onde enviamos um json com os campos a serem alterador para editar o colaborador com {{id}}

DELETE /colaboradores/{[id}}

que terá de response sucesso numa mensagem com o codigo http 200 se não houver aquele id para apagar responder com um código adequado


Garatir persistencia da informação, gravando em ficheiros (formato á escolha) os nossos colaboradores.

Objecto colaborador:

nome
morada
data de nascimento
departamento
