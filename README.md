# 🃏 JokeApp

![Kotlin](https://img.shields.io/badge/Kotlin-1.9.0-7F52FF?logo=kotlin&logoColor=white)
![Jetpack Compose](https://img.shields.io/badge/Jetpack%20Compose-Enabled-4285F4?logo=android&logoColor=white)
![Retrofit](https://img.shields.io/badge/Retrofit-2.9.0-Square?logo=square&logoColor=white)
![Status](https://img.shields.io/badge/Status-Em_Desenvolvimento-yellow)

O **JokeApp** é uma aplicação nativa Android desenvolvida com **Kotlin** e **Jetpack Compose**. O objetivo principal deste projeto é consumir uma API REST externa para buscar e exibir piadas aleatórias aos utilizadores, demonstrando a implementação de comunicação de rede moderna e injeção de dependências em Android.

## 📋 Índice

* [Sobre o Projeto](#-sobre-o-projeto)
* [Tecnologias Utilizadas](#-tecnologias-utilizadas)
* [Estrutura e Arquitetura](#-estrutura-e-arquitetura)
* [Como Executar](#-como-executar)
* [Autor](#-autor)

---

## 🚀 Sobre o Projeto

Este projeto serve como um laboratório para a implementação de boas práticas no desenvolvimento Android moderno. A aplicação está configurada para realizar chamadas assíncronas a um serviço web, processar a resposta JSON e apresentar o conteúdo numa interface reativa.

### Funcionalidades Planeadas
* 📡 **Consumo de API:** Busca de piadas (Jokes) em tempo real via internet.
* 🔄 **Atualização Dinâmica:** Interface reativa que exibe novas piadas a pedido do utilizador.
* 📱 **UI Moderna:** Interface construída 100% em código com Jetpack Compose.

---

## 🛠 Tecnologias Utilizadas

O projeto foi construído utilizando as seguintes bibliotecas e ferramentas:

* **[Kotlin](https://kotlinlang.org/)**: Linguagem principal de desenvolvimento.
* **[Jetpack Compose](https://developer.android.com/jetpack/compose)**: Toolkit moderno para construção de UI nativa.
* **[Retrofit 2](https://square.github.io/retrofit/)**: Cliente HTTP *Type-safe* para Android.
* **[Gson Converter](https://github.com/google/gson)**: Serialização e deserialização de JSON para objetos Kotlin.
* **Lifecycle & ViewModel**: Gestão de estado e ciclo de vida da aplicação.

---

## 📂 Estrutura e Arquitetura

O projeto segue as diretrizes recomendadas pela Google, com foco na separação de responsabilidades. Embora esteja na fase inicial de configuração, a arquitetura prevista inclui:

* **Camada de Dados (Data Layer):** Responsável por buscar dados da API utilizando o Retrofit.
* **Camada de UI (UI Layer):** Utiliza Jetpack Compose (`MainActivity.kt`) para renderizar os dados.

**Dependências Configuradas:**
O ficheiro `build.gradle.kts` já inclui as bibliotecas necessárias para a comunicação de rede:
```kotlin
implementation("com.squareup.retrofit2:retrofit:2.9.0")
implementation("com.squareup.retrofit2:converter-gson:2.9.0")
```

---

## 🔌 Como Executar

Para testar a aplicação no seu ambiente local:

1. **Clone o repositório:**
```bash
git clone [https://github.com/soulucascardoso/JokeApp.git](https://github.com/soulucascardoso/JokeApp.git)
cd JokeApp
```

2. **Abra no Android Studio:**
    - Selecione File > Open e navegue até à pasta do projeto.
    - Aguarde a sincronização do Gradle (necessária para descarregar o Retrofit e as bibliotecas do Compose).
      
3. **Execute a Aplicação:**
    - Conecte um dispositivo físico ou inicie um emulador (API 24+).
    - Clique no botão Run (▶️).

---

## 👤 Autor

### Lucas Cardoso Rodrigues

* 🎓 Estudante de Engenharia de Computação na SATC
* 💻 Desenvolvedor Mobile & Web
* 🎥 YouTube +50k
