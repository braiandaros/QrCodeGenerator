# 📱 QR Code Generator API

Uma API REST desenvolvida em Java e Spring Boot para geração dinâmica de QR Codes. A aplicação recebe um texto ou URL, gera uma imagem de QR Code em formato PNG e faz o upload automático para um bucket do Amazon S3, devolvendo o link público da imagem gerada.

## ✨ Funcionalidades

* **Geração de QR Code:** Converte qualquer string de texto num QR Code (200x200 pixels) utilizando a biblioteca ZXing.
* **Integração Cloud (AWS S3):** Upload automático da imagem gerada para a AWS através do AWS SDK.
* **Arquitetura Limpa:** Padrão de projeto baseado em Portas e Adaptadores (Hexagonal Architecture) para separar a lógica de negócio da infraestrutura de armazenamento.

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Java 21
* **Framework:** Spring Boot (WebMVC)
* **Gestor de Dependências:** Maven
* **Processamento de Imagem:** Google ZXing (Zebra Crossing)
* **Cloud & Storage:** AWS SDK para Java (Amazon S3)

## ⚙️ Pré-requisitos

Antes de executar o projeto, certifique-se de que tem instalado na sua máquina:
* [Java 21](https://jdk.java.net/21/) ou superior.
* [Maven](https://maven.apache.org/) instalado e configurado.
* Uma conta ativa na AWS com um bucket S3 criado.
* Credenciais da AWS configuradas no seu ambiente (ex: `~/.aws/credentials` ou variáveis de ambiente `AWS_ACCESS_KEY_ID` e `AWS_SECRET_ACCESS_KEY`).

## 🚀 Configuração e Execução

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/seu-usuario/qrcode.generator.git](https://github.com/seu-usuario/qrcode.generator.git)
   cd qrcode.generator
