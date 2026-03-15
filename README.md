# ☁️ Cloud Infrastructure Status Project

Este projeto demonstra uma **arquitetura simples de aplicação cloud**, integrando um **frontend estático** com uma **API serverless hospedada na Azure**.

A aplicação consulta uma API hospedada no Azure e exibe o **status da infraestrutura em tempo real**, incluindo informações sobre o serviço, provedor e horário da última atualização.

---

## 🌐 Acesse o projeto

🔗 **Visualizar aplicação**

https://molktru.github.io/Status-da-Infraestrutura/

---

## 🏗️ Arquitetura do projeto

A aplicação utiliza uma arquitetura simples e moderna baseada em **Serverless**.

```
GitHub Pages (Frontend)
        │
        │ HTTP Request
        ▼
Azure Functions (API Serverless)
        │
        ▼
JSON Response
```

O frontend realiza uma requisição HTTP para a API, que retorna dados em formato **JSON** contendo o status do serviço.

---

## ⚙️ Tecnologias utilizadas

### Frontend

* HTML5
* CSS3
* JavaScript (Fetch API)

Hospedagem do frontend:

* GitHub Pages

---

### Backend

* Python
* Azure Functions (Serverless API)

Hospedagem da API:

* Microsoft Azure

---

## 🔐 Configurações importantes

Para que a integração entre o frontend e a API funcione corretamente, foram aplicadas algumas configurações essenciais:

* **CORS habilitado na Azure Function**
* **Endpoint HTTP público (Authorization Level: Anonymous)**
* **Formatação de horário no backend (timezone Brasil)**

---

## 📡 Exemplo de resposta da API

A API retorna os dados no formato JSON:

```json
{
  "service": "cloud-api",
  "status": "online",
  "provider": "azure",
  "timestamp": "14/03/2026 19:10:00"
}
```

Essas informações são exibidas dinamicamente no frontend.

---

## 🎯 Objetivo do projeto

Este projeto foi desenvolvido para demonstrar habilidades em:

* Arquitetura **Serverless**
* Integração **Frontend ↔ API**
* Consumo de **API REST**
* Deploy de aplicações em **Cloud**
* Configuração de **CORS**
* Uso de **Azure Functions com Python**

---

## 📌 Resultado

A aplicação exibe um pequeno **dashboard de status da infraestrutura**, permitindo verificar rapidamente se a API está online e quando foi a última atualização.

---

## 👨‍💻 Autor - Marcílio Alves Galindo

Projeto desenvolvido como parte de estudos e prática em **Cloud Computing e desenvolvimento de APIs serverless**.
