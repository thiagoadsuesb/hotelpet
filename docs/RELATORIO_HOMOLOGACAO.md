# Relatório de Homologação — Hotel Pet

## 1. Identificação

- **Universidade:** UESB
- **Curso:** Análise e Desenvolvimento de Sistemas — EAD
- **Disciplina:** Programação Web I
- **Professor:** Lucas Santos de Oliveira
- **Aluno:** Thiago Ferreira Prates Neves
- **Repositório:** https://github.com/thiagoadsuesb/hotelpet
- **Domínio:** https://www.hotelpet.shop

## 2. Contexto Acadêmico

Projeto final da disciplina Programação Web I, dividido em duas entregas:

- **Semana 1 (14/08/2026):** Estrutura HTML.
- **Semana 2 (21/08/2026):** Estilização CSS e organização.

O projeto representa a visão do gerente de um sistema de gerenciamento de estadia de pets.

## 3. Fontes Analisadas

- Enunciado do trabalho final.
- Apostilas de HTML e CSS.
- Slides das aulas.
- Protótipo do Figma.
- PDFs exportados do Figma.
- Material de estudo disponibilizado pelo professor.

## 4. Problemas Encontrados

1. **Estrutura de pastas desorganizada:** arquivos CSS e imagens estavam dentro de `docs/`.
2. **Faltavam favicons:** as páginas não possuíam link de favicon.
3. **Inline style:** `index.html` utilizava `style="font-size:18px;"` diretamente no HTML.
4. **Faltavam páginas de simulação:** login, criação de usuário, exclusão e recibo não possuíam fluxos estáticos.
5. **Sem cabeçalho acadêmico:** arquivos não possuíam identificação padronizada.
6. **Materiais de estudo misturados:** PDFs e documentos estavam na mesma pasta do site.

## 5. Correções Realizadas

1. Reorganização das pastas `css/`, `imagens/`, `docs/` e criação de `documentos/material-estudo/`.
2. Adição de favicon em todas as páginas.
3. Remoção do inline style e criação da classe `.titulo-secao` no CSS.
4. Criação das páginas de simulação:
   - `login_demo.html`
   - `usuario_criado.html`
   - `usuario_excluir.html`
   - `usuario_excluido.html`
   - `reserva_recibo.html`
5. Adição de cabeçalho acadêmico em todos os arquivos HTML e CSS.
6. Atualização dos formulários para apontarem para páginas de confirmação estáticas.
7. Criação do CSS de impressão para o recibo (`@media print`).
8. Validação de todos os links locais.

## 6. HTML

- Estrutura semântica com `header`, `main`, `section`, `nav`, `aside`, `footer`.
- Formulários com `fieldset`, `legend`, `label`, `input`, `select`, `textarea`, `button`.
- Tabelas para listagens de pets, reservas e usuários.
- Menu lateral e breadcrumb em todas as páginas internas.
- Logomarca com link para `index.html`.

## 7. CSS

- Arquivo principal: `css/estilo.css`.
- Arquivo específico para login: `css/login.css`.
- Utilização de variáveis não aplicada, mantendo compatibilidade com o nível acadêmico.
- Conceitos aplicados:
  - Box Model (`margin`, `padding`, `border`, `border-radius`, `box-sizing`)
  - Tipografia (`font-family`, `font-size`, `font-weight`, `line-height`)
  - Cores (`background-color`, `color`)
  - Layout (`display`, `flex`)
  - Estados (`:hover`, `:focus`, `:active`)
  - Responsividade (`@media`)
  - Impressão (`@media print`)

## 8. Herança, Cascata e Especificidade

- A tipografia base é definida no `body` e herdada pelos elementos filhos.
- A cor dos links é controlada por classes específicas para evitar conflitos.
- Classes são utilizadas para estilização repetitiva; IDs são evitados.
- O seletor `.menu .item.ativo` demonstra especificidade combinada.

## 9. Funcionalidades como Simulação Estática

### Login
- O formulário de `login.html` envia para `login_demo.html`.
- `login_demo.html` informa que se trata de uma simulação e oferece link para `index.html`.

### Criação de Usuário
- O formulário de `usuario_cadastrar.html` envia para `usuario_criado.html`.
- A página de confirmação exibe mensagem estática de sucesso.

### Exclusão de Usuário
- `usuario_visualizar.html` possui link "Remover".
- `usuario_excluir.html` solicita confirmação.
- `usuario_excluido.html` exibe mensagem estática de exclusão simulada.

### Recibo
- `reserva_visualizar.html` possui link "Visualizar recibo".
- `reserva_recibo.html` exibe o recibo formatado.
- CSS de impressão oculta elementos de navegação e mantém apenas o recibo.

## 10. Testes

### Teste de Links
- Ferramenta: script PowerShell de validação local.
- Resultado: 0 links quebrados.

### Teste Sem JavaScript
- JavaScript desativado no navegador.
- Resultado: navegação e simulações continuam funcionando.

### Teste de Impressão
- Página: `reserva_recibo.html`.
- Resultado: elementos de navegação ocultos; recibo visível.

### Teste de Responsividade
- Resoluções testadas: 1440px, 1280px, 1024px, 768px, 480px, 375px.
- Resultado: menu, formulários, tabelas e botões se adaptam.

## 11. Git e GitHub

- Repositório: `thiagoadsuesb/hotelpet`
- Branch principal: `main`
- Chave SSH: `~/.ssh/id_ed25519_thiagoadsuesb`
- Configuração SSH: `~/.ssh/config` com host `thiagoadsuesb.github.com`

## 12. Pendências

- Adicionar a chave pública SSH à conta GitHub `thiagoadsuesb` para habilitar push via SSH.
- Verificar publicação no GitHub Pages após configuração.

## 13. Conclusão

O projeto Hotel Pet está organizado como uma entrega acadêmica de HTML e CSS, com navegação estática, simulações de operações, recibo para impressão e documentação. Todas as restrições do enunciado foram respeitadas: sem JavaScript, sem frameworks, sem backend e sem banco de dados.
