# Mapa de Rotas — Hotel Pet

## Validacao de links

Todos os links locais foram verificados em cada pagina HTML.

| Origem | Tipo | Destino | Existe | Observacao |
|--------|------|---------|--------|------------|
| login.html | href | login_demo.html | Sim | Simulacao de login |
| login.html | href | usuario_cadastrar.html | Sim | Criar conta |
| login_demo.html | href | index.html | Sim | Entrada no sistema |
| index.html | href | pets.html | Sim | Menu lateral |
| index.html | href | usuarios.html | Sim | Menu lateral |
| index.html | href | configuracoes.html | Sim | Menu lateral |
| index.html | href | reservas.html | Sim | Menu lateral |
| index.html | href | perfil.html | Sim | Cabecalho |
| index.html | src | imagens/logo.svg | Sim | Logo |
| index.html | src | imagens/avatar-joao.svg | Sim | Avatar |
| pets.html | href | pet_cadastrar.html | Sim | Novo pet |
| pets.html | href | pet_visualizar.html | Sim | Visualizar |
| pets.html | href | pet_editar.html | Sim | Editar |
| pet_cadastrar.html | action | pets.html | Sim | Voltar apos cadastro |
| pet_editar.html | action | pets.html | Sim | Voltar apos edicao |
| reservas.html | href | reserva_cadastrar.html | Sim | Nova reserva |
| reservas.html | href | reserva_visualizar.html | Sim | Visualizar |
| reservas.html | href | reserva_editar.html | Sim | Editar |
| reserva_cadastrar.html | action | reservas.html | Sim | Voltar apos cadastro |
| reserva_editar.html | action | reservas.html | Sim | Voltar apos edicao |
| reserva_visualizar.html | href | reserva_editar.html | Sim | Editar reserva |
| reserva_visualizar.html | href | reserva_recibo.html | Sim | Visualizar recibo |
| usuarios.html | href | usuario_cadastrar.html | Sim | Novo usuario |
| usuarios.html | href | usuario_visualizar.html | Sim | Visualizar |
| usuarios.html | href | usuario_editar.html | Sim | Editar |
| usuario_cadastrar.html | action | usuario_criado.html | Sim | Confirmacao de cadastro |
| usuario_visualizar.html | href | usuario_editar.html | Sim | Editar usuario |
| usuario_visualizar.html | href | usuario_excluir.html | Sim | Excluir usuario |
| usuario_excluir.html | href | usuario_excluido.html | Sim | Confirmar exclusao |
| usuario_excluido.html | href | usuarios.html | Sim | Voltar para lista |
| configuracoes.html | action | configuracoes.html | Sim | Simulacao de salvar |
| perfil.html | action | perfil.html | Sim | Simulacao de salvar |
| todas as paginas | stylesheet | css/estilo.css | Sim | Estilo principal |
| login.html | stylesheet | css/login.css | Sim | Estilo do login |
| todas as paginas | icon | imagens/favicon.svg | Sim | Favicon |

## Resultado

- Total de paginas HTML: 23
- Links quebrados: 0
- Referencias JavaScript: 0
- Referencias Python: 0
- Frameworks: 0
- Bibliotecas externas: 0

## Observacao

As acoes de formularios utilizam `method="get"` e apontam para paginas estaticas de confirmacao, conforme o escopo academico do projeto.
