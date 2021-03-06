## Introdução

 Histórias de usuários é uma especificação de uma ou mais sentenças na linguagem de negócio ou cotidiana do usuário final ou usuário do sistema que captura o que um usuário faz ou necessita fazer como parte de sua função de trabalho.

## Metodologia

Para a elaboração das Histórias de Usuários foi contruído _card_, como é mostrado abaixo para a especificação da mesma.

| **ID** | **Nome** |
|:-------|:---------|
| USXX | Titulo da História |
| Descrição | _Eu, como_ XXX, _desejo_ XXX _para que eu possa_ XXX |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > XXX </br> > XXX </br> |

| Local | Data | Hora |
|-------|------|------|
| Google Hangouts | 14/10/2019 | 14:00 - 18:00 |

|Membros Participantes|
|---------------------|
|Francisco Heronildo|
|Lude Ribeiro|
|Luis Gustavo|
|Vitor Meireles|

## Épicos

**Legenda**:

* E: Épico.

| **Épico** | **Descrição** | **Features** |
|:----------|:-------------:|:-------------|
| E01 - Cadastro e Autenticação | Engloba toda a parte de cadastramento, login, lougout e chaves de acesso. | > Cadastro; </br> > Login; </br> > Logout. |
| E02 - Perfil | Engloba toda a parte de informações de usuário, configurações da aplicação, notificações. | > Perfil; </br> > Configurações Gerais; </br> > Avisos; </br> > Central de Ajuda |
| E03 - Cursos | Engloba toda a parte de aprendizagem do usuário. | > Curso; </br> > Aula; </br> > Seção. |
| E04 - Gameficação | Engloba toda a parte que mantém o usuário engajado. | > Ranking; </br> > Conquistas; </br> > Amigos; </br> > Ofensiva; </br> > Nível; </br> > Lingots; </br> > Loja. |
| E05 - Lucro | Engloba toda a parte de monetização do aplicativo. | > Duolingo Plus; </br> Anúncios. |

## Features

**Legenda**:

* US: Histórias de Usuários.

### Feature 1 - Cadastro e Autenticação

| **ID** | **Nome** |
|:-------|:---------|
| US01 | Elaborar formulário de interese de curso |
| Descrição | _Eu, como_ desenvolvedor, _desejo_ elaborar um formulário com os dados interesse de curso do usuário _para que eu possa_ efetuar o cadastro na aplicação |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > Qual idioma quero aprender </br> > Por que você está aprendendo um idioma </br> > Quantos minutos por dia eu posso estudar </br> > Começar do básico ou teste de nivelamento |

| **ID** | **Nome** |
|:-------|:---------|
| US02 | Elaborar formulário de informações pessoais |
| Descrição | _Eu, como_ desenvolvedor, _desejo_ elaborar um formulário com as informações pessoais do usuario _para que eu possa_ efetuar o cadastro na aplicação |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > Idade </br> > Nome </br> > E-mail </br> > Senha |

