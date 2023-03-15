
#
## Documento Arquitetural de Software - Aplicativo de Gestão de Horas
### Visão Geral do Sistema
O aplicativo de gestão de horas trabalhadas por projetos e funcionários tem como objetivo facilitar o controle e gestão de horas trabalhadas por funcionários em projetos. A aplicação permitirá que os funcionários registrem suas horas trabalhadas em tarefas específicas em projetos, bem como permitirá que os gerentes de projeto gerenciem e monitorem as horas trabalhadas por seus funcionários. O sistema também irá notificar os gerentes de projeto quando as horas trabalhadas ultrapassarem os limites definidos.

#
## Arquitetura do Sistema
O sistema seguirá uma arquitetura baseada em Modulos e microserviços, com as seguintes camadas:

### - Camada de Interface de Usuário
Esta camada será responsável pela interface do usuário, incluindo as telas de login, registro, adição de horas trabalhadas, listagem de horas trabalhadas e outras funcionalidades relacionadas ao usuário.

### - Camada de Casos de Uso
Esta camada será responsável pela lógica de negócios do aplicativo, incluindo a validação de horas trabalhadas, o controle de acesso e a notificação de gerentes de projeto.

### - Camada de Adaptadores
Esta camada será responsável pela comunicação entre as camadas de interface de usuário e casos de uso e a camada de banco de dados.

### - Camada de Banco de Dados
Esta camada será responsável pelo armazenamento dos dados do aplicativo, incluindo as informações de login dos usuários, horas trabalhadas, projetos e outras informações relevantes.

#
## Casos de uso
O aplicativo terá as seguintes funcionalidades:

### - Login de Funcionário
O sistema permitirá que os funcionários se registrem e façam login para acessar suas informações e registrar suas horas trabalhadas em projetos específicos.

### - Adicionar Horas Trabalhadas
Os funcionários poderão adicionar as horas trabalhadas em tarefas específicas em projetos.

### - Listar Horas Trabalhadas
Os funcionários poderão listar as horas trabalhadas em tarefas específicas em projetos.

### - Restrição de Acesso
O sistema permitirá que os usuários vejam apenas suas próprias informações e horas trabalhadas.

### - Login de Gestor
Os gerentes de projeto poderão fazer login para gerenciar e monitorar as horas trabalhadas por seus funcionários.

### - Validar Horas Trabalhadas
Os gerentes de projeto poderão validar as horas trabalhadas pelos funcionários em tarefas específicas em projetos.

### - Definir Horas Limite de Trabalho por Projeto
Os gerentes de projeto poderão definir as horas limite de trabalho por projeto.

### - Notificar Gerentes de Projeto
O sistema notificará automaticamente os gerentes de projeto quando as horas trabalhadas ultrapassarem os limites definidos.

### - Verificar Horas Disponíveis por Projeto
Os gerentes de projeto poderão verificar as horas disponíveis em cada projeto.

### - Horários Definidos para Cada Usuário e Projeto
O sistema permitirá que os gerentes de projeto definam horários específicos para cada usuário e projeto para limitar o tempo de trabalho.


### - Relatório e Busca de Horas Trabalhadas por Funcionários e Projetos
O sistema permitirá que os gerentes de projeto gerem relatórios e busquem horas trabalhadas por funcionários e projetos.

### - Considerações Finais
Este documento arquitetural de software tem como objetivo fornecer uma visão geral da arquitetura e funcionalidades do aplicativo de gestão de horas trabalhadas por projetos e funcionários. Ele não cobre todos os detalhes técnicos e de implementação, mas fornece uma estrutura básica para o desenvolvimento do sistema.

É importante ressaltar que este é apenas um exemplo simplificado e que um documento arquitetural de software completo deve incluir informações mais detalhadas sobre a arquitetura do sistema, tecnologias utilizadas, interfaces de programação de aplicativos (APIs), banco de dados, requisitos de segurança, entre outros aspectos relevantes.

Além disso, é recomendável que o documento arquitetural de software seja revisado e atualizado regularmente ao longo do ciclo de vida do projeto, à medida que novas funcionalidades são adicionadas e as necessidades do sistema evoluem.




## Limites e Regras
Deve-se utilizar Interfaces/Abstrações para que o código seja mais reutilizável e de fácil manutenção.

Sempre utilizar Injeção de Dependência para que o código seja mais reutilizável e de fácil manutenção.

Deve-se utilizar a camada de Repository para tratar e converter os dados, deixando a camada External para abstrair a camada de dados externa.
Deve-se  utilizar arquitetura Modular criando módulos para cada funcionalidade do aplicativo.

Para camada de Presentation deve ser utilizado o de State Management por funcionalidade, sendo que cada funcionalidade deve ter seu próprio módulo.

Utilizar testes unitários para garantir a qualidade do código.

***ATENÇÃO: COBERTURA DE TESTES AINDA DEVE SER DE DEFINIDA.

## Padrões de projeto
- Singleton
- Prototype (CopyWith)
- Factory
- Adapter

## Packages e plugins
 - Utilizar HTTP (Reqquisições HTTP)
 - Modular (Modularização, Injeção de Dependência, Gerenciamento de rotas)
 - MobX
 - MOCKITO

## Regras de nomenclaturas
-  Utilizar o  Arquitetura Gritando para nomes de Classes. Ex.: -> Entity -> PersonEntity
- Utilizar o padrão CamelCase para nomes de classes. Ex.: -> NomeDaClasse
- Utilizar snake_case para nomes de arquivos. Ex.:-> nome_do_arquivo.dart
- Utilizar o sufixo 'Impl' para classes que implementam uma interface. Ex.: HttpClienteImpl -> HttpClient
DioClientImpl -> HttpClient



_____________


ANOTAÇÃOES:<BR>
**Aplicativo  de gestão de horas trabalhadas por projetos e funcionários.
Buscando facilitar o controle de horas trabalhadas por funcionários e projetos.
Busca de horas trabalhadas por funcionários e projetos. 
Login por funcionário.
Adiconar horas trabalhadas por funcionário e projeto.
Listar horas trabalhadas por funcionário e projeto.
Periodo de trabalho, tarefa que ele desenvolveu.
Usuário pode ver somente suas horas trabalhadas e seus projetos
Gestor e Gerenciar horas trabalhadas por funcionários e projetos.
Validar horas trabalhadas por funcionários e projetos.
Login por gestor.
Projeto tem horas limites de trabalho.
Definir horas limite de trabalho por projeto.
Alterar hora após check ele desabilita  ao check, e a atarefa vai pra análise novamente.
Notificar que precisa aprovar horas trabalhadas por funcionários e projetos.
Gestor consegue verificar horas disponiveis por projeto.
Ter horarios definidos para cada usuário e projeto (limitar).
**
