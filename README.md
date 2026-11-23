# 🖨️ Sistema de Controle de Impressora Elgin
### *(Controle de impressora com Java)*
---

## 📘 Sobre o Projeto


Este projeto foi desenvolvido pelo nosso grupo para se comunicar com uma impressora térmica **Elgin i8/i9** usando a biblioteca `E1_Impressora01.dll`. O sistema tem login com 3 tentativas, que é executado dentro de uma classe Menu, e um menu com operações da impressora que também está dentro da classe Menu, e a classe Impressora que possuí todos os métodos de cada opção. Faz parte da disciplina de **Programação Orientada a Objetos** do curso Técnico em Informática do Colégio UNASP-SP.

---

## 🧰 Tecnologias Utilizadas

- **Java** *(Versão 27)*
- **IntelliJ IDEA** 
- **JNA 5.15.0** (comunicação com a DLL)
- **DLL E1_Impressora01** (SDK da Elgin)
- **Impressora Elgin i8 ou i9** *(i9 utilizada para testes)*

---

## 📁 Estrutura do Projeto

*(Liste suas pastas e classes e diga o que cada uma faz.)*

```
/src                      → Código-fonte com todas as classes dentro dele. 
   Main.java              → Classe principal, responsável por rodar o progarma e criar os objetos.
   Menu.java           → Classe responsável pelo login com 3 tentativas e responsável por mostrar o menu com as opções.
   Impressora.java        → Classe responsável por executar todas as opções presentes no menu.
/Bibliotecas E1 Impressora → DLLs da Elgin (x64 e x86)
/libs Java                → jna-5.15.0.jar (Versão do JNA utilizada)
```

---

## ⚙️ Instalação e Execução



### 1. Baixar o projeto
1. Acesse o repositório no GitHub.
2. Clique em **Code → Download ZIP**.
3. Extraia o arquivo.

### 2. Abrir no IntelliJ IDEA
1. **File → Open** e escolha a pasta extraída.
2. Em **File → Project Structure → Libraries**, confirme que o `jna-5.15.0.jar` está adicionado.
3. Conecte e ligue a impressora.
4. Abra `Main.java` e clique em ▶️ **Run**.
5. Faça o Login digitando o usuário e senha corretos, você terá 3 tentativas.
6. Escolha uma opção do menu apresentado, mas primeiro abra a conexão, caso contrário uma mensagem pedindo para abrir a conexão será enviada.

---

## 🔐 Login

*Usuário de teste: cr7; Senha de teste: 1234567; 3 tentativas de acerto.*

---

## 📋 Funcionalidades do Menu

| Opção | O que faz |
|---|---|
| 1 | *(Configura a conexão com a impressora)* |
| 2 | *(Abre a conexão com a impressora)* |
| 3 | *(Fecha a conexão com a impressora)* |
| 4 | *(Imprime um texto)* |
| 5 | *(Imprime um QR code)* |
| 6 | *(Imprime um código de barras)* |
| 7 | *(Imprime XML SAT)* |
| 8 | *(Imprime XML de cancelamento SAT)* |
| 9 | *(Abre a gaveta da impressora)* |
| 10 | *(Emite sinal sonoro)* |
| 11 | *(Avança o papel)* |
| 12 | *(Status do papel)* | 
| 0 | *(Sair)* |
---

## 🧪 Testes Realizados

*(Testamos o funcionamento d login com 3 tentativas, e testamos cada uma das opções presentes no menu. Ajustamos um erro na função de imprimir código de barras e no tempo de cada Bip.)*

---

## 📚 Documentação Adicional

- https://elgindevelopercommunity.github.io/group___m1.html
- Documentação do SDK E1_Impressora

---

## 👥 Autores
*(em ordem alfabética)*

- Gabriel Brito
- Luiz Gustavo
- Victor Raphael Frana
