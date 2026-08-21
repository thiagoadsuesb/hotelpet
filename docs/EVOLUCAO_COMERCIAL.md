# Evolucao Comercial do Hotel Pet

## Visao Geral

A versao academica do `hotelpet.shop` foi construida com **HTML5** e **CSS3** puros, sem backend, para atender aos requisitos da disciplina **Programacao Web I** da UESB.

Este documento descreve a evolucao proposta para uma versao comercial completa do sistema.

---

## 1. Arquitetura Comercial Proposta

```
hotelpet.shop (comercial)
├── Frontend
│   ├── Site institucional (Next.js ou Vue.js)
│   ├── Painel do cliente
│   └── Painel administrativo
├── Backend
│   ├── API REST (Node.js com NestJS ou Python com FastAPI)
│   ├── Autenticacao JWT
│   └── Integracoes (e-mail, pagamento, notificacoes)
├── Banco de Dados
│   ├── PostgreSQL (dados estruturados)
│   └── Redis (sessoes e cache)
├── Infraestrutura
│   ├── Hospedagem em VPS ou cloud (AWS, Azure, Vercel)
│   ├── CI/CD com GitHub Actions
│   ├── Backup automatico
│   └── Certificado SSL
└── Domínio
    └── hotelpet.shop
```

---

## 2. Funcionalidades do Site Publico

- Pagina inicial com servicos, depoimentos e contato
- Cadastro de tutores e pets
- Agendamento de estadia online
- Consulta de disponibilidade de baias
- Pagamento online
- Area do cliente para acompanhar reservas
- Blog com dicas de cuidados com pets

---

## 3. Funcionalidades do Painel Administrativo

- Dashboard com indicadores de ocupacao, faturamento e pets ativos
- Cadastro e gerenciamento de pets, tutores e usuarios
- Controle de reservas (check-in, check-out, cancelamento)
- Emissao de recibos e notas fiscais
- Relatorios financeiros e operacionais
- Configuracoes do hotel (precos, servicos, horarios)
- Notificacoes por e-mail e WhatsApp

---

## 4. Stack Tecnologica Sugerida

| Camada | Tecnologia |
|--------|------------|
| Frontend | Next.js, Tailwind CSS, TypeScript |
| Backend | Node.js + NestJS ou Python + FastAPI |
| Banco de Dados | PostgreSQL |
| Cache | Redis |
| Autenticacao | JWT + OAuth2 (Google) |
| Pagamentos | Stripe ou Mercado Pago |
| E-mail | SendGrid ou AWS SES |
| Hospedagem | Vercel (frontend) + Railway/Render (backend) |
| CI/CD | GitHub Actions |
| Monitoramento | Sentry + UptimeRobot |

---

## 5. Modelo de Dados Simplificado

```
Tutor
 ├── nome
 ├── e-mail
 ├── telefone
 └── endereco

Pet
 ├── nome
 ├── especie
 ├── raca
 ├── idade
 ├── peso
 ├── observacoes
 └── tutor_id

Reserva
 ├── pet_id
 ├── tutor_id
 ├── data_entrada
 ├── data_saida
 ├── valor_total
 ├── status
 └── servicos_adicionais

Usuario (administrativo)
 ├── nome
 ├── e-mail
 ├── senha_hash
 └── perfil (gerente, funcionario)
```

---

## 6. Planos de Monetizacao

| Plano | Descricao |
|-------|-----------|
| Basico | Hospedagem por diaria, sem servicos extras |
| Conforto | Hospedagem + passeios e alimentacao premium |
| Premium | Hospedagem + servicos completos + relatorio diario |

---

## 7. Proximos Passos

1. Definir escopo minimo viavel (MVP)
2. Criar prototipo de alta fidelidade no Figma
3. Modelar banco de dados
4. Desenvolver API REST
5. Construir frontend com React/Next.js
6. Implementar autenticacao e pagamentos
7. Realizar testes e deploy em producao

---

## 8. Relacao com a Versao Academica

A versao academica serve como **base de design e referencia visual**. As telas HTML/CSS atualmente desenvolvidas podem ser reaproveitadas como wireframes para o desenvolvimento da interface comercial.

> **Nota:** A versao comercial nao faz parte da entrega da disciplina Programacao Web I. Ela representa uma possibilidade de continuacao do projeto.
