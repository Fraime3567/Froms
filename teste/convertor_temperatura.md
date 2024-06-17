# ProjetoES Conversor de temperaturas entre as várias escalas (C,F,K e R) 
Projeto de Engenharia de Software realizado pelo Grupo 1.
-Tomás Ribeiro
-Ismael 
-Nelson 

## Declaração do problema
Atualmente, muitos usuários precisam converter temperaturas entre diferentes escalas (Celsius, Fahrenheit, Kelvin e Rankine) para diversos fins, como estudos acadêmicos, trabalhos científicos, hobbies ou atividades cotidianas. A ausência de uma ferramenta simples e eficaz que permita essas conversões pode levar a erros e perda de tempo. Portanto, é necessário desenvolver um conversor de temperaturas que seja intuitivo, preciso e acessível.

## Requisitos Funcionais

- FR1: O sistema deve permitir a conversão de uma temperatura em Celsius (°C) para Fahrenheit (°F), Kelvin (K) e Rankine (°R).

- FR2: O sistema deve permitir a conversão de uma temperatura em Fahrenheit (°F) para Celsius (°C), Kelvin (K) e Rankine (°R).

- FR3: O sistema deve permitir a conversão de uma temperatura em Kelvin (K) para Celsius (°C), Fahrenheit (°F) e Rankine (°R).

- FR4: O sistema deve permitir a conversão de uma temperatura em Rankine (°R) para Celsius (°C), Fahrenheit (°F) e Kelvin (K).

- FR5: Não permitir valores negativos para Kelvin (K) e Rankine (R).

- FR6: Testes positivos e negativos para cada tipo de conversão.

- FR7: Testes para verificar a validade das temperaturas iniciais.

## Requisitos não funcionais e restrições de acordo com o projeto caso existam

# Requisitos não funcionais

- NFR1: O sistema deve ser capaz de realizar a conversão de temperaturas em menos de 1 segundo para garantir uma experiência de usuário fluida.

- NFR2: A saída dos resultados deve ser clara e legível, especificando a temperatura inicial, o tipo de conversão e o resultado da conversão.

- NFR3: O código deve ser modular para facilitar a manutenção e a adição de novas funcionalidades ou correções de bugs.

- NFR4: As funções de conversão devem ser claramente definidas e separadas, para permitir fácil atualização ou adição de novas conversões de temperatura.

- NFR5: O sistema deve ser capaz de lidar com entradas inválidas de forma graciosa, fornecendo mensagens de erro claras e evitando falhas inesperadas.

- NFR6: O sistema deve ser projetado de forma a permitir a adição de novas escalas de temperatura no futuro sem a necessidade de grandes refatorações.

# Restrições de acordo com o projeto

- As conversões de temperatura devem ser precisas até duas casas decimais.

- Não são permitidos valores negativos para as escalas Kelvin (K) e Rankine (R).

- Deve-se utilizar o framework unittest para a criação e execução dos testes unitários.

- Não é permitido o uso de bibliotecas externas para as conversões de temperatura. Todas as conversões devem ser implementadas manualmente.

## Atividades a desenvolver

# Identificando os atores:

- Usuário: 
    - Pessoa que utiliza o sistema para converter temperaturas entre diferentes escalas. 
    - Insere a temperatura e a escala desejada para a conversão, e recebe o resultado convertido.
- Testadores: 
    - Pessoas ou sistemas responsáveis por verificar a funcionalidade e a precisão do conversor de temperaturas. 
    - Executam testes unitários e de integração para garantir que as conversões estão corretas e que o sistema é robusto contra entradas inválidas.
- Suporte do Sistema: 
    - Equipa dedicada ao acompanhamento e manutenção do desempenho do sistema.

# Identificando os cenários:

- Cenário 1: Armazena o resultado de uma conversão e tem um método para imprimir o resultado.

- Cenário 2: Verificação se a temperatura fornecida é válida (não negativa para escalas Rankine e Kelvin). 

- Cenário 3: Implementação das funções de conversão para cada par de escalas.

- Cenário 4: Verificação de comportamento do sistema com entradas negativas para escalas que não aceitam valores negativos.

- Cenário 5: O código apresenta múltiplos testes onde "Temperatura(aa)" é utilizado, mas aa não está definido. Isso causará um erro de execução.

- Cenário 6: O teste "test_rankine_para_newton_negativo" utiliza uma conversão "R->N" que não está definida no dicionário de conversões do Conversor, levando a um erro de conversão não suportada.

- Cenário 7: O método "test_kelvin_para_celsius_valor_negativo" e "test_Rankine_para_celsius_valor_negativo" esperam uma conversão inválida, mas verificam com o valor "0", o que pode não ser a forma correta de capturar esse erro.

- Cenário 8: Ajustar os testes para capturar exceções esperadas quando há entradas inválidas.

- Cenário 9: Melhorar a validação no método "converter" para lidar com outros casos de entradas inválidas ou não suportadas.

[Tabela de Testes](https://github.com/pesobreiro/ES_exercicios/blob/master/projeto/grupo1/Imagens/testes.png)
![Tabela de Testes](https://github.com/pesobreiro/ES_exercicios/blob/master/projeto/grupo1/Imagens/testes.png)

## Identificar casos de uso

## Identificar relações entre casos de uso





## Diagrama casos de USO


## Diagrama de modelo de objetos


## Product backlog

- Criação de uma aplicação que permita a conversão precisa de temperaturas nas diferentes escalas.

## Sprints e Sprint Backlog

- Sprint FR1:
    - Escolha da arquitetura ideal para a realização do projeto.
    - Foi selecionada a arquitetura cliente servidor sendo esta a mais adequada para o projeto em questão.
- Sprint FR2:
    - Criação de um diagram de classes onde foram representadas as classes temperatura, opção, resultado e conversor.
- Sprint FR3:
    - Desenvolvimento do conversor de temperaturas em linguagem Python.
- Sprint FR4:
    - Fase de testes. 
    - Implementação de testes de modo a garantir que os resultados sejam corretos.
- Sprint FR5:
    - Implementação de correções caso sejam necessárias.
    - Testes finais.
- Sprint FR6:
    - Apresentação do produto ao cliente.

