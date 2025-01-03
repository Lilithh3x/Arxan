
*Esse artigo é baseado nas minhas necessidades e nas pesquisas realizadas na internet. Caso alguma informação não esteja correta ou você deseje acrescentar algo, peço que entre em contato comigo por meio de qualquer rede social disponível no meu perfil. Boa leitura!*

O Arxan é um sistema de proteção mobile contra ameaças de segurança, como engenharia reversa, roubo de propriedade intelectual e exploração de vulnerabilidades.

O Arxan não realiza chamadas de sistema, mas monitora e intercepta as chamadas feitas pelo aplicativo para protegê-lo contra ameaças de segurança em tempo de execução.

O Arxan utiliza um conjunto de técnicas de proteção, que incluem:

1. Ofuscação de código
2. Criptografia de código
3. Verificação de integridade
4. Controle de fluxo
5. Proteção de dados

**Arxan Runtime Library:** é uma biblioteca dinâmica usada para fornecer a proteção do Arxan em tempo de execução.

**GuardIt:** é uma solução de proteção de aplicativos móveis oferecida pela empresa Arxan.

---
**Tools**
* https://github.com/pr701/fix-arxan
---
### **Como funcionam as proteções de memória?**

Uma das proteções de memória é a **criptografia de seções de código**, que consiste em criptografar partes do código e dos dados do aplicativo.

Tipos de criptografia utilizados pelo Arxan:

- **Criptografia simétrica:** usada para proteger dados em repouso no dispositivo, incluindo dados armazenados no disco e na memória cache. O Arxan utiliza criptografias simétricas como AES e DES para criptografar e descriptografar os dados.

- **Criptografia assimétrica:** usada para proteger a comunicação entre o dispositivo e o servidor. O Arxan utiliza algoritmos de criptografia assimétrica como RSA e Diffie-Hellman.

- **Criptografia de ponteiros de função:** utilizada para proteger os ponteiros de função no código do aplicativo. Essa criptografia é feita durante a compilação e, durante a execução do aplicativo, os ponteiros de função são descriptografados em tempo real e usados normalmente.

Além dessas técnicas, o Arxan utiliza outras estratégias para proteger a memória do aplicativo, como a aleatorização de seções de memória e o monitoramento da atividade de memória.

---
### **Como funcionam as proteções de detecção?**

As proteções de detecção são utilizadas para proteger a integridade de um aplicativo contra ataques.

O Arxan utiliza diferentes técnicas de proteção, como:

- **Detecção de depuradores:** o Arxan verifica regularmente se há um depurador em execução e, se detectado, toma medidas de proteção para interromper o processo de depuração.

- **Detecção de emulação:** técnica usada para identificar a presença de emuladores que possam estar manipulando ou analisando o código do aplicativo. Se um emulador for detectado, o Arxan interrompe o processo para proteger o aplicativo.

- **Detecção de manipulação de código:** o Arxan utiliza a técnica de anti-tamper para verificar a integridade do código em tempo de execução. Se alguma manipulação for detectada, o processo é interrompido.

- **Detecção de injeção de código:** o Arxan monitora o processo do aplicativo para identificar tentativas de injetar códigos maliciosos. Caso detectada, a injeção é bloqueada.

- **Detecção de root/jailbreak:** o Arxan realiza verificações para identificar se o dispositivo foi comprometido. Em caso positivo, o processo de execução do aplicativo é interrompido.

---
### **Como funciona o monitoramento de atividade de memória?**

O monitoramento de atividade de memória envolve uma verificação constante das ações realizadas pelo aplicativo, em busca de comportamentos suspeitos que possam indicar algum tipo de ataque.

Essa monitorização é feita em tempo real e detecta diferentes tipos de ataques, como tentativas de acesso a áreas de memória não autorizadas ou manipulação de variáveis críticas.

O Arxan utiliza técnicas como:

- Verificação da integridade do código.
- Análise de padrões de acesso à memória.
- Detecção de tentativas de escrita em áreas de memória somente leitura.

Além disso, o Arxan pode isolar áreas críticas da memória do aplicativo. Caso seja identificada alguma atividade suspeita, o aplicativo é interrompido ou um código de defesa específico é ativado para bloquear o ataque.

---
### **Como funciona a prevenção de hooking de funções?** 

A prevenção de hooking de funções é uma técnica usada pelo Arxan para proteger o aplicativo contra ataques que visam modificar ou interceptar suas funções.

O hooking de função é uma técnica que altera o comportamento do aplicativo redirecionando uma chamada de função para outra ou injetando códigos maliciosos.

Para prevenir o hooking, o Arxan utiliza proteções baseadas em criptografia e ofuscação de código, realizadas durante a compilação. Essas proteções incluem:

- Renomeação de funções.
- Inserção de códigos redundantes.
- Alteração do fluxo de controle do aplicativo.

Se houver uma tentativa de hooking, o Arxan pode interromper a execução do aplicativo ou ativar um código de defesa para bloquear o ataque.

---
