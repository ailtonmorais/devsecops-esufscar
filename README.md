<p align="center">
<br>Departamento de Computação (DComp-So)</br>
<br>Centro de Ciências e Gestão em Tecnologias (CCGT)</br>
<br>UNIVERSIDADE FEDERAL DE SÃO CARLOS - Campus Sorocaba</br><br></br>
<img src="./images/ufscar.png" width="166">
</p>

# Sobre

Material criado para o seminário que aborda DevSecOps como parte da avaliação da disciplina de Engenharia de Software (2021/2) - Prof. Dr. Alexandre Alvaro, do programa de mestrado em Ciência da Computação da UFScar Sorocaba.

# DevSecOps
<sub>Autores: Ailton Morais & Alex Rocha</sub>

<a id="indice"></a>
# Índice
1. [Introdução](#introducao)    
	1.1. [O que é DevOps](#sobre-devops)<br>
	1.2. [Cultura DevOps](#cultura-devops)<br>
    1.3. [Pilares da Cultura DevOps](#pilares-cultura-devops)<br>
    1.3.1. [Integração Contínua](#integracao-continua)<br>
    1.3.2. [Feedback Contínuo](#feedback-continuo)<br>
    1.3.3. [Implantação Contínua](#implantacao-continua)<br>
    1.4. [DevOps & Lean](#devops-lean)
2. [Qual a importância do DevOps](#importancia-devops)    
	2.1. [Benefícios do DevOps](#beneficios-devops)<br>
    2.1.1. [Integrar as Equipes](#integrar-equipes)<br>
    2.1.2. [Identificar Possíveis Melhorias](#identificar-melhorias)<br>
    2.1.3. [Facilitar a Adoção de Novas Tecnologias](#facilitar-novas-tecnologias)<br>
    2.1.4. [Automatizar Atividades](#automatizar-atividades)<br>
    2.1.5. [Elaborar Novas Estratégias](#elaborar-estratégias)        
3. [Onde Entra a Segurança no Ciclo DevOps](#inicio-seg-devops)
4. [DevOps vs DevSecOps](#devops-devsecops)
5. [O que muda com o DevSecOps](#mudanca-devsecops)
6. [Quais os Benefícios do DevSecOps para o Negócio](#beneficios-devsecops)
7. [Como Implementar DevSecOps](#implementar-devsecops)
8. [Conclusão](#conclusao)
9. [Referências Bibliográficas](#referencias)

<a id="introducao"></a>
## 1. Introdução

A proposta do deste material é apresentar a abordagem DevSecOps nas empresas

<a id="sobre-devops"></a>
### 1.1. O que é DevOps

Podemos entender o DevOps como a união de ferramental e cultura no processo de desenvolvimento de software, sendo um conjunto de práticas para viabilizar a integração entre as equipes de desenvolvimento de software, controle de qualidade, suporte e infraestrutura através da automação de processos para entrega de software. DevOps também se trata de cultura a ser adotada pela empresa e pelos times envolvidos no ciclo de vida do produto de software.

A forma convencional de desenvolvimento de produtos de software adotada por diversas empresas, públicas e privadas, de diversos tamanhos e fins supõe que os times de Desenvolvimento de Operações trabalhem em diferentes setores de um determinado negócio tendo finalidades distintas fazendo com que esses times não compartilhem das mesmas motivações e comprometimento com os processos no ciclo de desenvolvimento de software. Isso ocorre não por um time se preocupar mais que o outro na entrega, mas por esses times possuírem visões diferentes do que é o pronto em suas atividades.

O time de desenvolvimento irá focar na sua entrega da base de código, o time de infraestrutura irá focar nos servidores funcionando, já o time de sustentação terá seu sucesso baseado na quantidade de chamados abertos e fechados.

As equipes de desenvolvimento hoje adotando metodologias ágeis e trabalhando de forma mais alinhadas ao negócio de cada empresa já consegue realizar alterações e implementações mais complexas de forma mais rápida e ágil do que da forma convencional. dessa forma conseguem atender a expectativa dos clientes valorizando o produto de software, já as áreas de operação prezam pela estabilidade do produto de software, dessa forma quanto menos alterações no ambiente de produção melhor, pois essas alterações podem gerar instabilidade e bugs impactando o usuário final e dessa forma desvalorizando o produto de software da empresa.

<a id="cultura-devops"></a>
### 1.2. Cultura DevOps

Sobre os pilares da cultura DevOps, pois podemos entender que o mesmo se trata de uma cultura, não apenas um conjunto de ferramentas tecnológicas a serem utilizadas podemos definir como Integração Contínua, Feedback contínuo e implantação contínua. Pelos pilares já é possível entender que o DevOps é implementado na tentativa de alcançar a máxima agilidade, assertividade e velocidade na implantação e reversão de mudanças na implementação e entrega de produtos software.

<a id="pilares-cultura-devops"></a>
## 1.3. Pilares da Cultura DevOps

A cultura DevOps se destaca por...

<a id="integracao-continua"></a>
### 1.3.1. Integração Contínua

No âmbito da Cultura DevOps, integração contínua trata-se da transferência facilitada e maximizada de conhecimento e das experiências adquiridas de forma empírica ou não   entre as áreas que impactam e são impactadas pelo produto de software. Realizar essa integração promove o compartilhamento de ideias, experiências e ajuda na adoção de alguma metodologia no trato do software que permita maior agilidade e confiabilidade na entrega e também na sustentação do produto após a entrega.

É necessário implementar ferramentas e metodologias promovendo essa integração para permitir essa troca de figurinhas entre as equipes que estão envolvidas nas fases do ciclo de vida do software ou serviço, isso ajudará na entrega, sustentação e na diminuição do tempo gasto para determinadas tarefas, essas podendo até ser automatizadas.

<a id="feedback-continuo"></a>
### 1.3.2. Feedback Contínuo

Feedback é necessário em qualquer meio, de qualquer negócio, porém se torna essencial como parte da cultura DevOps pois estimula que os times que fazem parte do ciclo de desenvolvimento de software possam aprender com os erros de seus pares, e encontrar soluções conjuntas para os problemas encontrados seja na entrega, quanto na sustentação, qualidade, etc.

Criar e manter um canal de feedback contínuo vai se mostrar essencial para a cultura DevOps pois permitirá que times que anteriormente trabalhavam distantes, influenciam nas decisões de execução e planejamento um dos outros, encontrando soluções em comum que beneficiem a entrega do produto de software como um todo.

<a id="implantacao-continua"></a>
### 1.3.3. Implantação Contínua

Implantação contínua ajudará na entrega, liberando de forma ágil novas versões de software para o cliente, porém vai além disso, se faz necessário para garantir qualidade podendo integrar um ciclo de teste anteriormente em um pipeline de implantação e também permitindo que ao encontrar determinado erro crítico, após sua correção, realizar uma nova implantação de maneira rápida minimizando os riscos e custos atrelados a uma implantação de software problemática contendo bugs.

Esse pilar também garante estratégia de negócio ao produto de software, pois viabiliza um ciclo de rápidas mudanças, onde um time de desenvolvimento poderá atender uma demanda de negócio/produto implementando e entregando uma nova feature de forma bem menos problemática e complicada do que a convencional.

<a id="devops-lean"></a>
## 1.4. DevOps & Lean

O DevOps baseia-se muito nas práticas do Lean que é uma filosofia de gestão inspirada nas práticas do sistema de gestão utilizado pela Toyota em seu Sistema Toyota de Produção. A filosofia Lean tem como seus princípios fundamentais: Valor, Fluxo de Valor, Fluxo, Produção Puxada e Perfeição. O Lean também foca muito em evitar o máximo de desperdício , entendendo que desperdício são componentes do processo que não possuem valor agregado ao projeto em si.

Se tratando de Lean, valor pode ser definido como a percepção do cliente acerca do resultado do produto ou serviço que será entregue pelo seu trabalho
Realizando um paralelo com DevOps, o Fluxo de valor definido para o mesmo pode ser entendido como um processo necessário para converter uma hipótese de negócio em um produto ou serviço que agregue e entregue valor ao cliente final.

[Voltar ao índice](#indice)

<a id="importancia-devops"></a>
## 2. Qual a importância do DevOps

Apoiar a implantação da cultura de DevOps no ciclo de desenvolvimento de software de qualquer empresa certamente levará a mesma a ganhos expressivos de diversos itens importantes e altamente impactantes para a melhoria e aumento da agilidade na entrega dos produtos de software. Temos os seguintes itens como pontos de melhoria expressivos do processo:

* **Velocidade**: Permite realizar adaptações, mudanças e entregas de forma mais ágil, garantindo maior dinamismo para os colaboradores e melhor experiência para o cliente;

* **Agilidade na Entrega**: Permite lançamentos mais rápidos e contínuos para os clientes, o que pode gerar vantagens competitivas para os negócios de TI;

* **Estabilidade**: É possível escalar as demandas de projetos de forma mais ágil, eficiente e sem gerar gargalos para os times. Isso é fundamental para evitar sobrecarga e atrasos;

* **CI/CD**: A   cultura DevOps permite implementar o método de Integração Contínua/Entrega Contínua (Continuous Integration/Continuous Delivery), permitindo entregar os produtos e serviços para o cliente de forma contínua e mais ágil;

* **Segurança**: Todos os envolvidos possuem responsabilidade compartilhada. Assim, é mais fácil identificar problemas que possam surgir e garantir maior segurança na criação da aplicação;

<a id="beneficios-devops"></a>
## 2.1. Benefícios do DevOps

Dentre os benefícios podemos citar...

<a id="integrar-equipes"></a>
### 2.1.1. Integrar as Equipes

Ao unir equipes, o entendimento da empresa como um todo é aprimorado e a visão passa a acontecer estrategicamente. Por contar com feedback contínuo, as necessidades da empresa passam a melhor compreendidas por todos.

Afinal nada como participar para entender a aceitação do produto na visão dos clientes. Sim, as áreas de uma empresa também podem e devem serem consideradas clientes pela TI.

O resultado dessa união é benéfico para todos os lados. Pois desenvolvedores conseguem maior respaldo enquanto o *service desk* se beneficia de um número menor na incidência de problemas.

<a id="identificar-melhorias"></a>
### 2.1.2. Identificar Possíveis Melhorias

Não podemos deixar de notar que as próprias áreas passam a se envolver mais com a tecnologia interna, dando mais sugestões de melhorias, o que aprimora ainda mais os projetos e aumenta a satisfação dos envolvidos.

Com comunicação constante e foco no cliente (sendo ele interno ou externo), as necessidades passam a ser melhor compreendidas. Isso possibilita a rápida ação dos desenvolvedores na implantação dos recursos.

<a id="facilitar-novas-tecnologias"></a>
### 2.1.3. Facilitar a Adoção de Novas Tecnologias

A adoção de novas tecnologias é uma característica inata da cultura DevOps. Conceitos como computação em nuvem se tornam mais presentes no ambiente corporativo e  trazem mais agilidade e praticidade no acesso à informação.

A adoção estratégica de APIs, por exemplo, potencializa a infraestrutura de TI e torna tudo mais seguro, prático e ágil.

<a id="automatizar-atividades"></a>
### 2.1.4. Automatizar Atividades

Contar com tecnologia para automatizar tarefas operacionais é essencial com a velocidade em que os negócios acontecem hoje. Atividades repetitivas ou que exijam um grau de segurança alto e com baixa margem de erro devem usar tecnologia para serem realizadas.

Se você tem um sistema ERP para faturamento, e um CRM para gestão das vendas, nada mais certo que eles se comuniquem automaticamente. Dessa forma, os profissionais envolvidos não precisem “re-digitar” informações. É mais produtividade, eficiência e tempo para pensar em estratégia: tudo que uma empresa precisa.

<a id="elaborar-estratégias"></a>
### 2.1.5. Elaborar Novas Estratégias

O DevOps é um movimento altamente adaptativo, podendo sofrer se necessário, modificações durante a sua aplicação. Com a supervisão da gestão, algumas otimizações podem acontecer durante o curso, como a diminuição no prazo de entrega, por exemplo.

Por contar com um monitoramento avançado, fica fácil identificar os pontos que precisam de ajuste. Basta a realização de um brainstorm coletivo para aprimorar ainda mais o processo.

[Voltar ao índice](#indice)

<a id="inicio-seg-devops"></a>
## 3. Onde Entra a Segurança no Ciclo DevOps

O Ciclo DevOps...

[Voltar ao índice](#indice)

<a id="devops-devsecops"></a>
## 4. DevOps vs DevSecOps

Ao falar de DevOps vs DevSecOps...

[Voltar ao índice](#indice)

<a id="mudanca-devsecops"></a>
## 5. O que muda com o DevSecOps

A mudança no DevSecOps...

[Voltar ao índice](#indice)

<a id="beneficios-devsecops"></a>
## 6. Quais os Benefícios do DevSecOps para o Negócio

Dentre os benefícios do DevSecOps podemos citar...

[Voltar ao índice](#indice)

<a id="implementar-devsecops"></a>
## 7. Como Implementar DevSecOps

Para immplentar o DevSecOps...

[Voltar ao índice](#indice)

<a id="conclusao"></a>
## 8. Conclusão

Podemos conncluir que o DevSecOps...

[Voltar ao índice](#indice)

<a id="referencias"></a>
# 9. Referências Bibliográficas

<a id="MySQL-2020a"></a>
1. MySQL. [MySQL CLUSTER, 2020a](https://www.mysql.com/products/cluster/mysql-cluster-datasheet.pdf). Acesso em 14 out 2020 às 19h20m.

<a id="MySQL-2020b"></a>
2. MySQL. [MySQL CLUSTER, 2020b](https://www.mysql.com/products/cluster/availability.html). Acesso em 17 out 2020 às 11h00m.