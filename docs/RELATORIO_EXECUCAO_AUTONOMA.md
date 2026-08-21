# Relatorio de Execucao Autonoma — Hotel Pet

## Resumo Executivo

Este relatorio descreve, de forma detalhada e em primeira pessoa, todo o trabalho realizado de maneira autonoma para transformar um prototipo no Figma em um site estatico publicado no dominio `hotelpet.shop`. O projeto foi desenvolvido como trabalho final da disciplina **Programacao Web I** da UESB e mantem, por restricao academica, apenas **HTML5 e CSS3**. Nao ha banco de dados, backend, JavaScript, frameworks ou qualquer forma de persistencia de dados. As informacoes apresentadas nas telas sao estaticas, gravadas diretamente no codigo HTML.

---

## 1. Ponto de Partida — O Prototipo no Figma

O projeto comecou a partir de um prototipo visual disponibilizado no Figma. A proposta era construir a interface de um sistema de gerenciamento de estadia para pets, representando a **visao do gerente** de um hotel para animais.

As telas principais identificadas no Figma foram:

- Tela de login
- Home com visao geral
- Cadastro e listagem de pets
- Cadastro e listagem de reservas
- Cadastro e listagem de usuarios
- Perfil do gerente
- Configuracoes do hotel

A partir dessas telas, iniciei a organizacao do projeto em HTML puro, respeitando a hierarquia visual, cores, tipografia e espacamento sugeridos no prototipo.

---

## 2. Analise dos Materiais da Disciplina

Dentro da pasta `G:\UESB`, havia diversos materiais da disciplina Programacao Web I, incluindo apostilas em PDF, atividades avaliativas anteriores e varias versoes do projeto Hotel Pet.

Identifiquei tres versoes relevantes:

- `hotelpetshop` — versao mais completa, mas com arquivos Python de apoio misturados
- `hotelpetshop_html` — versao antiga com guias de estudo
- `html-hotel-shop/final` — versao considerada final, mas sem documentacao

Decidi unificar o melhor de cada uma e reconstruir uma versao final limpa, academica e publicavel.

---

## 3. Reorganizacao e Limpeza do Projeto

A primeira acao pratica foi reorganizar a estrutura de pastas. Muitos arquivos estavam fora dos lugares corretos:

- CSS e imagens estavam dentro de `docs/`
- Materiais de estudo estavam misturados com os arquivos do site
- Arquivos Python de apoio local estavam na raiz do projeto

Criei a seguinte estrutura organizada:

```
Programacao-Web-I/
├── css/                  # Folhas de estilo
├── imagens/              # Imagens, icones e favicon
├── docs/                 # Documentacao academica
├── documentos/           # Materiais de estudo e historico
│   ├── material-estudo/
│   └── historico/
├── index.html
├── login.html
├── ... outras paginas
└── README.md
```

Também removi estilos inline, padronizei cabecalhos academicos em todos os arquivos HTML e CSS, e adicionei favicon em todas as paginas.

---

## 4. Desenvolvimento em HTML e CSS

### 4.1 HTML

Foram criadas 23 paginas HTML semanticamente estruturadas, utilizando:

- `header`, `main`, `section`, `aside`, `nav`, `footer`
- Formularios com `fieldset`, `legend`, `label`, `input`, `select`, `textarea`, `button`
- Tabelas para listagens de pets, reservas e usuarios
- Menu lateral fixo com navegacao entre modulos
- Breadcrumb e area de perfil do gerente

Todas as paginas possuem um cabecalho academico padronizado informando universidade, curso, disciplina, professor, aluno, etapa e tecnologias utilizadas.

### 4.2 CSS

Foram criados dois arquivos CSS:

- `css/estilo.css` — estilos principais do sistema
- `css/login.css` — estilos especificos da tela de login

Os conceitos aplicados incluem:

- Box Model (margin, padding, border)
- Tipografia e cores
- Flexbox para layouts
- Estados de interacao (`:hover`, `:focus`)
- Design responsivo com `@media queries`
- CSS para impressao do recibo (`@media print`)

### 4.3 Simulacoes Estaticas

Como nao ha backend, as operacoes de login, cadastro, edicao e exclusao foram simuladas atraves de navegacao entre paginas HTML.

