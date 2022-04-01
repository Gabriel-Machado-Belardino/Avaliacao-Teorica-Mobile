## 1)Descreva a arquitetura do sistema operacional Android
---

    -  O sistema Android foi construído usando o **kernel Linux**, no qual ocorre o gerenciamento de memória de baixo nível, controlando por exemplo os _USBS, WIFI, Câmera, Áudio_... 
    
    -  Outra camada é o **HAL** (Camada de abstração de hardware) que consiste em módulos de biblioteca, que implementam uma interface para cada tipo específico de componente dentro do hardware, como o módulo de _câmera_.
    
    - A próxima é o Android Runtime executar várias máquinas virtuais em dispositivos de baixa memória, isto com o intuito de apresentar o menor consumo de memória possível.
    
    - Em seguida vem as Bibliotecas C/C++ nativas, estra estrutura disponibiliza bibliotecas programadas em C e C++ para que outras partes possam funcionar, como o HAL

    - As Java APIs são importantes para que os desenvolvedores de aplicativos possam ter acesso a informações do sistema.
    - E por ultimo temos Os aplicativos do sistema, aplicativos nos quais já vem baixados e são impossibilitados de apaga-los pois eles disponibilizam ações para o usuários. Tais desses aplicativos são o Telefone, Navegador, Gerenciador de mensagens...