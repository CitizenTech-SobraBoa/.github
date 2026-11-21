# SobraBoa

> **CitizenTech · FIAP Global Solution 2026/2**  
> Plataforma que conecta pequenos comércios com excedente de alimentos a organizações receptoras e voluntários — reduzindo desperdício e combatendo a insegurança alimentar.

---

## Equipe

| Nome | RM |
|---|---|
| Felipe Kirschner Modesto | RM561810 |
| João Victor Luiz Oliveira Resende | RM565139 |
| Pedro Vaz Ferreira | RM566551 |
| Vitor Dias dos Santos | RM565422 |

---

## O problema

Pequenos comércios (padarias, feiras, hortifrútis, restaurantes) descartam diariamente alimentos ainda próprios para consumo por falta de um canal simples e rápido para doá-los. Do outro lado, organizações que atendem famílias em insegurança alimentar não sabem onde e quando há doação disponível.

**O SobraBoa resolve essa equação:** o doador publica em poucos toques, quem está perto recebe aviso, reserva, retira — e o sistema gera o comprovante.

---

## ODS contemplados

- **ODS 2** — Fome zero e agricultura sustentável  
- **ODS 11** — Cidades e comunidades sustentáveis  
- **ODS 12** — Consumo e produção responsáveis

---

## Arquitetura geral

```
React Native (Mobile)
        │
        ▼
  API REST (Java Spring Boot / .NET)
        │
        ├── PostgreSQL (banco principal)
        ├── Oracle (PL/SQL — disciplina de BD)
        ├── MongoDB (NoSQL — disciplina de BD)
        ├── Job agendado (expiração de doações)
        └── IA generativa (Spring AI / Python)
```

---

## Repositórios por disciplina

| Disciplina | Repositório | Tecnologias |
|---|---|---|
| **Java Advanced** | [sobraboa-api-java](https://github.com/CitizenTech-SobraBoa/sobraboa-api-java) | Spring Boot, Spring AI, JWT, RabbitMQ |
| **Advanced Business Development with .NET** | [sobraboa-api-dotnet](https://github.com/CitizenTech-SobraBoa/sobraboa-api-dotnet) | ASP.NET Core, EF Core, JWT, xUnit |
| **Mobile Application Development** | [SobraBoa_Mobile](https://github.com/CitizenTech-SobraBoa/SobraBoa_Mobile) | React Native, Expo Router, Axios |
| **Disruptive Architectures: IoT, IoB & Generative IA** | [sobraboa-ia](https://github.com/CitizenTech-SobraBoa/sobraboa-ia) | Python, IA generativa, RAG |
| **Compliance, Quality Assurance & Tests** | [sobraboa-qa](https://github.com/CitizenTech-SobraBoa/sobraboa-qa) | Azure DevOps Boards, Test Plans |

---

## Fluxo principal

```
Doador publica excedente
        │
        ▼
Receptor próximo recebe aviso e reserva
        │
        ▼
Doador valida código de retirada
        │
        ▼
Receptor confirma recebimento
        │
        ▼
Comprovante emitido · dashboard atualizado
```

---

## Video pitch

[Assistir no YouTube](https://youtu.be/6bxx7Nn27Ag)

---

## Uso de IA generativa

Este projeto utiliza IA generativa como apoio à pesquisa, revisão de texto e explicação de erros durante o desenvolvimento. Todo código e conteúdo entregue foi compreendido, revisado e validado pela equipe.

---

## Entrega

**Prazo:** 19/11/2026 · Portal FIAP  
**Apresentações presenciais:** 23 a 27/11/2026