Exemplos de fluxos simulados:

- Login: `login.html` → `login_demo.html`
- Cadastro de usuario: `usuario_cadastrar.html` → `usuario_criado.html`
- Exclusao de usuario: `usuario_visualizar.html` → `usuario_excluir.html` → `usuario_excluido.html`
- Recibo: `reserva_visualizar.html` → `reserva_recibo.html`

As informacoes apresentadas, como o nome "Joao da Silva", dados de pets, reservas e usuarios, estao **gravados estaticamente no HTML**. Nao existe banco de dados. Nenhuma informacao e salva, editada ou excluida de verdade.

---

## 5. Versionamento com Git

Iniciei o versionamento do projeto com Git e organizei os commits de forma clara:

1. `Entrega Semana 1 - HTML - 14/08/2026` — estrutura inicial das telas
2. `Etapa 2 - Estilizacao CSS e homologacao do Hotel Pet` — estilizacao e organizacao
3. `Adiciona CNAME para dominio hotelpet.shop` — preparacao para dominio personalizado
4. `Adiciona workflow de deploy no GitHub Pages, README profissional e evolucao comercial` — automacao e documentacao

Também criei arquivos de configuracao como `.editorconfig`, `.gitattributes` e `.gitignore` para manter a padronizacao do repositorio.

---

## 6. Geracao de Chaves SSH e Publicacao no GitHub

Para publicar o projeto no GitHub de forma segura, gerei um par de chaves SSH do tipo ED25519:

- Chave privada: `C:\Users\Thiago\.ssh\id_ed25519_thiagoadsuesb`
- Chave publica: `C:\Users\Thiago\.ssh\id_ed25519_thiagoadsuesb.pub`

Configurei o arquivo `C:\Users\Thiago\.ssh\config` com um host especifico para a conta `thiagoadsuesb` no GitHub.

Apos o aluno adicionar a chave publica na conta GitHub, realizei o push do repositorio para:

```
https://github.com/thiagoadsuesb/hotelpet
```

Como o repositorio remoto ja possuia um historico inicial, utilizei a estrategia de merge `ours` para preservar a versao final local sem perder o historico anterior.

---

## 7. Repositório de Perfil do GitHub

Para deixar o GitHub mais profissional e academico, criei um repositorio de perfil com o mesmo nome do usuario: `thiagoadsuesb/thiagoadsuesb`.

Esse repositorio contem um `README.md` com:

- Apresentacao pessoal
- Formacao academica na UESB
- Principais projetos
- Habilidades em desenvolvimento
- Estatisticas do GitHub
- Links de contato

O perfil ficou disponivel em:

```
https://github.com/thiagoadsuesb
```

---

## 8. Documentacao Criada

Foram elaborados os seguintes documentos dentro do projeto:

- `README.md` — apresentacao profissional e academica do projeto
- `docs/MAPA_DE_ROTAS.md` — mapeamento completo de todos os links
- `docs/RELATORIO_HOMOLOGACAO.md` — relatorio de validacao do projeto
- `docs/EVOLUCAO_COMERCIAL.md` — proposta de evolucao para uma versao comercial
- `docs/RELATORIO_EXECUCAO_AUTONOMA.md` — este relatorio

Também foi gerado um arquivo `manifesto_sha256.txt` com hash de integridade dos arquivos do projeto.

---

## 9. Automacao do Deploy com GitHub Actions

Criei um workflow em `.github/workflows/deploy.yml` para publicar automaticamente o site no GitHub Pages sempre que houver um push na branch `main`.

O workflow executa as seguintes etapas:

1. Checkout do codigo
2. Configuracao do GitHub Pages
3. Upload do artefato estatico
4. Deploy para o ambiente `github-pages`

Apos a ativacao do GitHub Actions nas configuracoes do repositorio, o workflow funcionou corretamente e publicou o site em:

```
https://thiagoadsuesb.github.io/hotelpet/
```

---

## 10. Compra do Dominio e Configuracao no Cloudflare

O dominio `hotelpet.shop` foi adquirido pelo aluno em um registrador de dominios. Inicialmente, os DNS estavam configurados para apontar para a Hostinger.

Para utilizar o dominio com o GitHub Pages, realizamos a migracao dos nameservers para o Cloudflare:

