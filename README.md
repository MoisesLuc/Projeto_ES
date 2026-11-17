# Projeto da disciplina Engenharia de Software

## DigiBus - Plataforma Digital de Linhas Rodoviárias

### Descrição do projeto

O DigiBus é uma plataforma digital para linhas rodoviárias que atende os moradores da região do Seridó, desde adolescentes até idosos que viajam com frequência entre cidades. O objetivo principal é facilitar a compra e o cancelamento de passagens e ajudar os passageiros a planejarem a viagem antes do embarque. Com o sistema, o usuário poderá acompanhar a localização dos ônibus, ver os horários previstos de chegada e partida e receber avisos sobre atrasos ou cancelamentos.

O projeto busca resolver problemas como a superlotação dos ônibus e a falta de aviso quando há atrasos ou cancelamentos. Para a empresa, a plataforma também ajuda no gerenciamento da frota, já que o número de passagens vendidas permite organizar melhor os ônibus de cada linha, além de gerar relatórios mensais e anuais.

### Tecnologias utilizadas

Nesta primeira etapa, o projeto será desenvolvido como uma plataforma web usando o framework Django, que é feito em Python. Ele foi escolhido porque já traz muitas funções prontas, como sistema de login, controle de usuários e painel administrativo. O Django também facilita a criação das telas, das regras de negócio e da organização do código.

Para o armazenamento dos dados será usado o banco de dados PostgreSQL. Nele serão guardadas as informações de usuários, linhas, horários, ônibus, passagens compradas e canceladas, além dos dados usados nos relatórios. O Django se conecta bem ao PostgreSQL, o que deixa o desenvolvimento mais simples e seguro.

Para o visual das páginas, o Django usará seus próprios templates em conjunto com HTML e CSS, de forma que as telas se adaptem a diferentes tamanhos de tela.
