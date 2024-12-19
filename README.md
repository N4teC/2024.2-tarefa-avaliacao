# 2024.2 Avaliação do 1o período de Sistemas Operacionais

## Informações gerais
- **Objetivo do repositório**: Avaliação do 1o bimestre da Disciplina de sistemas operacionais do curso de TADS do IFRN-CNAT
- **Público alvo**: alunos da disciplina de SO (Sistemas Operacionais) do curso de TADS (Superior em Tecnologia em Análise e Desenvolvimento de Sistemas) no CNAT-IFRN (Instituto Federal de Educação, Ciência e Tecnologia do Rio Grande do Norte - Campus Natal-Central).
- disciplina: **SO** Sistemas Operacionais
- professor: [Leonardo A. Minora](https://github.com/leonardo-minora)

## Avaliação
- **Lembre de fazer o fork deste repositório**
- As questões foram construídas com o auxílio do [copilot](https://copilot.microsoft.com/)

# Questão 1. Introdução a sistemas operacionais

Considere as funções e objetivos principais de um sistema operacional conforme discutido no texto. Explique como um sistema operacional gerencia os recursos de hardware e software de um computador para garantir eficiência e segurança. Em sua resposta, aborde os seguintes pontos:

- Gerenciamento de processos
- Gerenciamento de memória
- Gerenciamento de dispositivos de entrada e saída
- Gerenciamento de arquivos

**Dica**: Pense em exemplos práticos de como o sistema operacional realiza essas tarefas no dia a dia de um usuário.

**Copilot informa**: Essa questão incentiva os alunos a explorarem os conceitos fundamentais e a aplicarem o conhecimento teórico em situações práticas. Se precisar de mais alguma coisa, estou aqui para ajudar!

# Resposta 1:

## Como um Sistema Operacional Gerencia os Recursos do Computador

### **Gerenciamento de Processos**
O sistema operacional gerencia processos coordenando a execução de múltiplos programas de forma simultânea. Ele utiliza o escalonamento de processos para alocar a CPU eficientemente, permitindo que tarefas como abrir um navegador e um editor de texto ocorram ao mesmo tempo. Além disso, ele isola processos para evitar que falhas em um programa afetem os outros e utiliza mecanismos de comunicação entre processos para sincronização e colaboração.

### **Gerenciamento de Memória**
No gerenciamento de memória, o SO distribui a memória RAM entre os programas em execução, garantindo que cada um tenha acesso somente ao espaço necessário. Ele também utiliza a memória virtual para ampliar a capacidade disponível, transferindo dados temporariamente para o disco rígido ou SSD. Isso é visível, por exemplo, quando você edita fotos em programas que exigem grande capacidade de memória.

### **Gerenciamento de Dispositivos de Entrada e Saída**
O SO gerencia dispositivos de entrada e saída, como teclados, mouses e impressoras, por meio de drivers que padronizam a comunicação com o hardware. Ele utiliza técnicas como spooling para gerenciar filas de impressão e protege o acesso a dispositivos sensíveis, como webcams, pedindo permissão ao usuário antes de liberar o uso.

### **Gerenciamento de Arquivos**
Por fim, o gerenciamento de arquivos organiza os dados no sistema de arquivos, permitindo fácil acesso por meio de hierarquias de pastas. O SO controla permissões para garantir a segurança e pode usar logs para recuperar arquivos em caso de falhas inesperadas. Um exemplo disso é a recuperação automática de documentos no editor de texto após um desligamento abrupto.

# Questão 2. Estrutura de sistemas operacionais

## Texto informativo
### Estrutura de Sistemas Operacionais: Custo de Desenvolvimento e Segurança da Informação

A estrutura de um sistema operacional (SO) é fundamental para determinar tanto o custo de desenvolvimento e manutenção quanto a segurança da informação. Existem várias arquiteturas de SO, como monolítica, microkernel e em camadas, cada uma com suas próprias implicações em termos de custo e segurança.

#### Custo de Desenvolvimento e Manutenção

1. **Arquitetura Monolítica**:
   - **Desenvolvimento**: Geralmente, mais rápida de desenvolver inicialmente, pois todos os componentes do SO são integrados em um único bloco de código.
   - **Manutenção**: Pode ser mais complexa e cara, pois qualquer alteração em um componente pode afetar todo o sistema, exigindo testes extensivos e cuidadosos.

2. **Arquitetura Microkernel**:
   - **Desenvolvimento**: Pode ser mais demorada e cara inicialmente, pois envolve a criação de um núcleo mínimo e a implementação de serviços adicionais como processos separados.
   - **Manutenção**: Mais fácil e menos custosa, já que os componentes são isolados. Atualizações e correções podem ser feitas em módulos específicos sem impactar o núcleo do sistema.

3. **Arquitetura em Camadas**:
   - **Desenvolvimento**: Moderadamente complexa, pois cada camada deve ser bem definida e interagir corretamente com as outras.
   - **Manutenção**: Relativamente fácil, pois problemas podem ser isolados e corrigidos em camadas específicas sem afetar o restante do sistema.

#### Segurança da Informação

1. **Arquitetura Monolítica**:
   - **Segurança**: Pode ser mais vulnerável, pois uma falha em qualquer parte do sistema pode comprometer todo o SO. A integração de todos os componentes em um único bloco de código pode dificultar a implementação de medidas de segurança robustas.

2. **Arquitetura Microkernel**:
   - **Segurança**: Geralmente mais segura, pois isola os serviços em processos separados. Isso limita o impacto de uma falha ou ataque a um único componente, protegendo o núcleo do sistema e outros serviços.

3. **Arquitetura em Camadas**:
   - **Segurança**: Oferece um bom equilíbrio, pois cada camada pode implementar suas próprias medidas de segurança. No entanto, a comunicação entre camadas deve ser cuidadosamente gerenciada para evitar vulnerabilidades.

### Conclusão

A escolha da arquitetura de um sistema operacional tem um impacto significativo tanto no custo de desenvolvimento e manutenção quanto na segurança da informação. Arquiteturas monolíticas podem ser mais rápidas e baratas de desenvolver inicialmente, mas podem acarretar custos de manutenção mais altos e maiores riscos de segurança. Por outro lado, arquiteturas microkernel e em camadas podem exigir um investimento inicial maior, mas oferecem vantagens em termos de manutenção e segurança.

## Questão
Com base no texto sobre a estrutura de sistemas operacionais, analise como as diferentes arquiteturas (monolítica, microkernel e camadas) impactam o custo com a equipe de desenvolvimento e a segurança do sistema operacional. Em sua resposta, considere os seguintes pontos:
- Complexidade de implementação e manutenção
- Necessidade de especialização da equipe
- Potenciais vulnerabilidades de segurança
- Facilidade de atualização e correção de falhas

**Dica:** Utilize exemplos de sistemas operacionais reais que adotam essas arquiteturas para ilustrar sua análise.

**Copilot informa**: Essa questão incentiva os alunos a considerarem tanto os aspectos econômicos quanto os de segurança ao avaliar diferentes arquiteturas de sistemas operacionais.

# Resposta 2:

Arquiteturas monolíticas são rápidas e baratas de desenvolver, mas enfrentam desafios significativos em segurança e manutenção. Isso ocorre porque qualquer falha em um componente pode comprometer todo o sistema, resultando em altos custos de manutenção. Por outro lado, arquiteturas microkernel e em camadas oferecem maior modularidade e segurança, mas exigem maior especialização e investimento inicial.
A arquitetura monolítica, como o Linux, é inicialmente mais simples, com todos os componentes integrados em um único bloco de código. No entanto, sua vulnerabilidade em termos de segurança e a complexidade na implementação de atualizações tornam sua manutenção cara e trabalhosa.
Já a arquitetura microkernel, como o Minix, possui um custo inicial elevado devido à necessidade de criar um núcleo mínimo e separar os processos em módulos independentes. No entanto, sua alta segurança e modularidade permitem uma manutenção mais eficiente e menos onerosa a longo prazo.
Por fim, a arquitetura em camadas, como o Windows, apresenta um equilíbrio entre segurança e modularidade. Cada camada possui sua própria segurança, o que facilita a manutenção e atualização. Contudo, problemas podem surgir na comunicação entre as camadas, e o desenvolvimento inicial ainda demanda um investimento significativo.

# Questão 3. Introdução à Segurança de Sistemas Operacionais

## Texto informativo

A segurança de um sistema operacional é um aspecto crucial que visa proteger os recursos do sistema contra acessos não autorizados, ataques maliciosos e falhas. Um sistema operacional seguro deve garantir a integridade, confidencialidade e disponibilidade dos dados e serviços. Para alcançar esses objetivos, várias técnicas e mecanismos são implementados, incluindo:

1. **Controle de Acesso**: Define quem pode acessar o sistema e quais recursos podem ser utilizados. Isso é feito através de autenticação (verificação de identidade) e autorização (permissão de acesso).

2. **Criptografia**: Utilizada para proteger dados em trânsito e em repouso, garantindo que apenas usuários autorizados possam acessar informações sensíveis.

3. **Auditoria e Monitoramento**: Registra atividades do sistema para detectar e responder a comportamentos suspeitos ou anômalos.

4. **Isolamento de Processos**: Garante que os processos sejam executados em ambientes isolados, evitando que um processo comprometa a segurança de outro.

5. **Atualizações e Patches**: Manter o sistema operacional atualizado é essencial para corrigir vulnerabilidades conhecidas e proteger contra novas ameaças.


## Questão

Considerando os mecanismos de segurança discutidos, analise como a implementação de controles de acesso e criptografia pode impactar a performance e a usabilidade de um sistema operacional. Em sua resposta, aborde os seguintes pontos:
- Benefícios e desafios de cada mecanismo
- Impacto na experiência do usuário
- Exemplos de situações onde esses mecanismos são críticos

**Dica:** Pense em como esses mecanismos são aplicados em sistemas operacionais que você utiliza no dia a dia, como Windows, Linux ou macOS.

**Copilot informa**: Essa questão incentiva os alunos a refletirem sobre o equilíbrio entre segurança, performance e usabilidade, aplicando conceitos teóricos a contextos práticos.

# Resposta 3:
O controle de acesso e a criptografia são fundamentais para a segurança de sistemas operacionais, mas podem influenciar a performance e a usabilidade de diferentes formas.

## **Controle de Acesso**
- **Benefícios:** Limita acessos não autorizados, garantindo maior proteção ao sistema.
- **Impactos na usabilidade:** Pode frustrar usuários com autenticações frequentes ou rígidas. Quando bem implementado, como o uso de biometria, torna-se quase imperceptível. Entretanto, se mal otimizado, pode causar atrasos, especialmente em sistemas com grande volume de dados ou em dispositivos com hardware mais antigo.

## **Criptografia**
- **Benefícios:** Protege dados confidenciais contra acessos indevidos.
- **Impactos na performance:** A criptografia pode consumir muitos recursos, principalmente em dispositivos menos potentes. Configurações bem ajustadas podem minimizar esse impacto, garantindo que a usabilidade não seja prejudicada.

## **Aplicações em Situações Críticas**
1. **Ambientes corporativos:**  
   Controle de acesso e criptografia são indispensáveis para proteger informações confidenciais e atender a regulamentações, como o **GDPR**.

2. **Serviços online:**  
   Ferramentas como controle de acesso e criptografia (ex.: **HTTPS** e senhas protegidas) são essenciais para proteger os dados dos usuários em plataformas como redes sociais ou bancos.

# Questão 4. Custo de Processamento versus Algoritmo Ótimo de Escalonamento

## Texto informativo

O escalonamento de processos é uma função crítica de um sistema operacional, responsável por determinar a ordem em que os processos são executados pelo processador. O objetivo é maximizar a eficiência do sistema, garantindo que os recursos sejam utilizados de maneira justa e eficaz. No entanto, encontrar o algoritmo de escalonamento ótimo envolve um equilíbrio delicado entre o custo de processamento e a eficiência do escalonamento.

### Custo de Processamento

O custo de processamento refere-se ao tempo e aos recursos necessários para executar um algoritmo de escalonamento. Algoritmos mais complexos podem oferecer melhores resultados em termos de tempo de resposta e utilização do processador, mas também podem exigir mais recursos computacionais para tomar decisões de escalonamento. Isso pode incluir tempo de CPU, memória e outras operações de sistema.

### Algoritmo Ótimo de Escalonamento

Um algoritmo ótimo de escalonamento é aquele que maximiza a eficiência do sistema operacional, minimizando o tempo de espera dos processos, o tempo de resposta e o tempo de retorno. Alguns dos algoritmos de escalonamento mais comuns incluem:

- **First-Come, First-Served (FCFS)**: Simples e fácil de implementar, mas pode levar a longos tempos de espera para processos curtos.
- **Shortest Job Next (SJN)**: Minimiza o tempo médio de espera, mas pode ser difícil de implementar devido à necessidade de prever o tempo de execução dos processos.
- **Round Robin (RR)**: Oferece uma abordagem justa, atribuindo fatias de tempo iguais a todos os processos, mas pode resultar em maior sobrecarga de contexto.
- **Priority Scheduling**: Processos com maior prioridade são executados primeiro, mas pode levar à inanição de processos de baixa prioridade.

## Questão

Considerando os conceitos de custo de processamento e algoritmo ótimo de escalonamento, analise como diferentes algoritmos de escalonamento podem impactar a performance de um sistema operacional em termos de tempo de resposta, tempo de espera e utilização do processador. Em sua resposta, aborde os seguintes pontos:
- Vantagens e desvantagens de pelo menos dois algoritmos de escalonamento
- Impacto do custo de processamento na escolha do algoritmo
- Exemplos de situações onde um algoritmo pode ser preferível a outro

**Dica:** Pense em como esses algoritmos são aplicados em diferentes cenários, como sistemas de tempo real, servidores web e sistemas operacionais de uso geral.

**Copilot informa**: Essa questão incentiva os alunos a refletirem sobre a complexidade e os trade-offs envolvidos na escolha de um algoritmo de escalonamento, aplicando conceitos teóricos a contextos práticos.

# Resposta 4:

# Algoritmos de Escalonamento: FCFS e SJN

## **First-Come, First-Served (FCFS)**

- **Vantagens:**  
  - É simples de implementar, com baixo custo de processamento.  
  - É adequado para sistemas onde a ordem de chegada é essencial, como em filas de impressão.  

- **Desvantagens:**  
  - Pode sofrer com o *convoy effect*, onde processos pequenos ficam aguardando a finalização de processos maiores.  
  - Isso resulta em tempos de espera elevados para processos curtos.  

- **Uso:**  
  - Utilizado em filas de impressão ou sistemas de processamento simples.  

## **Shortest Job Next (SJN)**

- **Vantagens:**  
  - Reduz o tempo médio de espera ao priorizar processos mais curtos.  
  - Aumenta a eficiência do processador em sistemas de processamento em lote.  

- **Desvantagens:**  
  - Depende do conhecimento prévio do tempo de execução dos processos, o que pode ser inviável.  
  - Pode causar inanição de processos longos, que acabam sendo constantemente adiados.  

- **Uso:**  
  - Comumente aplicado em servidores de processamento em lote. 

# Questão 5. Aplicativo em python vs aplicativos em c

## Questão

Explique o caminho que as instruções seguem desde um aplicativo escrito em Python e um aplicativo escrito em linguagem C até serem executadas pelo hardware. Em sua resposta, considere os seguintes pontos:
- O papel do interpretador no caso do Python
- O processo de compilação no caso do C
- A interação entre o kernel do sistema operacional e os drivers de dispositivo
- A tradução final das instruções para o formato binário (0 e 1) executado pelo hardware

**Dica:** Compare e contraste os dois processos, destacando as principais diferenças e semelhanças na forma como as instruções são processadas e executadas.

**Copilot informa**: Essa questão incentiva os alunos a refletirem sobre os diferentes caminhos que as instruções seguem em linguagens interpretadas e compiladas, aplicando conceitos teóricos a contextos práticos.

# Resposta 5:

# Comparação de Execução: Python e C

## 1. **Aplicativo em Python**

### Características:  
Python é uma linguagem interpretada, o que significa que as instruções do código-fonte são lidas e executadas linha a linha por um interpretador, como o **CPython**.

### Caminho das Instruções:
1. O código Python é convertido em *bytecode* pelo interpretador, que é uma representação intermediária mais próxima do código de máquina.  
2. Esse *bytecode* é executado por uma máquina virtual, a **Python Virtual Machine (PVM)**.  
3. Durante a execução, o interpretador interage com o kernel do sistema operacional para solicitar recursos, como memória, processamento e entrada/saída.  
4. As instruções finais são traduzidas em código binário pelo kernel e pelos drivers e enviadas ao hardware.

### Impacto:
- O uso de um interpretador torna o Python mais lento na execução em comparação ao C, pois as instruções são processadas em tempo real.

## 2. **Aplicativo em C**

### Características:  
C é uma linguagem compilada, ou seja, o código-fonte é traduzido previamente para código de máquina por um compilador, como o **GCC**.

### Caminho das Instruções:
1. O código é transformado em código de máquina (binário executável) durante o processo de compilação, antes da execução.  
2. Quando executado, o binário interage diretamente com o kernel do sistema operacional, que gerencia os recursos do sistema.  
3. O kernel solicita a ajuda dos drivers de dispositivo para traduzir as instruções em comandos que o hardware compreenda.  
4. As instruções chegam ao processador já no formato binário (0s e 1s).  

### Impacto:
- Por já estar em código de máquina, aplicativos em C têm execução mais rápida e eficiente. Contudo, isso requer um passo extra de compilação.

## 3. **Interação com o Kernel e Drivers**

Em ambos os casos, o kernel do sistema operacional é responsável por:  
- Gerenciar os recursos do sistema, como memória e CPU.  
- Solicitar aos drivers de dispositivo que traduzam as instruções para comandos de hardware específicos.

### Diferença no Caminho:
- **Python:** Interage com o kernel através do interpretador e da máquina virtual.  
- **C:** Envia instruções diretamente como código de máquina já compilado.

## 4. **Semelhanças e Diferenças**

### Semelhanças:
- Ambos interagem com o kernel e os drivers para acessar recursos de hardware.  
- Ambos precisam traduzir suas instruções para binário, que é compreendido pelo hardware.

### Diferenças:
- Python usa um interpretador; C utiliza um compilador.  
- Python requer mais etapas em tempo de execução (interpretação, *bytecode*, execução pela PVM).  
- C gera código de máquina direto, resultando em maior eficiência.  
