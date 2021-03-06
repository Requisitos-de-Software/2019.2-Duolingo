## Introdução

Casos de Uso são utilizados para descrever um conjunto de ações(casos de uso) que um sistema ou um conjunto de sistemas(sujeito) deve desempenhar em colaboração com um ou mais usuários externos ao sistema(ator). Cada caso de uso deverá prover algum resultado observável e de valor para os atores ou outros interessados do sistema.

## Metodologia

Para criação dos casos de uso foram identificados e analisados os documentos de elicitação de requisitos gerados na sprint anterior. A partir disso, foram feitos os casos de uso utilizando a ferramenta Astah.

## Casos de Uso & Especificação

### **Caso de Uso - Geral**

![Caso-de-Uso-Geral](../images/UseCase/uc-geral.png)

### **UC01 - Fazer Login**

![Caso-de-Uso-Login](../images/UseCase/uc-login.png)

| UC01                     | Fazer Login |
| --------------           |:----------- |
| **Versão**               | Atual: 1.0 (25/09) <br> Anterior: -- |
| **Autor(es)**            | Luis Gustavo e Vitor Alves |
| **Descrição**            | Fazer Login no Duolingo |
| **Ator(es)**             | > Usuário <br> > Duolingo |
| **Pré condições**        | > Usuário estar deslogado no aplicativo |
| **Fluxo principal**      | > Usuário acessa o Duolingo <br> > Usuário clica no botão "Já tenho uma conta" <br> > Usuário insere os dados de email ou nome de usuário e senha <br> > Usuário clica no botão "Entrar" <br> > Os dados de login são autenticados |
| **Fluxos alternativos**  | **Fluxo Alternativo 1 - Cadastro:** <br> > Usuário acessa o Duolingo <br> > Usuário clica no botão "Início" <br> > Usuário segue os passos para realizar o [cadastro](#uc02-cadastrar-usuario) <br> > O usuário é logado automaticamente ao criar seu cadastro |
| **Fluxos de exceção**    |  **Fluxo de Exceção 1 - Dados de Login inválidos:** <br> > Aplicativo apresentar uma mensagem de erro avisando que não foi possível fazer o Login <br> <br> **Fluxo de Excecão 2 - Usuário esqueceu a senha:** <br> > Usuário clica no botão "Esqueci a Senha" <br> > Usuário insere email para recuperar a senha <br> > É feita uma validação para identificar se existe um usuário cadastrado com aquele email <br> > É enviado um email para o usuário redefinir sua senha |
| **Pós condições**        | Usuário fica logado no Duolingo e é direcionado para a aba de aulas |
| **Rastreabilidade**      | INT02 |

### **UC02 - Cadastrar Usuário**

![Caso-de-Uso-Cadastro](../images/UseCase/uc-cadastro.png)

| UC02                     | Cadastrar usuário |
| --------------           |:----------- |
| **Versão**               | Atual: 1.0 (26/09) <br> Anterior: -- |
| **Autor(es)**            | Luis Gustavo e Vitor Alves |
| **Descrição**            | Criar cadastro para um usuário |
| **Ator(es)**             | > Usuário <br> > Duolingo |
| **Pré condições**        | > Usuário estar deslogado no aplicativo |
| **Fluxo principal**      | > Usuário acessa o Duolingo <br> > Usuário clica no botão "Início" <br> > Usuário insere do curso(idioma que deseja apreder, motivo de estar aprendendo um idioma, meta(minutos de estudo por dia) e caminho(aprender do início ou fazer um teste de nivelamento)) <br> > Usuário segue os passos para realizar uma [aula](#uc05-aulas) <br> > Usuário insere as informações de perfil(idade, nome, email e senha) <br> > Os dados de cadastro são autenticados |
| **Fluxos alternativos**  | **Fluxo Alternativo 1 - Usuário realiza mais aulas:** <br> > Usuário acessa o Duolingo <br> > Usuário clica no botão "Início" <br> > > Usuário insere do curso(idioma que deseja apreder, motivo de estar aprendendo um idioma, meta(minutos de estudo por dia) e caminho(aprender do início ou fazer um teste de nivelamento)) <br> > Usuário segue os passos para realizar uma [aula](#uc05-aulas) <br> > Usuário clica no botão "Depois" <br> > > Usuário segue os passos para realizar uma [aula](#uc05-aulas) <br> > Usuário clica no botão "Criar Perfil" <br> > Usuário segue os passos para realizar uma [aula](#uc05-aulas) <br> > Usuário insere as informações de perfil(idade, nome, email e senha) <br> > Os dados de cadastro são autenticados |
| **Fluxos de exceção**    |  **Fluxo de Exceção 1 - Email já cadastrado:** <br> > Aplicativo mostra que já existe um usuário cadastrado com esse email e fornece o campo de senha para fazer login nessa conta já cadastrada <br> <br> **Fluxo de Excecão 2 - Email inválido:** <br> > Aplicativo apresenta uma mensagem de erro pedindo para o usuário inserir um email válido <br> <br> **Fluxo de Excecão 3 - Idade inválida, negativa ou muito alta:** <br> > Aplicativo apresenta uma mensagem de erro pedindo para o usuário inserir uma idade válida |
| **Pós condições**        | Usuário fica logado no Duolingo e é direcionado para a aba de aulas |
| **Rastreabilidade**      | INT02 |

### **UC03 - Visualizar Perfil**

![Caso-de-Uso-Perfil](../images/UseCase/uc-perfil-v2.png)

| UC03                     |  |
| --------------           |:----------- |
| **Versão**               | Atual: 2.0 (04/11) <br> Anterior: 1.0 (28/09) |
| **Autor(es)**            | Atual: Luis Gustavo <br> Anterior: Francisco Heronildo e Vitor Meireles |
| **Descrição**            | Acessar Pefil do Duolingo |
| **Ator(es)**             | > Usuário <br> > Duolingo |
| **Pré condições**        | > Usuário estar [cadastrado](#uc02-cadastrar-usuario) no aplicativo |
| **Fluxo principal**      | > Usuário acessa o Duolingo <br> > Usuário clica no ícone do seu "Perfil" <br>|
| **Fluxos alternativos**  | -- |
| **Fluxos de exceção**    | **Fluxo de Exceção 1 - Não há conexão com a Internet:** <br> > Usuário acessa o Duolingo <br> > Usuário clica no ícone do seu "Perfil" <br> > Aplicativo apresenta um alerta dizendo que não há conexão com a internet |
| **Pós condições**        | Usuário fica logado no Duolingo e consegue acompanhar os XP's que o amigo adquire |
| **Rastreabilidade**      | AP09 |

### **UC04 - Seguir Amigos**

![Caso-de-Uso-Perfil](../images/UseCase/uc-amigos-v2.png)

| UC04                     |  |
| --------------           |:----------- |
| **Versão**               | Atual: 2.0 (04/11) <br> Anterior: 1.0 (28/09) |
| **Autor(es)**            | Atual: Luis Gustavo <br> Anterior: Francisco Heronildo e Vitor Meireles |
| **Descrição**            | Seguir Amigos |
| **Ator(es)**             | > Usuário <br> > Duolingo |
| **Pré condições**        | > Usuário estar [cadastrado](#uc02-cadastrar-usuario) no aplicativo |
| **Fluxo principal**      | > Usuário acessa o Duolingo <br> > Usuário clica no ícone do seu "Perfil" <br> > Usuário acessar a aba "Amigos" <br> > Usuário clica em "Adicionar" <br> > Usuário clica em "Procurar Amigo" <br> > Usuário digita o nome do usuário que quer encontar <br> > Usuário clica em "Seguir" |
| **Fluxos alternativos**  | **Fluxo Alternativo 1 - Adicionar Amigos:** > Usuário acessa o Duolingo <br> > Usuário clica no ícone do seu "Perfil" <br> > Usuário clica na aba "Amigos" <br> > Usuário clica em "Adicionar" <br> > Usuário clica em "Convidar um amigo" <br> > Usuário insere o email do amigo <br> <br> **Fluxo Alternativo 2 - Adicionar Amigos pelo site:** > Usuário acessa o Duolingo <br> > Usuário clica em "Enviar Convite" <br> > Usuário insere o email do amigo <br> <br>**Fluxo Alternativo 3 - Adicionar Amigos pelo Facebook:** > Usuário acessa o Duolingo <br> > Usuário clica em "Encontre Amigos no Facebook" <br> > Autorize o Facebook <br> <br> **Fluxo Alternativo 4 - Convidar Amigos** <br> > Usuário clica no ícone do seu "Perfil" <br> > Usuário clica na aba "Amigos" <br> > Usuário clica em "Adicionar" <br> > Usuário clica em "Convidar um amigo" <br> Usuário enviar um convite através de alguma rede social ou aplicativo de mensagem |
| **Fluxos de exceção**    | **Fluxo de Exceção 1 - Nome ou email inválido:** <br> > Aplicativo apresenta uma mensagem de erro avisando que não foi possível encontrar o usuário desejado <br> <br> **Fluxo de Exceção 1 - Não há conexão com a internet:** <br> > Aplicativo apresenta um alerta avisando que não há conexão com a internet |
| **Pós condições**        | Usuário fica logado no Duolingo e consegue acompanhar os XP's que o amigo adquire |
| **Rastreabilidade**      | AD04 |

### **UC05 - Selecionar Curso**

![Caso-de-Uso-Cursos](../images/UseCase/uc-cursos-v2.png)

| UC05                     | Selecionar Curso |
| --------------           |:----------- |
| **Versão**               | Atual: 2.0 (04/11) <br> Anterior: 1.0 (29/09) |
| **Autor(es)**            | Atuak: Luis Gustavo <br> Anterior: Francisco Heronildo e Vitor Meireles |
| **Descrição**            | Usuário escolher o idioma que quer aprender |
| **Ator(es)**             | > Usuário |
| **Pré condições**        | > Usuário estar logado no aplicativo |
| **Fluxo principal**      | > Usuário acessa o Duolingo <br> > Usuário clica na bandeira do curso atual <br> > Usuário clica no curso que deseja |
| **Fluxos alternativos**  | **Fluxo Alternativo 1 - Escolher mais cursos:** <br> > Usuário acessa o Duolingo <br> > Usuário clica no ícone da bandeira de seu curso <br> > Usuário clica em "Curso" ou "Adicionar um novo curso" <br> > Usuário adiciona outro curso |
| **Fluxos de exceção**    | **Fluxo de Exceção 1 - Não há conexão com a internet** <br> > Usuário acessa o Duolingo <br> > Usuário clica na bandeira do curso atual <br> > Aplicativo apresenta uma alerta dizendo que não é possível selecionar cursos offline |
| **Pós condições**        | Usuário é direcionado para a aba de aulas |
| **Rastreabilidade**      | Q01 |

### **UC06 - Realizar Aula**

![Caso-de-Uso-Aulas](../images/UseCase/uc-aulas-v2.png)

| UC06                     | Aulas |
| --------------           |:----------- |
| **Versão**               | Atual: 2.0 (09/11) <br> Anterior: 1.0 (29/09) |
| **Autor(es)**            | Atual: Luis Gustavo <br> Anterior: Francisco Heronildo e Vitor Meireles |
| **Descrição**            | Usuário deve escolher e realizar uma aula |
| **Ator(es)**             | > Usuário |
| **Pré condições**        | > Usuário estar [cadastrado](#uc02-cadastrar-usuario) no aplicativo |
| **Fluxo principal**      | > Usuário acessa o Duolingo <br> > Usuário clica na aula disponível do [curso](#uc04-escolher-cursos) escolhido <br> > Usuário clica em "Começar" <br> > E as lições são apresentadas progressivamente |
| **Fluxos alternativos**  | --- |
| **Fluxos de exceção**    | **Fluxo de Exceção 1 - Não há conexão com a internet** <br> > Usuário acessa o Duolingo <br> > Usuário clica na aula disponível do [curso](#uc04-escolher-cursos) escolhido <br> > Usuário clica em "Começar" <br> > Aplicativo apresenta uma alerta dizendo que não é possível selecionar cursos offline |
| **Pós condições**        | Usuário pode abandonar a aula e retomar depois |
| **Rastreabilidade**      | ENT03 |

### **UC07 - Acessar Loja**

![Caso-de-Uso-Loja](../images/UseCase/uc-loja-v2.png)

| UC07                     | Loja |
| --------------           |:----------- |
| **Versão**               | Atual: 2.0 (09/11) <br> Anterior: 1.0 (30/09) |
| **Autor(es)**            | Atual: Luis Gustavo <br> Anterior: Brian Lui e Lude Ribeiro |
| **Descrição**            | Usuário vai acessar a loja |
| **Ator(es)**             | > Usuário |
| **Pré condições**        | > Usuário estar [cadastrado](#uc02-cadastrar-usuario) no aplicativo |
| **Fluxo principal**      | > Usuário acessa o Duolingo <br> > Usuário clica no botão "Shop" |
| **Fluxos alternativos**  | **Fluxo Alternativo 1 - Usuário compra Super Poder:** <br> > Usuário acessa o Duolingo <br> > Usuário clica no botão "Shop" <br> > Comprar Super Poder <br> Usuário Clica em "Adquirir" <br> <br> **Fluxo Alternativo 2 - Usuário compra Traje:** <br> > Usuário acessa o Duolingo <br> > Usuário clica no botão "Shop" <br> > Comprar Traje <br> Usuário Clica em "Adquirir" <br> <br> **Fluxo Alternativo 3 - Usuário compra Unidade Bônus:** <br> > Usuário acessa o Duolingo <br> > Usuário clica no botão "Shop" <br> > Comprar Unidade Bônus <br> Usuário Clica em "Adquirir" <br> <br> |
| **Fluxos de exceção**    | **Fluxo de Excessão 1 - Não há conexão com a internet:** <br> > Usuário acessa o Duolingo <br> > Usuário clica no botão "Shop" <br> > Comprar Algo da Loja <br> Aparece um alerta dizendo que não há conexão com a internet <br> <br> **Fluxo de Excessão 1 - Não tem moedas suficiente:** <br> > Usuário acessa o Duolingo <br> > Usuário clica no botão "Shop" <br> > Comprar Algo da Loja <br> Aparece um alerta dizendo que o usuário não consegue comprar o item pois não tem moedas suficientes |
| **Pós condições**        | Usuário recebe o item que comprou |
| **Rastreabilidade**      | ENT11 |

### **UC08 - Ranking**

![Caso-de-Uso-Ranking](../images/UseCase/uc-ranking-v2.png)

| UC08                     | Ranking |
| --------------           |:----------- |
| **Versão**               | Atual: 2.0 (09/11) <br> Anterior: 1.0 (30/09) |
| **Autor(es)**            | Atual: Luis Gustavo <br> Anterior: Brian Lui e Lude Ribeiro |
| **Descrição**            | Usuário irá ver a sua posição no Ranking |
| **Ator(es)**             | > Usuário |
| **Pré condições**        | > Usuário estar [cadastrado](#uc02-cadastrar-usuario) no aplicativo |
| **Fluxo principal**      | > Usuário acessa o Duolingo <br> > Usuário clica no botão "Leaderboards" <br> > E é apresentado uma tabela do Ranking <br> |
| **Fluxos alternativos**  | --- |
| **Fluxos de exceção**    | **Fluxo de Exceção 1 - Menos de 10 Lições Completas:** <br> > Aplicativo apresentar uma mensagem avisando para o Usuário completar no mínimo 10 Lições para começar a competir e assim fazer parte do Ranking <br> <br> **Fluxo de Exceção 1 - Menos de 10 Lições Completas:** <br> > Aplicativo apresentar uma mensagem avisando para o Usuário que não há conexão com a internet |
| **Pós condições**        | Usuário irá ver o Ranking |
| **Rastreabilidade**      | ST06 |

### **UC09 - Configurações**

![Caso-de-Uso-Configuracoes](../images/UseCase/uc-configuracoes-v2.png)

| UC09                     | Configurações |
| --------------           |:----------- |
| **Versão**               | Atual: 2.0 (09/11) <br> Anterior: 1.0 (30/09) |
| **Autor(es)**            | Atual: Luis Gustavo <br> Anterior: Brian Lui e Lude Ribeiro |
| **Descrição**            | Usuário irá fazer alguma configuração no Duolingo |
| **Ator(es)**             | > Usuário |
| **Pré condições**        | > Usuário estar [cadastrado](#uc02-cadastrar-usuario) no aplicativo |
| **Fluxo principal**      | > Usuário acessa o Duolingo <br> > Usuário clica no botão "Perfil" <br> > Usuário clica em "Configurações" <br> > E serão apresentadas as possíveis configurações <br> > Usuário irá alterar dados do Perfil <br> |
| **Fluxos alternativos**  | **Fluxo Alternativo 1 - Alterar Objetivos Diários:** > Usuário acessa o Duolingo <br> > Usuário clica no botão "Perfil" <br> > Usuário clica em "Configurações" <br> > E serão apresentadas as possíveis configurações <br> > Usuário irá alterar dados dos Objetivos Diários <br>**Fluxo Alternativo 2 - Alterar dados Gerais:** > Usuário acessa o Duolingo <br> > Usuário clica no botão "Perfil" <br> > Usuário clica em "Configurações" <br> > E serão apresentadas as possíveis configurações <br> > Usuário irá alterar dados gerais <br>**Fluxo Alternativo 3 - Alterar dados de Acessibilidade:** > Usuário acessa o Duolingo <br> > Usuário clica no botão "Perfil" <br> > Usuário clica em "Configurações" <br> > E serão apresentadas as possíveis configurações <br> > Usuário irá alterar dados de Acessibilidade <br>**Fluxo Alternativo 4 - Alterar dados de Notificações:** > Usuário acessa o Duolingo <br> > Usuário clica no botão "Perfil" <br> > Usuário clica em "Configurações" <br> > E serão apresentadas as possíveis configurações <br> > Usuário irá alterar dados de Notificações <br> |
| **Fluxos de exceção**    | --- |
| **Pós condições**        | Configurações são realizadas |
| **Rastreabilidade**      | Q06 |

|  | Casos de Uso |
|--|--------------|
| **Versão** | Atual: 2.0 (09/11/2019) <br> Atual: [1.0](https://drive.google.com/drive/folders/1x2NCXOnoE1u1etT4E-kZ68jcE5iW2a6X?usp=sharing) (30/09/2019) |
| **Descrição** | Especificação dos Requisitos Funcionais  |


## Referências

SERRANO, Maurício; SERRANO, Milene. Requisitos - Aula 11. 1º/2019. 40 slides. Material apresentado para a disciplina de Requisitos de Software no curso de Engenharia de Software da UnB, FGA.
