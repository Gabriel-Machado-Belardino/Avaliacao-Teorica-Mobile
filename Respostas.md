## 1)Descreva a arquitetura do sistema operacional Android
---

    -  O sistema Android foi construído usando o **kernel Linux**, no qual ocorre o gerenciamento de memória de baixo nível, controlando por exemplo os _USBS, WIFI, Câmera, Áudio_... 
    
    -  Outra camada é o **HAL** (Camada de abstração de hardware) que consiste em módulos de biblioteca, que implementam uma interface para cada tipo específico de componente dentro do hardware, como o módulo de _câmera_.
    
    - A próxima é o Android Runtime executar várias máquinas virtuais em dispositivos de baixa memória, isto com o intuito de apresentar o menor consumo de memória possível.
    
    - Em seguida vem as Bibliotecas C/C++ nativas, estra estrutura disponibiliza bibliotecas programadas em C e C++ para que outras partes possam funcionar, como o HAL

    - As Java APIs são importantes para que os desenvolvedores de aplicativos possam ter acesso a informações do sistema.
    - E por ultimo temos Os aplicativos do sistema, aplicativos nos quais já vem baixados e são impossibilitados de apaga-los pois eles disponibilizam ações para o usuários. Tais desses aplicativos são o Telefone, Navegador, Gerenciador de mensagens...

>![][arquitetura_android]

[arquitetura_android]:https://developer.android.com/guide/platform/images/android-stack_2x.png?hl=pt-br

---
## 2)Descreva como desenvolvemos interfaces em aplicações Android nativas em Kotlin
---
1. Para começarmos precisamos abrir o **Android Studio** e criar um arquivo novo, no qual escolhemos a linguagem `Kotlin` a ser usada, apos isso programamos o nossa aplicação no arquivo _MainActivity.kt_, este arquivo representa toda a logica da aplicação
1. Tambem utilizamos a _activity_main.xml_ dentro da pasta layout para criar o design da tela da aplicação
1. E tambem utilizamos os arquivos da pasta `Drawable` para gerenciar as imagens do sistema 

## 3)	Defina o que é uma View
---

    É um objeto da interface gráfica na qual aparece para o usuário e ocupa uma área retangular dentro da tela do aplicativo, podendo ser um Botão, Imagem, Texto...
## 4)	Defina o que é um Event Listener
---
    Um Event Listener é uma parte do sistema no qual realiza uma operação quando uma ação definida é realizada.
## 5)	Defina o que é o Graddle
---

    É um sistema de compilação no qual agrupa vários builds, no qual permite o programador escrever os códigos em JAVA durante o build 
## 6)	Escreva o que é o SDK android
---
    É um emulador Android no qual nos permite testar nossas aplicações
## 7)	Escreva o que sãos API level, e dentro das configs de build o que é Target API e minimal API level
---
- API level é uma maneira de identificar diferentes versões do Android, porém esse número   é apenas utilizado pelos programadores
    - **Target API** é a versão do Android na qual a aplicação vai ser rodada, da mesma maneira que a minimal `API level` representa a versão mínima para que a aplicação rode, podendo ser diferentes, porém a minimal `API level` deve ser menor que a **Target API**
## 8)	O que é o processo de Build
---
    processo no qual traduz as linhas do código para o computador ler
## 9)	Descreva como podemos testar aplicações Android em nossos próprios celulares.
---
    Primero devemos liberar o modo desenvolvedor no celular, para que possamos habilitar o processo de depuração USB, após esse processo devemos criar uma conexão entre o Android Studio e o Dispositivo, Essa conexão pode ser a fio ou ate mesmo via Wi-fi dependendo do celular

