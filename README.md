# 🧙‍♂️ ASA - Entrega 02: Ambiente com DNS, Proxy Reverso e Web Servers usando Docker

Este projeto foi desenvolvido como parte da disciplina de **Administração de Sistemas e Aplicações (ASA)** e tem como objetivo a construção de um ambiente em containers Docker com:

- Um servidor **DNS** configurado manualmente
- Um **proxy reverso** com Nginx
- Dois **servidores web** representando casas de Hogwarts: Grifinória e Sonserina

---

## 📁 Estrutura do Projeto

```
ASA-Entrega-02/
├── compose.yaml               # Arquivo principal do Docker Compose
├── dns/
│   ├── Dockerfile             # Criação do container DNS
│   ├── db.asa.br              # Zona DNS com os registros
│   └── named.conf.local       # Configurações do bind9
├── proxy/
│   ├── Dockerfile             # Dockerfile do container proxy
│   ├── default.conf           # Configuração do Nginx como proxy reverso
│   └── index.html             # Página temática de Hogwarts ✨
├── web/                       # Web01 - Grifinória 🦁
│   ├── Dockerfile
│   └── index.html
├── web02/                     # Web02 - Sonserina 🐍
│   ├── Dockerfile
│   └── index.html
```

---

## ⚙️ Tecnologias Utilizadas

- 🐳 Docker e Docker Compose
- 🌐 Servidor **BIND9** para DNS
- 🔁 **Nginx** como proxy reverso
- 🌍 HTML/CSS básico para as páginas web
- 📦 Containers isolados e comunicando via rede Docker

---

## 🔍 Visão Geral do Projeto

- O DNS resolve os domínios personalizados como `grifinoria.asa.br`, `sonserina.asa.br` e `proxy.asa.br`.
- O Nginx atua como **proxy reverso**, direcionando os acessos de acordo com o nome do host.
- As páginas HTML foram personalizadas com temas de **Grifinória** e **Sonserina**, e o proxy exibe uma tela de **boas-vindas inspirada em Hogwarts**.

---

## ✅ Conclusão

Este projeto foi essencial para praticar o uso de containers em um ambiente realista, simulando um cenário com múltiplos serviços integrados via Docker. A configuração manual do DNS e o uso do Nginx como proxy reverso reforçaram conceitos importantes de rede, roteamento interno e virtualização leve.

Além disso, a personalização visual das páginas deixou o trabalho mais imersivo e divertido! 🎉

