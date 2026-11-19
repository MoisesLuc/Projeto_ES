## Descrição do Projeto

O DigiBus é uma plataforma digital para linhas rodoviárias que atende os moradores
da região do Seridó, desde adolescentes até idosos que viajam com frequência entre
cidades. O objetivo principal é facilitar a compra e o cancelamento de passagens e ajudar
os passageiros a planejarem a viagem antes do embarque. Com o sistema, o usuário
poderá acompanhar a localização dos ônibus, ver os horários previstos de chegada e
partida e receber avisos sobre atrasos ou cancelamentos.
O projeto busca resolver problemas como a superlotação dos ônibus e a falta de aviso
quando há atrasos ou cancelamentos. Para a empresa, a plataforma também ajuda no
gerenciamento da frota, já que o número de passagens vendidas permite organizar melhor
os ônibus de cada linha, além de gerar relatórios mensais e anuais.

## Equipe e Definição de Papéis

| Membro     |     Papel   |   E-mail   |
| ---------  | ----------- | ---------- |
Moisés Lucena de Oliveira    | Aluno  | moisesbrats98@gmail.com

### Matriz de Competências

| Membro     |     Competências   |
| ---------  | ----------- |
Moisés    | Desenvolvedor Python, PostgreSQL |

## Perfis dos Usuários

O sistema poderá ser utilizado por diversos usuários. Temos os seguintes perfis/atores:

| Perfil                                 | Descrição   |
| ---------                              | ----------- |
Administrador | Gerenciar o escopo da empresa cadastrada no sistema e registrar outros funcionários, frota de ônibus, rotas, horários e datas, etc.
Atendente de Bilheteria | Ficará responsável por registrar as compras físicas de passagem no sistema, informar sobre os horários e datas, atualizar o sistema sobre possíveis atrasos, etc.
Cliente Final | Poderá visualizar os ônibus disponíveis conforme estes forem sendo cadastrados, os horários e datas, as rotas, quantidade de passageiros, etc

## Requisitos Funcionais

| Requisito | Descrição | Ator |
|---|---|---|
| RF01 – Autenticação de usuários | Permite login e logout com e-mail e senha. Cada tipo de usuário só pode acessar as telas e funções do seu perfil. | Todos |
| RF02 – Cadastro de clientes | Criar conta informando os dados básicos, como nome, e-mail, telefone e senha, além de poder editar esses dados depois. | Cliente Final |
| RF03 – Gerenciamento de funcionários | Cadastrar, editar e desativar os funcionários da empresa, definindo se cada um é administrador ou atendente de bilheteria. | Administrador |
| RF04 – Gerenciamento da frota | Cadastrar, editar e remover os ônibus da frota, informando dados como placa, modelo e capacidade de passageiros. | Administrador |
| RF05 – Gerenciamento de rotas | Cadastrar, editar e remover as rotas, informando a cidade de origem, a cidade de destino e as paradas, caso existam. | Administrador |
| RF06 – Gerenciamento de viagens | Cadastrar e alterar as viagens, definindo a rota, o ônibus, a data, o horário de partida e o horário previsto de chegada. | Administrador |
| RF07 – Consulta de viagens | Visualizar os ônibus disponíveis, com suas rotas, datas e horários, conforme forem cadastrados no sistema. Também deve ser possível buscar por cidade de origem, destino e data. | Atendente, Cliente Final |
| RF08 – Consulta de lotação | Mostrar a quantidade de passageiros e de lugares livres em cada viagem, para o cliente e para os funcionários. | Atendente, Cliente Final |
| RF09 – Registro de compras presenciais | Registrar no sistema as passagens vendidas no balcão, informando a viagem e os dados do passageiro. O sistema deve impedir a venda quando o ônibus estiver lotado. | Atendente |
| RF12 – Atualização de atrasos e cancelamentos | Registrar atrasos e cancelamentos de uma viagem, informando o novo horário previsto ou o motivo. | Atendente |

## Requisitos não-Funcionais

| Requisito | Descrição |
|---|---|
| RNF01 – Tecnologia | O sistema será desenvolvido como plataforma web usando o framework Django, com banco de dados PostgreSQL hospedado em nuvem. |
| RNF02 – Usabilidade | A interface deve ser simples e fácil de usar, com poucos passos para realizar as tarefas principais, já que o sistema será usado por pessoas de várias idades e níveis de experiência. |
| RNF03 – Acessibilidade | As telas devem usar fontes legíveis, botões grandes e bom contraste entre texto e fundo, pensando principalmente nos usuários mais idosos. |
| RNF04 – Responsividade | O sistema deve se adaptar a diferentes tamanhos de tela, funcionando bem tanto em computadores quanto em celulares pelo navegador. |
| RNF05 – Identidade visual | O visual do sistema deve seguir as cores da empresa, que são azul, branco e vermelho. |
| RNF06 – Segurança | As senhas devem ser armazenadas de forma criptografada e cada perfil de usuário só pode acessar o que for permitido para ele. O acesso ao sistema deve ser protegido contra falhas comuns, como as que o próprio Django já ajuda a evitar. |

## Riscos

| Data | Risco | Prioridade | Responsável | Status | Providência/Solução |
|---|---|---|---|---|---|
| 19/11/2026 | Mudança ou má compreensão dos requisitos durante o desenvolvimento | Média | Gerente | Vigente | Revisar os requisitos a cada entrega. |
| 19/11/2026 | Venda duplicada da mesma poltrona na mesma viagem | Alta | Desenvolvedores | Vigente | Implementar limitadores e funções de checagem e testar o fluxo de compra com vários acessos ao mesmo tempo. |
| 19/11/2026 | Perda de dados de passagens, viagens ou cadastros | Alta | Desenvolvedores | Vigente | Configurar backups automáticos do banco e testar a restauração dos dados. |
| 19/11/2026 | Interface difícil de usar para idosos e pessoas com pouca experiência | Média | Todos | Vigente | Manter o design simples, usar fontes e botões grandes e fazer testes de uso com pessoas desse perfil. |
| 19/11/2026 | Atendentes não atualizarem o sistema sobre atrasos e cancelamentos | Média | Gerente | Vigente | Fazer um treinamento rápido com os funcionários e deixar o registro de atrasos fácil de acessar. |

## Referências

https://github.com/tacianosilva/engenharia-software/blob/main/docs/doc-visao.md
