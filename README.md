# ATIVIDADE-CONTEXTUALIZADA-01
*PRIMEIRA ATIVIDADE DA DISCIPLINA DE FUNDAMENTOS DA PROGRAMAÇÃO E DESENVOLVIMENTO Á NEUROENGENHARIA DE PROJETOS APLICADOS*

**1 -Descreva de forma narrativa (slide 27) com a maior quantidade de detalhes possível (Interação paciente máquina, setup, comunicação com hardware, o que estiver mais familiarizado) como se daria a utilização do Lokomat® e ZeroG®.**

Utilização do Lokomat®

Fazer amedição do tamanho da perna do paciente até o joelho;

Por a sinta desuporte alinhada com a coluna do paciente;

Paciente é posto no dipositivo; 

O fixar dispositivo na altura do quadril dopaciente;

Fixar suporte na altura nos tornozelos dopaciente;

Ajuste da amplitude do movimento;

Registro do peso e altura do paciente;

Definir velocidade do movimento;

Iniciar movimento;

Verificar no display grafico de amplitude de movimento e valocidade;

Verificar se paciente está estável com com a valocidade pré definida;

Se não, diminuir velocidade até o paciente ficar estável;

Se sim, verificar se paciente está sendo desafiado;

Se não,aumentar velocidade até o pacciente ser desafiado;

Se sim, manter movimento por um tempo determinado pelo reabilitador;

Analisar se o paciente concluiu o número necessário de reabilitações;

Se não, ir para a próxima sessão;

Se sim, encerrar reabilitação.

Utilização ZeroG®

**2 -A partir das informações colocadas no texto da questão 1, destacar o que seriam memória, processamento, entrada/saída:**

Entrada, seriam as informações de altura, peso, velocidade e amplitude do movimento.
Saída são, os gráficos de amplitude do movimento e e dados de avanço na reabilitação.
Memória, quando é feito o registro de velocidade, altura, peso, amplitude do movimento, dos gráficos e registro do número de seções de reabilitação.
Processamento, quado é feita a leitura do peso, altura, velocidade e amplitude do movimento. Também quando se inicia o meovimento, quando se verifica a 
estabilidade do paciente,quando se define um tempo para a repetição do movimento,quando é feita a análise se o paciente está sendo desafiado e quando se avalia em que etapa da reabilitação o paciente se enontra.

**3 -A partir das informações colocadas no texto da questão 1, destacar o que seriam as estruturas de repetição e de decisão:**

Etrutura de repetição são:

Ajuste de velocidade até o paciente encontrar estabilidade;
repetir o processo durante um tempo determinado;

Estrutura de decisão são:

Quando é feita a decisão sobre a estabilidade do paciente;
Quando se decide se o paciente está sendo desafiado;
Quando é questionado se o paciente realizou o número de reabilitações necessárias.




**4 -Converter as informações compiladas nas questões 1, 2 e 3 em um diagrama de blocos conforme apresentado no slide 28.**
file:///home/leticia.sousa/Downloads/fluxograma_aula_01.png![image](https://user-images.githubusercontent.com/110606748/183483447-2110d446-b31f-4558-92e0-f15c3839e26d.png)
 
**5 -Converter as informações compiladas nas questões 1, 2 e 3 em um pseudocódigo conforme apresentado no slide 30**

**Pseudocódico**


**algoritmo** EQUIPAMENTO_REABILITACAO

**VAR** tempo; **real**

**VAR** VELOCIDADE,AMPLITUDE, PESO, ALTURA; **float**;

**VAR** sim, não; **texto**;

**inicio;**

**leia** altura, peso, velocidade, amplitude;

< iniciar movimento >

**escreva** "grafico de amplitude e velocidade"

**escreva** "O paciente demonstra estabilidade?"

**leia** sim, não;

**Se** sim  **então**

< continuar reabilitação > 

**Senão**

 < Diminuir velocidade >
 
 **enquanto** < o paciente não demonstrar estabilidade>  **faça** < diminuir velocidade >

**escreva** "O paciente está sendo fisicamente desafiado?"

**leia** sim, não;

**Se** sim; **então**

< continuar reabilitação >

**senão**

< aumentar velocidade >

**escreva** "O paciente demonstra estabilidade?"

**leia** sim, não;

**Se** sim  **então**

< continuar reabilitação > 

**Senão**

 < Diminuir velocidade >
 
 **enquanto** < o paciente não demonstrar estabilidade>  **faça** < diminuir velocidade >

**escreva** "Mantaer movimento por quanto tempo?"

**leia** t;

**para** < t > **faça** < manter movimento >

 **escreva** "Concluiu o n° de sessões necessárias para reabilitação?"
 
 **leia** sim, não;
 
 **se** sim **então** < encerrar reabilitação >
 
 **senão** 
 
 <proxima sessão>
 
 **enquanto** < não concluir o n° de sessões de reabilitação necessária > **faça** < realizar processo novamente >
 
 **fim_se**
 
 **fim_enquanto**
 
 **fim_para**
 
 **fim**
 

 
 