| **ID** | **Nome** |
|:-------|:---------|
| US03 | Validação do formulário de informações pessoais |
| Descrição | _Eu, como_ desenvolvedor, _desejo_ elaborar um processo de validação das informações pessoais do usuário _para que eu possa_ garantir a veracidade dos dados |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> **Idade** </br> > Apenas caracteres numéricos e inteiros </br> > Não pode ser negativo </br> >  Não pode ser maior que 149 </br> **Nome** </br> > Apenas caracteres do alfabeto </br> **Email** </br> > Tem que ser email válido segundo este [link](https://www.devmedia.com.br/validando-e-mail-em-inputs-html-com-javascript/26427) </br> > Não pode ser um email duplicado </br> **Senha** </br> > Tem que ter, no mínimo, 7 caracteres da Tabela ASCII |

### Feature 2 - Login

| **ID** | **Nome** |
|:-------|:---------|
| US04 | Fazer login |
| Descrição | _Eu, como_ usuário, _desejo_ fazer login na plataforma _para que eu possa_ entrar na minha conta e dar continuidade nas atividades da plataforma |
| Critérios  de Aceitação | Deve conter as seguintes opções: </br> > Implementar caixa de texto para inserir email e senha </br> > Opção de recuperar senha </br> > Opção de entrar com Google/Facebook </br> > Opção que redireciona para parte de criar cadastro </br> > Ter opção de visualizar senha inserida |

| **ID** | **Nome** |
|:-------|:---------|
| US05 | Validação do formulário de login |
| Descrição | _Eu, como_ desenvolvedor, _desejo_ elaborar um processo de validação das informações de login do usuário _para que eu possa_ autenticá-lo |
| Critérios de Aceitação | Deve conter as seguintes opções: **Email** </br> > Tem que ser email válido segundo este [link](https://www.devmedia.com.br/validando-e-mail-em-inputs-html-com-javascript/26427) </br> > Não pode ser um email já cadastrado </br> **Senha** </br> > Tem que ter, no mínimo, 7 caracteres da Tabela ASCII </br> A senha tem que corresponder a senha de castramento do usuário |

| **ID** | **Nome** |
|:-------|:---------|
| US59 | Boas vindas |
| Descrição | _Eu, como_ usuário, _desejo_ ser recebido no aplicativo com uma tela de boas vindas _para que eu possa_ me sentir mais animado |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > Após o usuário estar registra e fazer login <br> > Ao entrar no aplicativo deve ter uma tela de boas vindas |

### Feature 3 - Logout

| **ID** | **Nome** |
|:-------|:---------|
| US06 | Fazer lougout |
| Descrição | _Eu, como_ usuário, _desejo_ fazer lougout na plataforma _para que eu possa_ fazer o login em outra conta |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > Tem que ter uma opção para o usuário poder sair de sua conta |

### Feature 4 - Perfil

| **ID** | **Nome** |
|:-------|:---------|
| US07 | Alterar Avatar |
| Descrição | _Eu, como_ usuário, _desejo_ alterar o meu avatar _para que eu possa_ customizar meu perfil da forma que eu desejo |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > Botão com minha foto atual </br> > Poder trocar o avatar de duas formas: 1. Tirar uma foto; 2. Escolher uma foto da galeria; |

| **ID** | **Nome** |
|:-------|:---------|
| US08 | Alterar Nome |
| Descrição | _Eu, como_ usuário, _desejo_ alterar o meu nome _para que eu possa_ corrigir erros feitos no cadastro ou para customizar meu perfil |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > Caixa de texto editável com meu nome atual </br> > Se o nome digitado for válido segundo a [**US03**](#feature-1-cadastro-e-autenticacao), o nome deve ser alterado automaticamente |

| **ID** | **Nome** |
|:-------|:---------|
| US09 | Alterar Nome de Usuário |
| Descrição | _Eu, como_ usuário, _desejo_ alterar o meu nome de usuário _para que eu possa_ customizar meu perfil |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > Caixa de texto editável com meu nome de usuário atual </br> > Se o nome de usuário digitado for válido segundo a [**US03**](#feature-1-cadastro-e-autenticacao), o nome de usuário deve ser alterado automaticamente |

| **ID** | **Nome** |
|:-------|:---------|
| US10 | Alterar Senha |
| Descrição | _Eu, como_ usuário, _desejo_ alterar o minha senha _para que eu possa_ usar minha conta novamente caso esqueça a senha |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > Caixa de texto editável com a senha do usuário </br> > Se a senha digitada for válido segundo a [**US03**](#feature-1-cadastro-e-autenticacao), a senha deve ser alterado automaticamente |

| **ID** | **Nome** |
|:-------|:---------|
| US11 | Alterar Email |
| Descrição | _Eu, como_ usuário, _desejo_ alterar o meu email _para que eu possa_ corrigir erros feitos no cadastro ou para customizar meu perfil |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > Caixa de texto editável com o email do usuário </br> > Se o email digitado for válido segundo a [**US03**](#feature-1-cadastro-e-autenticacao), o email deve ser alterado automaticamente |

| **ID** | **Nome** |
|:-------|:---------|
| US55 | Alterar Meta Diária |
| Descrição | _Eu, como_ usuário, _desejo_ alterar minha meta diária de estudo _para que eu possa_ escolher uma meta que se seja mais adequada a minha rotina |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > Seguintes opções pré definidas de meta: 1. 5 minutos por dia <br> 2. 10 minutos por dia <br> 3. 15 minutos por dia <br> 4. 5 minutos por dia  |

### Feature 5 - Configurações Gerais

| **ID** | **Nome** |
|:-------|:---------|
| US12 | Ativar/Desativar Efeitos Sonoros |
| Descrição | _Eu, como_ usuário, _desejo_ alterar a utilização dos efeitos sonoros _para que eu possa_ fazer as aulas da forma que eu sentir mais confortável |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > Um [switch](https://developer.apple.com/design/human-interface-guidelines/ios/controls/switches/) que mostra se os efeitos sonoros estão ativados ou desativados </br> > Ao clicar no switch, ele deve alterar o comportamento atual dos efeitos sonoros |

| **ID** | **Nome** |
|:-------|:---------|
| US13 | Ativar/Desativar Mensagens Motivacionais |
| Descrição | _Eu, como_ usuário, _desejo_ alterar a utilização de mensagens motivacionais _para que eu possa_ fazer as aulas da forma que eu sentir mais confortável |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > Um [switch](https://developer.apple.com/design/human-interface-guidelines/ios/controls/switches/) que mostra se as mensagens motivacionais estão ativadas ou desativadas </br> > Ao clicar no switch, ele deve alterar o comportamento atual das mensagens motivacionais |

| **ID** | **Nome** |
|:-------|:---------|
| US14 | Ativar/Desativar Exercícios de Conversação |
| Descrição | _Eu, como_ usuário, _desejo_ alterar a utilização de exercícios de conversação _para que eu possa_ fazer apenas os tipos de aulas que desejo |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > Um [switch](https://developer.apple.com/design/human-interface-guidelines/ios/controls/switches/) que mostra se os exercícios de conversação estão ativados ou desativados </br> > Ao clicar no switch, ele deve alterar o comportamento atual dos exercícios de conversação |

| **ID** | **Nome** |
|:-------|:---------|
| US15 | Ativar/Desativar Exercícios de Compreensão |
| Descrição | _Eu, como_ usuário, _desejo_ alterar a utilização de exercícios de compreensão _para que eu possa_ fazer apenas os tipos de aulas que desejo |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > Um [switch](https://developer.apple.com/design/human-interface-guidelines/ios/controls/switches/) que mostra se os exercícios de compreensão estão ativados ou desativados </br> > Ao clicar no switch, ele deve alterar o comportamento atual dos exercícios de compreensão |

| **ID** | **Nome** |
|:-------|:---------|
| US16 | Ativar/Desativar Atualização de Recursos Utilizando Dados Móveis |
| Descrição | _Eu, como_ usuário, _desejo_ alterar a utilização de recursos utilizando dados móveis _para que eu possa_ gerenciar melhor a utilização dos dados móveis no aplicativo |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > Um [switch](https://developer.apple.com/design/human-interface-guidelines/ios/controls/switches/) que mostra se a atualização de recursos utilizando dados móveis </br> > Ao clicar no switch, ele deve alterar o comportamento da atualização de recursos utilizando dados móveis |

| **ID** | **Nome** |
|:-------|:---------|
| US17 | Restaurar Compras |
| Descrição | _Eu, como_ usuário, _desejo_ restaurar compras _para que eu possa_ utilizar os recursos por qual eu paguei |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > Ao clicar no botão de restaurar compras, todas os recursos obtidos através de compras que já foram feitas no aplicativo devem ficar disponíveis |

| **ID** | **Nome** |
|:-------|:---------|
| US18 | Restaurar Contatar o Suporte |
| Descrição | _Eu, como_ usuário, _desejo_ contatar o suporte do Duolingo _para que eu possa_ entrar em contato com alguém que possa resolver meus problemas ou tirar dúvidas |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > Ao clicar no botão de contatar suporte, devo ser redirecionado para algum aplicativo de email que eu tenha no meu celular |

| **ID** | **Nome** |
|:-------|:---------|
| US19 | Ativar/Desativar Estado de Conexão com Facebook |
| Descrição | _Eu, como_ usuário, _desejo_ alterar estado de conexão com Facebook _para que eu possa_ sincronizar meus amigos com os amigos do Facebook |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > Um [switch](https://developer.apple.com/design/human-interface-guidelines/ios/controls/switches/) que mostra o estado de conexão com o Facebook </br> > Ao clicar no switch, ele deve alterar o comportamento do estado de conexão com o Facebook |

| **ID** | **Nome** |
|:-------|:---------|
| US20 | Ativar/Desativar Estado de Conexão com Google |
| Descrição | _Eu, como_ usuário, _desejo_ alterar estado de conexão com Google _para que eu possa_ sincronizar meus amigos com os amigos do Google |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > Um [switch](https://developer.apple.com/design/human-interface-guidelines/ios/controls/switches/) que mostra o estado de conexão com o Google </br> > Ao clicar no switch, ele deve alterar o comportamento do estado de conexão com o Google |

### Feature 6 - Avisos

| **ID** | **Nome** |
|:-------|:---------|
| US21 | Ativar/Desativar Ligas |
| Descrição | _Eu, como_ usuário, _desejo_ a minha participação nas ligas _para que eu possa_ escolher progredir no aprendizado da maneira que me agradar mais |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > Um [switch](https://developer.apple.com/design/human-interface-guidelines/ios/controls/switches/) que mostra a minha participação nas ligas </br> > Ao clicar no switch, ele deve alterar o comportamento da minha participação nas ligas |

| **ID** | **Nome** |
|:-------|:---------|
| US22 | Ativar/Desativar Lembrete de Praticar |
| Descrição | _Eu, como_ usuário, _desejo_ alterar o lembrete de praticar _para que eu possa_ ser lembrado de praticar o(s) idioma(s) que estou aprendendo |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > Um [switch](https://developer.apple.com/design/human-interface-guidelines/ios/controls/switches/) que mostra o lembrete de praticar </br> > Ao clicar no switch, ele deve alterar o comportamento do lembrete de praticar |

| **ID** | **Nome** |
|:-------|:---------|
| US23 | Ativar/Desativar Atualização de Produtos |
| Descrição | _Eu, como_ usuário, _desejo_ alterar a atualização de produtos _para que eu possa_ gerenciar melhor a utilização de dados no App |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > Um [switch](https://developer.apple.com/design/human-interface-guidelines/ios/controls/switches/) que mostra a atualização de produtos </br> > Ao clicar no switch, ele deve alterar o comportamento da atualização de produtos |

| **ID** | **Nome** |
|:-------|:---------|
| US24 | Alterar Horário de Lembrete |
| Descrição | _Eu, como_ usuário, _desejo_ alterar o horário de lembrete _para que eu possa_ ser lembrado de praticar no melhor horário para mim |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > Um campo com os possíveis horários de lembrete </br> > Ao escolher um novo horário o horário de lembrete deve ser atualizado automaticamente |

| **ID** | **Nome** |
|:-------|:---------|
| US25 | Visualizar Termos |
| Descrição | _Eu, como_ usuário, _desejo_ visualizar os termos e condições de serviço _para que eu possa_ saber sobre a parte legal do aplicativo |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > Ao clicar no botão de Termos, devo ser redirecionado para uma página web que explique sobre os termos e condições de serviço do Duolingo |

| **ID** | **Nome** |
|:-------|:---------|
| US26 | Visualizar Privacidade |
| Descrição | _Eu, como_ usuário, _desejo_ visualizar a política de privacidade _para que eu possa_ saber sobre a parte legal do aplicativo |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > Ao clicar no botão de Privacidade, devo ser redirecionado para uma página web que explique sobre a política de privacidade do Duolingo |

| **ID** | **Nome** |
|:-------|:---------|
| US62 | Notificar usuário sobre as metas diárias |
| Descrição | _Eu, como_ usuário, _desejo_ receber notificações sobre as metas diárias _para que eu possa_ lembrar de realizá-las |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > Todos os dias devo receber a notificação ao menos uma vez, caso ainda não tenha completado minha meta diária |

### Feature 7 - Central de Ajuda

| **ID** | **Nome** |
|:-------|:---------|
| US27 | Visualizar Central de Ajuda |
| Descrição | _Eu, como_ usuário, _desejo_ visualizar a central de ajuda _para que eu possa_ aprender mais sobre o Duolingo e tirar alguma dúvida que eu tiver |
| Critérios de Aceitação | Deve conter as seguintes opções: </br> > Ao clicar no botão de Central de Ajuda, deve abrir uma nova tela que contenha as principais informações sobre o Duolingo e as perguntas e respostas mais frequentes |

### Feature 8 - Curso

| **ID** | **Nome** |
|:-------|:---------|
| US28 | Escolher um curso |
| Descrição | _Eu, como_ usuário, _desejo_ escolher qual curso de idioma fazer _para que eu possa_ aprender |
| Critérios de Aceitação| Deve contém as seguintes opções: </br> > Tem que haver uma lista de cursos para escolher </br> |

| **ID** | **Nome** |
|:-------|:---------|
| US29 | Adicionar um curso |
| Descrição | _Eu, como_ usuário, _desejo_ escolher outro idioma para cursar _para que eu possa_ ganhar mais conhecimento |
| Critérios de Aceitação| Deve contém as seguintes opções: </br> > Tem que haver uma lista de cursos para escolher </br> |

| **ID** | **Nome** |
|:-------|:---------|
| US60 | Voltar ao início do curso |
| Descrição | _Eu, como_ desenvolvedor, _desejo_ desejo fazer com que o usuário volte ao início do curso caso ele fique muito tempo sem utilizar o aplicativo _para que eu possa_ fazer com  que o curso reflita o conhecimento efetivo do usuário |
| Critérios de Aceitação| Deve contém as seguintes opções: </br> > Se o usuário ficar um longo período sem realizar nenhuma aula as aulas que ele já havia feito anteriormente devem ser bloqueadas e ele deve voltar ao início do curso |

### Feature 9 - Aula

| **ID** | **Nome** |
|:-------|:---------|
| US30 | Começar exercicios |
| Descrição | _Eu, como_ usuário, _desejo_ ter aulas a serem realizadas _para que eu possa_ aprender |
| Critérios de Aceitação | Deve contém as seguintes opções: </br> > Tem que haver uma lista categorizada de atividades exercicios  </br> > Tem que haver exercícios de conversação </br>  > Tem que haver exercícios de compreensão </br> |

| **ID** | **Nome** |
|:-------|:---------|
| US31 | Realizar exercícios de conversação |
| Descrição | _Eu, como_ usuário, _desejo_ fazer exercícios de conversação _para que eu possa_ melhor meu aprendizado |
| Critérios de Aceitação | Deve contém as seguintes opções: </br> > Tem que haver um botão para verificar a voz </br> |

| **ID** | **Nome** |
|:-------|:---------|
| US32 | Realizar exercícios de compreensão |
| Descrição | _Eu, como_ usuário, _desejo_ fazer exercícios de conversação _para que eu possa_ melhor meu aprendizado |
| Critérios de Aceitação | Deve contém as seguintes opções: </br> > Tem que haver exercícios de gramática </br> |

| **ID** | **Nome** |
|:-------|:---------|
| US33 | Progressão de exercícios |
| Descrição | _Eu, como_ usuário, _desejo_ fazer exercícios de forma gradual _para que eu possa_ aprender progredindo |
| Critérios de Aceitação | Deve contém as seguintes opções: </br> > Tem que haver exercícios categorizado por unidade </br> |

| **ID** | **Nome** |
|:-------|:---------|
| US56 | Incentivos e Dicas |
| Descrição | _Eu, como_ usuário, _desejo_ desejo receber incentivos e dicas durante a realização das aulas _para que eu possa_ me sentir mais motivado e engajado |
| Critérios de Aceitação | Deve contém as seguintes opções: </br> > Durante a realização das aulas eu devo receber incentivos e dicas de acordo com meus acertos nos exercícios |

| **ID** | **Nome** |
|:-------|:---------|
| US61 | Repetir exercícios |
| Descrição | _Eu, como_ desenvolvedor, _desejo_ repetir exercícios realizados _para que eu possa_ conseguir ajudar o usuário a fixar o conteúdo do idioma que ele está estudando |
| Critérios de Aceitação | Deve contém as seguintes opções: </br> > Durante a realização das aulas os exercícios devem se repetir |

### Feature 10 - Seção

| **ID** | **Nome** |
|:-------|:---------|
| US34 |  Aulas organizadas por seção |
| Descrição | _Eu, como_ usuário, _desejo_ ter aulas organizadas por seção _para que eu possa_ organizar os meus estudos de um novo idioma |
| Critérios de Aceitação | Deve contém as seguintes opções: </br> > Tem que haver aulas dividas por nível de dificuldade </br> > Realizar aulas da próxima seção ao concluir um teste nivelamento da seção anterior </br> > Realizar aulas da próxima seção ao concluir aulas da seção anterior </br> |

### Feature 11 - Ranking

| **ID** | **Nome** |
|:-------|:---------|
| US35   | Ver o Ranking |
| Descrição | _Eu como_ usuário _Desejo_ ter a seção de ranking _Para que eu possa_ visualizar meu rendimento em relação aos outros competidores da minha Liga |
| Críterios de Aceitação| Deve contém as seguintes opções: </br> > Tem que existir  pelo menos uma Liga para que exista a competição </br> > Deve concluir no minimo uma questão no dia para ter acesso ao Ranking </br>|

| **ID** | **Nome** |
|:-------|:---------|
| US36   | Subir de Liga |
| Descrição | _Eu como_ usuário _Desejo_ subir de liga _Para que eu possa_ me engajar mais com a competição |
| Críterios de Aceitação| Deve contém as seguintes opções: </br> > Tem que existir mais de uma liga para que se possa fazer um nivelamento maior </br> > Deve se ficar entre os N primeiros colocados para que seja promovido entre as ligas (número varia de acordo com a liga que o usuário participa) </br>|

| **ID** | **Nome** |
|:-------|:---------|
| US37   | Rebaixamento de Liga |
| Descrição | _Eu como_ desenvolvedor _Desejo_ criar um sistema de rebaixamento de liga _Para que eu possa_ evitar que o usuário deixe de se engaijar com o passar do tempo |
| Críterios de Aceitação| Deve contém as seguintes opções: </br> > Tem que existir mais de uma liga para que se possa fazer um nivelamento maior </br> > Caso o usuário fique entre as N ultimas posições (número varia de acordo com a liga do participante) </br>|

| **ID** | **Nome** |
|:-------|:---------|
| US57 | Aumentar pontuação |
| Descrição | _Eu, como_ usuário, _desejo_ que a cada aula finalizada minha pontuação aumentasse _para que eu possa_ subir no ranking |
| Critérios de Aceitação | Deve contém as seguintes opções: </br> > Tem que haver exercícios categorizado por unidade </br> |


### Feature 12 - Conquistas

| **ID** | **Nome** |
|:-------|:---------|
| US38   | Conquistas |
| Descrição | _Eu como_ usuário _Desejo_ ter uma seção de conquistas _Para que eu possa_ me sentir satisfeito ao usar mais o aplicativo  |
| Críterios de Aceitação| Deve contém as seguintes opções: </br> > Tem que existir mais de uma liga para que se possa fazer um nivelamento maior </br> > Deve se ficar entre os 20 primeiros colocados para que seja promovido entre as ligas </br>|

### Feature 13 - Amigos

| **ID** | **Nome** |
|:-------|:---------|
| US39   | Amigos |
| Descrição | _Eu como_ usuário _Desejo_ poder seguir meus amigos _Para que eu possa_ acompanhar o ritmo do meu amigo no curso  |
| Críterios de Aceitação| Deve contém as seguintes opções: </br> > Deve existir uma seção de amigos no aplicativo </br> > Deve ser possível seguir o amigo no aplicativo </br> > Deve ser possível ver o rendimento do amigo no aplicativo|

| **ID** | **Nome** |
|:-------|:---------|
| US54   | Compartilhar progresso |
| Descrição | _Eu como_ usuário _Desejo_ compartilhar meu progresso _Para que eu possa_ mostar aos meus amigos o quanto evolui  |
| Críterios de Aceitação| Deve contém as seguintes opções: </br> > Deve existir uma seção de configurações </br> > Deve ser possível compartilhar meu progresso através de uma chave gerada |


### Feature 14 - Ofensiva

| **ID** | **Nome** |
|:-------|:---------|
| US40   | Ofensiva |
| Descrição | _Eu como_ desenvolvedor _Desejo_ criar uma meta de engajamento chamada "ofensiva" _Para que eu possa_ dar ao usuário tenha mais motivação para usar o aplicativo todos os dias  |
| Críterios de Aceitação| Deve contém as seguintes opções: </br> > O usuário ganha ofensiva ao realizar uma tarefa no dia </br> > O usuário deve fazer tarefas todos os dias para manter a ofensiva </br> > Ao deixar de fazer lições no dia a ofensiva do usuário é perdida|

### Feature 15 - Nível

| **ID** | **Nome** |
|:-------|:---------|
| US41   | Seções |
| Descrição | _Eu como_ desenvolvedor _Desejo_ dividir os cursos em módulos (seções) bem definidas _Para que eu possa_ dar ao usuário uma melhor esperiencia ao fazer o curso  |
| Críterios de Aceitação| Deve contém as seguintes opções: </br> > O curso deve ser dividido em seções para que seja possível acompanhar o rendimento do aluno durante o curso </br> > Deve existir um teste de nivelamento para que o usuário possa pular as seções que ele já possui um conhecimento prévio|

| **ID** | **Nome** |
|:-------|:---------|
| US42   | Tópico |
| Descrição | _Eu como_ desenvolvedor _Desejo_ dividir os módulos do curso tópicos _Para que eu possa_ dar ao usuário um aprendizado seja ainda mais efetivo  |
| Críterios de Aceitação| Deve contém as seguintes opções: </br> > Cada seção do curso deve ter um número de tópicos adequado </br> > Ao concluir os Tópicos da seção anterior deve-se liberar a nova seção </br> > Cada tópico deve ser dividido em 5 níveis|

| **ID** | **Nome** |
|:-------|:---------|
| US58   | Teste de Nivelamento |
| Descrição | _Eu, como_ desenvolvedor, _desejo_ realizar um teste de nivelamento _para que eu possa_ fazer aulas do curso que sejam consistentes com meu conheicmneto |
| Críterios de Aceitação| Deve contém as seguintes opções: </br> > Na escolha de curso deve haver a opção de fazer um teste de nivelamento <br> > Após o teste aulas do curso deve ser liberadas de acordo com minha nota no teste; |

### Feature 16 - Lingots

| **ID** | **Nome** |
|:-------|:---------|
| US43     | Lingots por finalizar tarefas diárias |
| Descrição | _Eu como_ usuário _Desejo_ receber a moeda gamificada (Lingots) após completar minha tarefa diária _Para que eu possa_ me sentir mais satisfeito ao usar mais o aplicativo  |
| Críterios de Aceitação| Deve contém as seguintes opções: </br> > Tem que determinar a meta diária </br> > Deve-se chegar até ofinal das tarefas diárias de forma completa </br>|

| **ID** | **Nome** |
|:-------|:---------|
| US44     | Lingots por finalizar módulo de tarefas |
| Descrição | _Eu como_ usuário _Desejo_ receber a moeda gamificada (Lingots) após completar um módulo de tarefa  _Para que eu possa_ me sentir mais motivado ao usar o aplicativo e a aprender mais  |
| Críterios de Aceitação| Deve contém as seguintes opções: </br> > Tem que estar de acordo com o nível </br> > Deve-se chegar até ofinal das tarefas do módulo de forma completa </br>|

| **ID** | **Nome** |
|:-------|:---------|
| US45     | Lingots por finalizar a liga entre os três primeiros |
| Descrição | _Eu como_ usuário _Desejo_ receber a moeda gamificada (Lingots) após o final do período de uma liga terminando entre os três primeiros colocados _Para que eu possa_ me sentir mais motivado ao usar o aplicativo e a aprender mais  |
| Críterios de Aceitação| Deve contém as seguintes opções: </br> > Tem que estar de acordo com o nível da liga </br> > Deve-se chegar até ofinal do período da liga entre os três primeiros colocados </br>|

### Feature 17 - Loja

| **ID** | **Nome** |
|:-------|:---------|
| US46     | Compra de "Bloqueio de ofensivos" |
| Descrição | _Eu como_ usuário _Desejo_ comprar a skill por 10 Lingots para congelar danos cousados por tempo fora do app sem preaticar _Para que eu possa_ me sentir ainda em equidade para competir de forma gamificada com meus amigos e colegas  |
| Críterios de Aceitação| Deve contém as seguintes opções: </br> > Tem que ter Lingots sufientes </br>|

| **ID** | **Nome** |
|:-------|:---------|
| US47     | Compra de "Dobro ou nada" |
| Descrição | _Eu como_ usuário _Desejo_ comprar a skill por 5 Lingots para aumentar meus pontos xp _Para que eu possa_ me sentir mais motivado a continuar utilizando o app e ganhar pontos de experiência  |
| Críterios de Aceitação| Deve contém as seguintes opções: </br> > Tem que ter Lingots suficientes </br>|

| **ID** | **Nome** |
|:-------|:---------|
| US48     | Compra de Traje formal |
| Descrição | _Eu como_ usuário _Desejo_ comprar o traje formal por 20 Lingots para meu Duo ficar mais caracterizado _Para que eu possa_ sentir que o aplicativo está mais pessoal e traga mais motivação  |
| Críterios de Aceitação| Deve contém as seguintes opções: </br> > Tem que ter Lingots suficientes </br>|

| **ID** | **Nome** |
|:-------|:---------|
| US49     | Compra de Traje esportivo dourado |
| Descrição | _Eu como_ usuário _Desejo_ comprar o traje esportivo dourado por 30 Lingots para meu Duo ficar mais caracterizado _Para que o eu possa_ sentir que o aplicativo está mais pessoal e traga mais motivação  |
| Críterios de Aceitação| Deve contém as seguintes opções: </br> > Tem que ter Lingots suficientes </br>|

| **ID** | **Nome** |
|:-------|:---------|
| US50     | Compra de Traje super Duo |
| Descrição | _Eu como_ usuário _Desejo_ comprar o traje super Duo por 50 Lingots para meu Duo ficar mais caracterizado _Para que eu possa_ sentir que o aplicativo está mais pessoal e traga mais motivação  |
| Críterios de Aceitação| Deve contém as seguintes opções: </br> > Tem que ter Lingots suficientes </br>|

### Feature 18 - Duolingo Plus

| **ID** | **Nome** |
|:-------|:---------|
| US51     | Deixar o usuário testar a versão plus |
| Descrição | _Eu como_ desenvolvedor _Desejo_ dar a oportunidade do usuário testar a versão plus do aplicativo _Para que eu possa_ ver que tenho mais chance de usuários aderindo à versão paga do aplicativo  |
| Críterios de Aceitação| Deve contém as seguintes opções: </br> > Disponibilidade da versão por tem determindado </br> > Deve-se apresentar um pop-up de forma gratuita e convicente </br>|

| **ID** | **Nome** |
|:-------|:---------|
| US52     | Aderir ao Duolingo Plus |
| Descrição | _Eu como_ usuário _Desejo_ ter acesso à versão com exclusividades para ter melhor aproveito do aplicativo _Para que o eu possa_ me sinta mais satisfeito ao usar mais o aplicativo e a aprender de forma mais eficiente  |
| Críterios de Aceitação| Deve contém as seguintes opções: </br> > Tem que ser usuário que não recebeu ainda o tempo de teste da versão plus </br> > Deve-se pagar a taxa para utilizar a versão paga </br>|

### Feature 19 - Anúncios

| **ID** | **Nome** |
|:-------|:---------|
| US53     | Mostrar ao usuário que não é plus anúncios |
| Descrição | _Eu como_ desenvolvedor _Desejo_ mostrar ao meu usuário anúncios de propagandas _Para que eu possa_ ver que meu usuários têm motivos maiores para aderir a versão paga e eu posso desenvolvedor e empresa possa lucrar com propagandas  |
| Críterios de Aceitação| Deve contém as seguintes opções: </br> > Tem que ser usuário que não está no plano plus </br> > O usuário deve completar um ciclo de tarefas para que apareça o anúncio </br>|

## Referências

SERRANO, Maurício; SERRANO, Milene. Requisitos - Aula 15. 1º/2019. 46 slides. Material apresentado para a disciplina de Requisitos de Software no curso de Engenharia de Software da UnB, FGA.
