<h2><a href= "https://www.mackenzie.br">Universidade Presbiteriana Mackenzie</a></h2>
<h3><a href= "https://www.mackenzie.br/graduacao/sao-paulo-higienopolis/sistemas-de-informacao">Sistemas de Informação</a></h3>


<font size="+12"><center>
# Escola do amanhã
</center></font>

>*Observação 1: A estrutura inicial deste documento é só um exemplo. O seu grupo deverá alterar esta estrutura de acordo com o que está sendo solicitado na disciplina.*

>*Observação 2: O índice abaixo não precisa ser editado se você utilizar o Visual Studio Code com a extensão **Markdown All in One**. Essa extensão atualiza o índice automaticamente quando o arquivo é salvo.*

**Conteúdo**

- [Autores](#nome-alunos)
- [Descrição do Projeto](#introdução-do-projeto)
- [Análise de Requisitos Funcionais e Não-Fucionais](#descrição-dos-requisitos)
- [Diagrama de Atividades](#diagrama-de-atividades) 
- [Diagrama de Casos de Uso](#diagrama-de-comportamento-atores)
- [Descrição dos Casos de Uso](#descrição-das-funcões)
- [Diagrama de Senquencia](#diagrama-de-ordem-interações)
- [Diagrama de Classes](#diagrama-orientado-objetos)
- [Diagrama de Estados](#diagrama-estrutura-componente)
- [Diagrama de Implantação](#diagrama-de-hardware-software)
- [Referências](#referências)


# Autores

* Pedro Augusto Yoshikuni
* Luiz Henrique Ribeiro Pulga
* Andrés Nunes Filipe

# Descrição do Projeto

* Este projeto visa desenvolver um sistema unificado de gestão de faltas para a Escola do amanhã, melhorando o controle e acompanhamento da presença de alunos. A acessibilidade é uma prioridade, e para isso, o sistema incluirá recursos como leitores de tela e compatibilidade com dispositivos de entrada alternativos para garantir o acesso a todos os usuários.
O sistema será projetado para ser intuitivo e eficiente no registro de faltas, além de incluir um módulo de geração de relatórios detalhados. Esses relatórios oferecerão análises detalhadas com filtros e buscas que podem ser configurados por variáveis como data, série escolar, turma, e professor.
Implementaremos também um sistema de notificações por e-mail, que garantirá que pais e responsáveis sejam informados de forma ágil sobre as ausências dos estudantes.

# Análise de Requisitos Funcionais e Não-Funcionais
# Requisitos Funcionais
Registro e Gestão de Faltas:

* Capacidade de registrar e monitorar a presença de alunos.
* Selecionar e identificar alunos que faltaram.
* Confirmar manualmente o envio das informações de faltas para o sistema.
  
Recursos de Acessibilidade:

* Compatibilidade com leitores de tela e dispositivos de entrada alternativos.
* Assegurar que todos os usuários possam acessar o sistema facilmente.

* Interface e Usabilidade:

* Desenvolvimento de uma interface intuitiva e fácil de usar.
* Capacidade de os alunos acessarem informações sobre suas próprias notas e faltas.

Relatórios e Análises:

* Geração de relatórios detalhados sobre faltas com filtros por data, série escolar, turma, e professor.
* Relatórios devem permitir análises detalhadas e configuráveis.

Sistema de Notificações:

* Envio automático de notificações por e-mail aos pais e responsáveis sobre as faltas dos alunos.
* Envio de alertas automáticos quando um aluno ultrapassa o limite de faltas permitido.

# Requisitos Não-Funcionais
Desempenho:

* Processamento rápido de um alto número de presenças.
* Tempo de resposta para as solicitações deve ser inferior a 1 segundo.

Segurança e Privacidade:

* Criptografia de dados de alunos e professores.
* Conformidade com a Lei Geral de Proteção de Dados (LGPD) e outras regulamentações de proteção de dados e privacidade.

Disponibilidade e Recuperação:

* Alta disponibilidade do sistema com minimização do tempo de inatividade.
* Realização de backups automáticos a cada 24 horas e capacidade de recuperação completa dos dados em caso de falha.

Escalabilidade e Confiabilidade:

* Capacidade de suportar um grande número de usuários simultaneamente, adequada para grandes escolas.
* Manutenção de operação constante e confiável, com alta disponibilidade.

# Diagrama de Atividades

![Diagrama de Atividades](https://github.com/user-attachments/assets/d922b0ee-146a-4a17-9ae4-86b2cef675fb)

# Diagrama de Casos de Uso
![Diagrama Casos de uso](https://github.com/user-attachments/assets/45705ab6-537d-4334-a613-cdbda444e226)

# Descrição dos Casos de Uso

![image](https://github.com/user-attachments/assets/5cfc9107-9df0-4ee1-9508-daa690f70262)

### Registrar Presença dos Estudantes:

**Agente**: Professor

**Descrição**: O professor faz o registro e acompanha a presença dos estudantes em uma determinada aula ou período.

**Fluxo**:
1. O professor acessa o sistema.
2. O sistema exibe a lista de turmas e alunos.
3. O professor seleciona a turma e marca os alunos presentes.
4. O sistema salva as presenças dos estudantes.

### Registrar Ausência do Aluno:

**Agente**: Professor

**Descrição**: O professor ou administrador seleciona os estudantes que estiveram ausentes para registro no sistema.

**Fluxo**:
1. O professor acessa o sistema.
2. O sistema exibe a lista de estudantes.
3. O professor seleciona o estudante que esteve ausente.
4. O sistema registra a ausência do aluno.

### Confirmar Envio das Ausências:

**Agente**: Professor

**Descrição**: O professor confirma o envio das informações de ausências ao sistema.

**Fluxo**:
1. O professor acessa a tela de confirmação de ausências.
2. O sistema exibe a lista de ausências pendentes.
3. O professor confirma as ausências.
4. O sistema atualiza o registro oficial das ausências.

### Acessibilidade do Sistema:

**Agente**: Todos os Usuários

**Descrição**: Garantir que o sistema seja acessível para todos os usuários, incluindo aqueles com necessidades especiais.

**Fluxo**:
1. O usuário acessa o sistema.
2. O sistema oferece suporte a leitores de tela e dispositivos de entrada alternativos.
3. O usuário navega pelo sistema sem obstáculos.

### Criação de Relatórios:

**Agente**: Professor/Administrador

**Descrição**: Gerar relatórios completos sobre as ausências dos estudantes.

**Fluxo**:
1. O professor ou administrador acessa a funcionalidade de relatórios.
2. O sistema exibe as opções de filtros (data, turma, professor).
3. O professor ou administrador seleciona os filtros desejados.
4. O sistema gera o relatório com base nos filtros escolhidos.
5. O usuário visualiza o relatório gerado.

### Envio de Notificação Automática:

**Agente**: Sistema

**Descrição**: Enviar notificações automáticas aos responsáveis quando o estudante ultrapassar o limite de ausências permitido.

**Fluxo**:
1. O sistema monitora diariamente o percentual de ausências dos estudantes.
2. O sistema identifica estudantes que excederam o limite de ausências.
3. O sistema busca os dados de contato dos responsáveis.
4. O sistema envia uma notificação por e-mail aos responsáveis.

### Processamento Ágil:

**Agente**: Sistema

**Descrição**: Assegurar um processamento ágil do registro de presenças dos estudantes.

**Fluxo**:
1. O sistema recebe os dados de presença.
2. O sistema processa e registra as informações instantaneamente.
3. O sistema confirma o processamento ao usuário.

### Backups Regulares:

**Agente**: Sistema

**Descrição**: Executar backups automáticos dos dados para garantir segurança e disponibilidade.

**Fluxo**:
1. O sistema inicia o processo de backup a cada 24 horas.
2. O sistema cria uma cópia dos dados e armazena de maneira segura.
3. O sistema registra a conclusão do backup e assegura a recuperação em caso de falhas.

# Diagrama de Sequência

![diagrama](https://github.com/user-attachments/assets/d87ccfb4-9167-42aa-abe6-d531849f8da1)

# Diagrama de Classes

![Diagrama_de_Classe](https://github.com/user-attachments/assets/02a0f34e-cd0a-4243-bb7a-bc12b9f81de5)


# Diagrama de Estados

![Diagrama_de_Estados](https://github.com/user-attachments/assets/ffdd267e-a0ba-4923-ace5-393485316a6a)


# Diagrama de Implantação

![Implantacao](https://github.com/user-attachments/assets/27d50236-256e-454c-87e7-c49615d21ff1)


# Referências

*&lt;Lista de referências&gt;*
