# In Memory Test

O termo "In Memory Test" é conhecido com uma estratégia de desenvolvimento em que permite ao desenvolvedor construir e testar sua aplicação sem a necessidade de ter um banco de dados. E no AdvPL não seria diferente...

Mas como assim? O Protheus SEMPRE precisa ter um banco de dados, senão o sistema não funciona.

Concordo, porém, o Protheus precisa já seu desenvolvimento não...

Imagine que você esteja trabalhando em uma personalização que necessite salvar dados numa tabela personalizada, contudo, nesse cliente existem outros desenvolvedores atuando na mesma base de HOMOLOGAÇÃO que você, e com isso seja necessário alinhar com o time uma parada no sistema para que sua tabela, campos e índices sejam criados. Você como desenvolvedor ficaria esperando todo esse tempo pra seguir com o desenvolvimento? CLARO que não.

É aí que entram os "In Memory Test", que consiste num padrão estratégico em que você se utiliza da persistência de dados em memória, simulando um banco de dados.

Por exemplo, você está atuando numa feature que precisa salvar algumas informações numa tabela personalizada, e nessa tabela precisarão ser salvas informações de diferentes tipos e com formatações específicas. Você pode simplesmente jogar esses dados numa variável, e _printá-los_ no trecho em que seria escrito a parte do _RecLock_. Com os dados já tratados vc só precisaria desenvolver o trecho do _RecLock_ após a criação da tabela, o que te pouparia um tempo enorme.

O objetivo desse tópico é apresentar outras formas ao desenvolvedor para superar barreiras com a qual nos deparamos no dia a dia.