```
carlos.ns.cloudflare.com
riya.ns.cloudflare.com
```

Apos a propagacao dos nameservers, configurei os registros DNS necessarios para apontar o dominio para o GitHub Pages:

| Tipo | Nome | Conteudo |
|------|------|----------|
| A | `@` | `185.199.108.153` |
| A | `@` | `185.199.109.153` |
| A | `@` | `185.199.110.153` |
| A | `@` | `185.199.111.153` |
| CNAME | `www` | `thiagoadsuesb.github.io` |

A configuracao foi realizada atraves da API do Cloudflare, utilizando um token de acesso temporario fornecido pelo aluno. Apos o uso, o token foi revogado por questoes de seguranca.

---

## 11. Configuracao do Dominio Personalizado no GitHub Pages

No painel de configuracao do GitHub Pages do repositorio `thiagoadsuesb/hotelpet`, foi adicionado o dominio personalizado:

```
hotelpet.shop
```

O GitHub realizou a verificacao de DNS e confirmou que tudo estava correto. O certificado SSL foi provisionado automaticamente pelo Let's Encrypt, e o site passou a responder via HTTPS.

A opcao **Enforce HTTPS** foi disponibilizada e deve ser ativada para forcar todo o trafego para a versao segura do site.

---

## 12. Resultado Final

O site Hotel Pet foi publicado com sucesso e esta acessivel em:

```
https://hotelpet.shop
```

A verificacao final confirmou:

- Status HTTP: 200 OK
- URL final: https://hotelpet.shop/
- Titulo da pagina: Home - Hotel Pet
- DNS check no GitHub Pages: successful

O repositorio completo pode ser consultado em:

```
https://github.com/thiagoadsuesb/hotelpet
```

---

## 13. Caracteristicas Tecnicas Importantes

E crucial destacar que esta versao do Hotel Pet e **estatica e academica**:

- **Nao ha banco de dados.**
- **Nao ha backend.**
- **Nao ha JavaScript.**
- **Nao ha frameworks ou bibliotecas externas.**
- **Nao ha persistencia de dados.**

Todas as informacoes exibidas, como nome do gerente, lista de pets, reservas e usuarios, estao gravadas diretamente nos arquivos HTML. Qualquer simulacao de cadastro, edicao ou exclusao e apenas uma navegacao entre paginas estaticas.

Essa restricao e intencional e atende aos requisitos da disciplina Programacao Web I, que tem como foco o dominio de HTML5 e CSS3.

---

## 14. Evolucao Futura — Versao Comercial

A ideia do Hotel Pet foi considerada otima e com grande potencial para evolucao. Por isso, foi elaborado um documento de evolucao comercial (`docs/EVOLUCAO_COMERCIAL.md`) descrevendo uma versao completa do sistema.

A versao comercial proposta incluira:

- **Backend em Python** — provavelmente utilizando FastAPI ou Django
- **Banco de dados PostgreSQL** — para persistencia de tutores, pets, reservas, usuarios e pagamentos
- **Sistema vetorizado** — possivelmente para busca semantica, recomendacoes de servicos ou matching de pets com acomodacoes
- **Autenticacao real** — login com senha criptografada e controle de perfis
- **Painel administrativo dinamico** — com dashboards, relatorios e gestao completa
- **Site publico para clientes** — com agendamento online e pagamento integrado
- **API REST** — para comunicacao entre frontend e backend
- **CI/CD** — com GitHub Actions para deploy automatizado
- **Hospedagem em cloud** — AWS, Azure ou provedores especializados

Essa evolucao transformara o projeto de uma interface estatica academica em uma aplicacao real, escalavel e comercialmente viavel.

---

## 15. Consideracoes Finais

Todo o processo, desde a analise do prototipo ate a publicacao no dominio proprio, foi realizado de forma autonoma, seguindo boas praticas de organizacao, versionamento, documentacao e seguranca.

O resultado e um site funcional, bem estruturado, publicado em um dominio personalizado e pronto para servir de base para uma futura aplicacao completa em Python com PostgreSQL.

---

**Relatorio elaborado em:** 21 de agosto de 2026  
**Projeto:** Hotel Pet  
**Disciplina:** Programacao Web I — UESB  
**Aluno:** Thiago Ferreira Prates Neves
