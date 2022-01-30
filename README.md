[<img src="https://raw.githubusercontent.com/masuta16/awesome-apache-airflow-br/main/master/images/apache-airflow.png" align="right">](https://airflow.apache.org/)
# Awesome Apache Airflow
<!-- ![contrib badge](https://img.shields.io/github/contributors/jghoman/awesome-apache-airflow.svg) ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/jghoman/awesome-apache-airflow?style=plastic) -->

Essa é uma lista de referências sobre o [Apache Airflow](https://airflow.apache.org/).
Por favor sinta-se livre para contribuir com qualquer item que você gostaria de incluir. Os items são geralmente adicionados no topo de cada seção.

## Conteúdo (Inglês)
- [Links Essenciais](#links-essenciais)
- [Soluções para deploy no Airflow](#soluções-para-deploy-no-Airflow)
- [Introduções e tutoriais](#introduções-e-tutoriais)
<!-- - [Videos da conferencia Airflow Summit](#airflow-summit-2020-videos) -->
- [Boas praticas, lições aprendidas e bons usos de casos](#best-practices-lessons-learned-and-cool-use-cases)
<!-- - [Livros, blogs, podcasts e mais](#books-blogs-podcasts-and-such)
- [Apresentação de vídeos online](#slide-deck-presentations-and-online-videos)
- [Bibliotecas, Hooks, Utilitários](#libraries-hooks-utilities)
- [Meetups](#meetups)
- [Airflow comercial como um provedor de serviços](#commercial-airflow-as-a-service-providers)
- [Referencias para o Cloud Composer](#cloud-composer-resources)
- [Non-English resources](#non-english-resources) -->
## Links Essenciais
- [Codigo Fonte](https://github.com/apache/airflow/) (latest stable release [1.10.12](https://github.com/apache/airflow/tree/1.10.12))
- [Documentação](https://airflow.apache.org/) (also the official website)
- [Pagina do confluence](https://cwiki.apache.org/confluence/display/AIRFLOW/Airflow+Home)
- [![Twitter Follow](https://img.shields.io/twitter/follow/apacheairflow?style=social)](https://twitter.com/ApacheAirflow)
- [Area de trabalho no Slack ](https://apache-airflow-slack.herokuapp.com/)
## Soluções de deployment do Airflow 
- [Tutorial de como instalar Apache Airflow na IBM Cloud](https://github.com/KissConsult/Apache-Airflow) - Tutorial de deploy feito de forma rápida e fácil na nuvem IBM com IBM [Bitnami Charts](https://github.com/bitnami/charts)

- [Três formas de executar o airflow no Kubernetes](https://fullstaq.com/blog/three-ways-to-run-airflow-on-kubernetes/) - [Tim van de Keer](https://www.linkedin.com/in/tim-van-de-keer-bb5a1966) explica por diversas formas como fazer o deploy do Airflow no Kubernetes.
- [Deploy Multi Tier gratuito do Apache Airflow na Azure ](https://azure.microsoft.com/en-us/blog/bitnami-apache-airflow-multi-tier-now-available-in-azure-marketplace/) - Um template gratuito ARM ou Azure Resource Manager feito pela Bitnami oferecendo uma solução de um clique para o deployment para estudos de caso.

- [KubernetesExecutor Helm Chart](https://github.com/tekn0ir/airflow-chart) - Um Helm Chart mais simples usando o KubernetesExecutor para uma experiencia nativa com o Kubernetes ou k8s e que também serve para complementar
[KubernetesExecutor Docker Image](https://github.com/tekn0ir/airflow-docker).
- [Stable Celery Helm Chart](https://github.com/helm/charts/tree/master/stable/airflow) - 
Chart Helm do Celery no repositório oficial

- [Puckel's Docker Image](https://github.com/puckel/docker-airflow) - Feita pelo usuário do twitter [@Puckel_](https://twitter.com/Puckel_) é
uma imagem Docker muito bem planejada que tem chegado como base para muitas instalações no Airflow. Ela é normalmente atualizada e segue muito próxima dos releases oficiais do Apache.
- [Operador customizado do Kubernetes para fazer deploy do Airflow](https://github.com/GoogleCloudPlatform/airflow-operator) - Controlador customizado do Kubernetes(tambem chamado de padrão de operador) para fazer o deploy do Airflow no Kubernetes.
- [airflow-pipeline](https://github.com/datagovsg/airflow-pipeline) - Container docker do Airflow que vem pre-configurado para Spark e Hadoop. Ele pode ser retirado de ``datagovsg/airflow-pipeline``.
- [aws-airflow-stack](https://github.com/villasv/aws-airflow-stack) -Um cluster de deploy baseado na AWS com o CeleryExecutor. Ele faz o deploy apos alguns cliques com CloudFormation

- [kube-airflow](https://github.com/mumoshu/kube-airflow) - Esse repositório contém uma imagem Docker Airflow (que parece ter sido baseada no trabalho do Puckel) e a definição recente do serviço Kubernetes. O repositório do usuário [mumoshu](https://github.com/mumoshu) não foi recentemente atualizado mas foram feitos muitos forks que podem ser baseados em mais releases recentes
- [airflow-on-kubernetes](https://github.com/rolanddb/airflow-on-kubernetes) -
Um guia de todas referencias relevantes, scripts e projetos que se relacionam para executar Airflow no Kubernetes.

- [airflow-k8s-executor-on-GKE](https://github.com/EamonKeane/airflow-GKE-k8sExecutor-helm) - 
Um tutorial para ter um executor do airflow no ambiente do kubernetes para ser feito o deploy na [Google Kubernetes Engine](https://cloud.google.com/kubernetes-engine/) com [helm](https://helm.sh/).
- [airflow-cookbook](https://github.com/bahchis/airflow-cookbook) - Receitas de como fazer o deploy do Airflow
- [Executando Airflow com Apache Mesos](http://agrajmangal.in/blog/big-data/running-airflow-on-top-of-apache-mesos/) - 
Blog descrevendo como configurar [Mesos](http://mesos.apache.org/) para executar todos os componentes do Airflow. 
- [Integrando Apache Airflow com Apache Ambari ](https://medium.com/@mykolamykhalov/integrating-apache-airflow-with-apache-ambari-ccab2c90173) - [Mykola Mykhalov](https://www.linkedin.com/in/mykola-mykhalov-9079a8107/) explica como usar o [Apache Ambari](https://ambari.apache.org/) para configurar e fazer o deploy de uma instancia do Airflow.
- [Platforma Astronomer ](https://github.com/astronomerio/astronomer) - 
Apache Airflow como um serviço no Kubernetes. Para maiores informações visite https://www.astronomer.io.
- [Imagem Docker Bitnami Airflow ](https://github.com/bitnami/bitnami-docker-airflow) - Uma imagem docker segura e atualizada para Airflow fornecida por Bitnami
- [Imagem Docker de Agendador do Bitnami Airflow ](https://github.com/bitnami/bitnami-docker-airflow-scheduler) - Uma imagem docker segura e atualizada para o agendador de tarefas do Airflow fornecida por Bitnami
- [Bitnami Airflow Worker Docker image](https://github.com/bitnami/bitnami-docker-airflow-worker) - Uma imagem segura e atualizada para o Airflow Worker fornecida pela Bitnami. Um deployment com CeleryExecutor esta disponivel [aqui](https://github.com/bitnami/bitnami-docker-airflow-worker/blob/master/docker-compose.yml).
- [Distribuição & deploy no Apache Airflow via arquivos Python PEX](https://github.com/msumit/airflow-pex) - Repositorio exemplo com passos para distribuir e fazer o deploy do Apache Airflow com arquivos PEX.
- [Introduzindo KEDA para o Airflow](https://www.astronomer.io/blog/the-keda-autoscaler/) - Como usar o KEDA para habilitar workers celery baseados no armazenamento de dados da base de metadados do Airflow.
- [Airflow-Component](https://github.com/noelmcloughlin/airflow-component#lightweight-federated-apache-airflow-installer) - Instalador leve da arquitetura  de referência federated Airflow-Airflow (RabbitMQ) nos nós calculados.

## Introduções e tutoriais
- [Métricas de monitoramento do Apache Airflow](https://youtu.be/xyeR_uFhnD4) - Uma serie em duas partes feita por [maxcotec](https://maxcotec.com) em como você pode utilizar as métricas existentes do Airflow para monitorar seu deploy da dashboard do Grafana via Prometheus. Também aprenda como criar métricas customizadas
- [Introdução ao Airflow](https://www.youtube.com/playlist?list=PLzKRcZrsJN_xcKKyKn18K7sWu5TTtdywh) - Um tutorial em serie web por [maxcotec](https://maxcotec.com) para usuários iniciantes e intermediários do Apache Airflow
- [ETL com Apache Airflow para analise de dados em dados transacionais](https://github.com/KimaruThagna/ml-pipelines-airflow). [Kimaru Thagana](https://www.linkedin.com/in/kimaru-thagana-4920b5181/) cobre um caso pratico de fazer o processo de ETL usando Apache Airflow usando um comercio dummy para transações, usuário e dados de produtos. Os dados são entregues via uma API flask.
- [Comece construindo pipelines de dados melhores com Apache Airflow](https://blog.delaplex.com/start-building-better-data-pipelines-with-apache-airflow) - Naman Gupta cobre o básico do Airflow e seus conceitos .
- [Template de repositório do Airflow](https://github.com/soggycactus/airflow-repo-template) - 
  Um repositorio boilerplate para desenvolver localmente com Airflow com testes para DAGs validas e plugins. Só cole e execute `make start-airflow` para começar. Adicione alguns jobs CI para fazer o deploy do seu código quando você tiver terminado.
- [Como Apache Airflow distribui jobs nos workers Celery](https://blog.sicara.com/using-airflow-with-celery-workers-54cb5212d405) - 
Uma curta descrição dos passos feitos para uma instancia de tarefas para o processo de agendamento ao sucesso em uma arquitetura distribuída
-[Submissão remota do Spark para o YARN executando no EMR](https://medium.com/@tamizhgeek/remote-spark-submit-toyarn-running-on-emr-9804b89d82d2) - [Azhaguselvan](https://github.com/tamizhgeek) explica como submeter jobs do Spark para os cluster existentes EMR com Airflow
- [Executando Airflow no topo do Apache Mesos](http://agrajmangal.in/blog/big-data/running-airflow-on-top-of-apache-mesos/) e seu acompanhamento, [Mesos, Airflow & Docker](http://agrajmangal.in/blog/big-data/mesos-airflow-docker/) by [Agraj Mangal](https://twitter.com/agrajm) tem uma revisão rápida de como executar Airflow no Apache Mesos
- [Dustin Stansbury](https://twitter.com/corrcoef) do [Quizlet](https://quizlet.com/) escreveu uma serie de quatro partets que cobre o que gerenciadores de workflow fazer em geral, como Quizlet pegou Airflow um turismo dos conceitos chaves do Airflow e como Quizlet está agora usando Airflow na pratica:
  - [Além de CRON uma introdução para os sistemas de gerenciamento em workflow](https://medium.com/@dustinstansbury/beyond-cron-an-introduction-to-workflow-management-systems-19987afcdb5e)
  - [Porque Quizlet escolheu Apache Airflow para executar workflow de dados](https://towardsdatascience.com/why-quizlet-chose-apache-airflow-for-executing-data-workflows-3f97d40e9571)
  - [Entendendo os conceitos chave do Apache Airflow](https://medium.com/@dustinstansbury/understanding-apache-airflows-key-concepts-a96efed52b1a)
  - [Como Quizlet usa o Apache Airflow na pratica](https://medium.com/@dustinstansbury/how-quizlet-uses-apache-airflow-in-practice-a903cbb5626d)
  
- [Integrando Apache Airflow com Databricks](https://databricks.com/blog/2017/07/19/integrating-apache-airflow-with-databricks.html) -   Esse tutorial é focado especificamente nas soluções com Spark do databricks ele tem uma visão razoável do básico do Airflow e demonstra como uma solução third party pode rapidamente integrar com Airflow
- [Tutorial do Apache Airflow 2.0](https://turbaszek.medium.com/apache-airflow-2-0-tutorial-41329bbf7211) - Esse artigo discute conceitos básicos de como ficar por trás de Airflow e discute os problemas que ele resolve. 
- [Testando e debugando Apache Airflow](https://blog.godatadriven.com/testing-and-debugging-apache-airflow) - Artigo explicando como aplicar teste unitário, mocking e debugging para o código do Airflow. 
- [Iniciando desenvolvimento de workflows com Apache Airfloww](http://michal.karzynski.pl/blog/2017/03/19/developing-workflows-with-apache-airflow/) - Esse breve tutorial de introdução cobre como criar um pipeline de dados e processar o workflow usando DAG, operadores, sensor, usar Xcoms para comunicar entre operadores.
- [Iniciando com Airflow + Plataforma Google Cloud + Docker](https://medium.com/@junjiejiang94/get-started-with-airflow-google-cloud-platform-docker-a21c46e0f797) - Introcdução passo a passo por [Jayce Jiang](https://medium.com/@junjiejiang94).
- [Como desenvolver um pipeline de dados no Airflow por teste TDD(test-driven development)](https://blog.magrathealabs.com/how-to-develop-data-pipeline-in-airflow-through-tdd-test-driven-development-c3333439f358) -Aprenda como construir um pipeline de dados usando TDD passo a passo e no fim como configurar um simples workflow CLI usando Github actions.
## Boas praticas, lições aprendidas e bons usos de caso

- [Gerenciamento de pacotes de Python com DAG do Airflow](https://www.youtube.com/watch?v=9pykChPp-X4&t=121s) - Gerenciar pacotes Python com mais de 100 dependências em DAGs pode se tornar trabalhoso. É difícil rastrear quais pacotes são usado para cada DAG, e mais difícil limpar durante a remoção ou atualização da DAG. Aprenda como o KubernetesPodOperator e o DockerOperator pode consertar isso.
- [Gerenciamento de Dag do Airflow & versionamento](https://youtu.be/a-4yRne3ba4) - Gestione DAGs eficientemente com o processo de lançamento usando Git e submódulos
- [Testando no Airflow parte 2](https://medium.com/@chandukavar/testing-in-airflow-part-2-integration-tests-and-end-to-end-pipeline-tests-af0555cd1a82) - [Chandu Kavar](https://twitter.com/chandukavar) e [Sarang Shinde](https://www.linkedin.com/in/sarang-shinde-219a4873/) explicam testes de integração e testes end to end para pipeline.
- [Atualizando e escalando Airflow em Robinhood](https://robinhood.engineering/upgrading-scaling-airflow-at-robinhood-5b625dfaa2ee) - [Abishek Ray](https://www.linkedin.com/in/abhishek-ray-29210145/) descreve como Robinhood abordou o upgrade de sua produção Airflow enquanto minimizava o tempo de inatividade.
- [Nos todos estamos usando Airflow errado e como podemos consertar isso](https://medium.com/bluecore-engineering/were-all-using-airflow-wrong-and-how-to-fix-it-a56f14cb0753) - [Jessica Laughlin](https://www.jldlaughlin.com/) da [Bluecore](https://www.bluecore.com/) compartilha tres problemas de engenharia associados com o design do Airflow e como resolver isso usando [KubernetesPodOperator](https://github.com/apache/airflow/blob/v1-10-stable/airflow/contrib/operators/kubernetes_pod_operator.py) em dois padrões de design.
- [Começando com linhagem de dados](https://medium.com/dailymotion/getting-started-with-data-lineage-6307b2b429b3) - [Germain Tanguy](https://www.linkedin.com/in/germain-tanguy/) de [Dailymotion](https://www.dailymotion.com/) compartilha um protótipo de linhagem de dados integrado com Apache Airflow.
- [Colaboração entre engenheiros de dados analistas de dados e cientistas de dados](https://medium.com/dailymotion/collaboration-between-data-engineers-data-analysts-and-data-scientists-97c00ab1211f) - [Germain Tanguy](https://www.linkedin.com/in/germain-tanguy/) de [Dailymotion](https://www.dailymotion.com/) mostra como lançar uma produção eficiente para colaboração com Apache Airflow.
- [Usando o operador Docker do Airflow com o repositório de container da Amazon](https://www.lucidchart.com/techblog/2019/03/22/using-apache-airflows-docker-operator-with-amazons-container-repository/) - [Brian Campbell](https://www.linkedin.com/in/bvcampbell3) da [Lucid](https://www.lucidchart.com/) oferece dicas de como integrar o serviço da AWS [ECR](https://aws.amazon.com/ecr/) com o DockerOperator do Airflow.
- [Airflow: dicas menos conhecidas truques e melhores praticas](https://medium.com/datareply/airflow-lesser-known-tips-tricks-and-best-practises-cf4d4a90f8f) - [Kaxil Naik](https://www.linkedin.com/in/kaxil/) explica as menos conhecidas ainda muito uteis dicas de melhores praticas em usar Airflow.
- [boundary-layer:Workflows declarativos do Airflow](https://codeascraft.com/2018/11/14/boundary-layer%E2%80%89-declarative-airflow-workflows/) - [Kevin McHale](https://www.linkedin.com/in/mchalek) explica como usar uma camada de projeto open source que gera a DAG do Airflow com workflows declarativos.
- [Testando no Airflow parte 1](https://medium.com/@chandukavar/testing-in-airflow-part-1-dag-validation-tests-dag-definition-tests-and-unit-tests-2aa94970570c) - [Chandu Kavar](https://twitter.com/chandukavar) explica diferentes características de testes no Airflow. Isso inclui testes de validação, testes de definição da DAG e testes unitários
- [Melhorando a segurança de interface de usuário do Airflow](https://wecode.wepay.com/posts/improving-airflow-ui-security) -  [Joy Gao](https://twitter.com/joygao) da WePay explica a necessidade da para a função de controles baseados em regra (RBAC) e como ela introduziu isso para o Airflow.
- [Como criar um workflow em Apache Airflow para rastrear surtos de doenças na India](https://blog.socialcops.com/engineering/apache-airflow-disease-outbreaks-india/) - [Vinayak Mehta](https://twitter.com/vortex_ape) explica como [SocialCops](https://socialcops.com/) usa o Airflow para fazer coleta de dados do ministro da saúde e casos de família para gerar dados derivados de possíveis surtos de doenças.
- [ Airflow, engenharia de meta dados, e uma plataforma de dados para a maior democracia do mundo](https://blog.socialcops.com/technology/engineering/airflow-meta-data-engineering-disha/) - [Vinayak Mehta](https://twitter.com/vortex_ape) fala sobre identificar padrões de engenharia de dados(engenharia de meta dados)para automatizar a geração de DAG e como isso ajudou [SocialCops](https://socialcops.com/) para empoderar DISHA, uma plataforma de dados nacionais onde os MPs indianos e monitorar MLAs no progresso de 42 níveis de esquemas nacionais.
- [Lições aprendidas no Airflow-ing](https://medium.com/@nehiljain/lessons-learnt-while-airflow-ing-32d3b7fc3fbf) e [Airflow part 2: lições aprendidas](https://medium.com/snaptravel/airflow-part-2-lessons-learned-793fa3c0841e) - [Nehil Jain](https://twitter.com/nehiljain) escreveu uma serie de duas partes que cobre o valor dos agendadores de workflow, algumas boas praticas e pontos que ele encontra enquanto esta trabalhando com Airflow. O [segundo artigo](https://medium.com/snaptravel/airflow-part-2-lessons-learned-793fa3c0841e) em particular inclui muitas dicas de produção.
- [Porque Robinhood usa Airflow](https://robinhood.engineering/why-robinhood-uses-airflow-aed13a9a90c8) - [Vineet Goel](https://twitter.com/vineetik) explica porque uma plataforma de troca financeira [Robinhood](https://robinhood.com/) começou com Airflow sobre work schedulers alternativos.
- [O que nós aprendemos migrando de Cron para Airflow](https://medium.com/videoamp/what-we-learned-migrating-off-cron-to-airflow-b391841a0da4) - [Katie Macias](https://medium.com/@katiemacias) descreve a jornada do engenheiro de dados [VideoAmp](https://www.videoamp.com/) de cron para Airflow.
- [Under the Hood: Construindo AIR em Qubole](https://www.qubole.com/blog/hood-building-air-qubole/) - [Sreenath Kamath](https://www.linkedin.com/in/sreenath-kamath-66a1b970/) e [Rajat Venkatesh](https://twitter.com/vrajat) escrevem sobre construir a [Qubole](https://www.qubole.com/)'s [plataforma de descoberta de dados insights e recomendações](https://www.qubole.com/blog/building-qdsair-infrastructure/) sobre o Airflow.
  
- [Airflow porque não esta funcionando  - TL;DR Airflow’s SubDagOperator causes deadlocks](https://medium.com/bluecore-engineering/airflow-why-is-nothing-working-f705eb6b7b04) by [Jessica Laughlin](https://twitter.com/thepressofjess) - Se aprofunde no conceito de solução de problemas com a DAG do Airflow com boas dicas de como diagnosticar problemas.
- [Apache Airflow como um agendador externo para sistemas distribuidos](https://medium.com/@rako/apache-airflow-as-an-external-scheduler-for-distributed-systems-53b7354d3e48) - [Arunkumar](https://medium.com/@rako) sugere usar Airflow como um agendador externo simples para um sistema distribuído.
- [Como Sift treina milhares de modelos usando o Apache Airflow](https://engineering.siftscience.com/sift-trains-thousands-models-using-apache-airflow/) - Resumo da estratégia de deployment da [Sift Science](https://siftscience.com/)para as pipelines de modelos de machine learning.
- [Apache Airflow no Pandora](https://engineering.pandora.com/apache-airflow-at-pandora-1d7a844d68ee) - [Ace Haidrey](https://www.linkedin.com/in/acehaidrey/) discute porque Pandora escolheu Airflow e oferece um resumo de seu deployment e a infraestrutura por trás disso.
- [ Lições da frente de engenharia de dados em Chicago com Airflow](https://medium.com/stanton-ventures-insights/airflow-lessons-from-the-data-engineering-front-in-chicago-9489e6ad5c3d) - [Alison Stanton](https://twitter.com/alison985) oferece uma lista de dicas de como evitar pegadinhas nos jobs do Airflow.
- [Inferno dos dados: 7 círculos de inferno de teste de dados com Airflow](https://medium.com/wbaa/datas-inferno-7-circles-of-data-testing-hell-with-airflow-cef4adff58d8) -A equipe  Wholesale Banking Advanced Analytics em ING detalha como eles torturam testes das DAGs do Airflow antes do deployment.
-  [Teste de dados com repositório do Airflow](https://github.com/danielvdende/data-testing-with-airflow)
- [Checadores de qualidade de dados](https://drivy.engineering/data-quality/) - [Antoine Augusti](https://twitter.com/AntoineAugusti) descreve como o framework [drivy](https://www.drivy.co.uk/) tem sido aplicado sobre o Airflow para testar o dataset deles para completude, pontualidade, distinção, validades e acurácia
- [Construindo o data warehouse da WePay usando BigQuery e Airflow](https://wecode.wepay.com/posts/wepays-data-warehouse-bigquery-airflow) - O inestimável [Chris Riccomini](https://twitter.com/criccomini) descreve como [WePay](https://go.wepay.com/), um dos primeiros adeptos do Airflow integrou para o ambiente deles o [Google Cloud Compute](https://cloud.google.com/compute/).
- [Usando Apache Airflow para criar uma infraestrutura de dados no setor publico](https://www.astronomer.io/blog/using-apache-airflow-to-create-data-infrastructure/) - Apesar de um tom de pitch de vendas, esse artigo de blog descreve como [ARGO Labs](http://www.argolabs.org/), uma organização sem fins lucrativos, utiliza Airflow para fazer ETL nos dados do setor publico.
- [ETL with airflow](https://gtoonstra.github.io/etl-with-airflow/) - Os princípios do core de ETL e muitos exemplos docker end to end incluindo Kimball, data vault no Hive e alguns exemplos mais simples.
- [Como agregar dados para BigQuery usando Apache Airflow](https://cloud.google.com/blog/big-data/2017/07/how-to-aggregate-data-for-bigquery-using-apache-airflow) - Exemplo de como usar Airflow para a Big Query do Google para aprimorar uma dashboard Data Studio.
- [Produzindo ML com workflows no twitter](https://blog.twitter.com/engineering/en_us/topics/insights/2018/ml-workflows.html) - Post de como e porque twitter usa o Airflow para ML workflows incluindo operadores customizados e uma custom UI embarcada na interface web do Airflow.3
- [Executando Apache Airflow no Lyft](https://eng.lyft.com/running-apache-airflow-at-lyft-6e53bb8fccff) - Este tutorial mostra uma overview de como o Lyft opera com Apache Airflow na produção(monitoramento, customização, etc).
- [Fazendo deploy do Apache Airflow na Azure para construir e executar pipelines de dados](https://azure.microsoft.com/sv-se/blog/deploying-apache-airflow-in-azure-to-build-and-run-data-pipelines/) - Esse texto fala como executar Airflow na Azure.
- [O Zen de Python e o Apache Airflow](https://blog.godatadriven.com/zen-of-python-and-apache-airflow) - Post de blog de como o Zen do python pode ser aplicado para o codigo do Airflow.
- [Deixando Apache Airflow mais seguro com UI e DAG Level Acess](https://eng.lyft.com/securing-apache-airflow-ui-with-dag-level-access-a7bc649a2821) - Post de blog sobre o nivel de acesso da DAG do Airflow e como Lyft usa ele.
- [Atualizando Airflow com Zero inatividade](https://medium.com/flatiron-engineering/upgrading-airflow-with-zero-downtime-8df303760c96) - Um artigo detalhado de como fazer deploy do Airflow com zero de inatividade.
- [Building a Production-Level ETL Pipeline Platform Using Apache Airflow](https://towardsdatascience.com/building-a-production-level-etl-pipeline-platform-using-apache-airflow-a4cf34203fbd) - Esse post descreve como a equipe de gestão de sistemas no Cerner usa Airflow
- [Usando setup minimo do Airflow no Kubernetes (Local, EKS, AKS)](https://github.com/stwind/airflow-on-kubernetes) - Um artigo de como fazer deploy do Airflow no Kubernetes local, AWS EKS e Azure AKS com um setup minimalista.
- [Explicando o Airflow DAG monorepo](https://tech.scribd.com/blog/2020/breaking-up-the-dag-repo.html) - Esse post descreve como fazer gerenciamento de suporte das DAGs do Airflow de multplos repositorios git pelo S3.
- [Improving Performance of Apache Airflow Scheduler](https://medium.com/databand-ai/improving-performance-of-apache-airflow-scheduler-507f4cb6462a) - Uma historia de uma aventura que permitiu [Databand](https://databand.ai/) a acelerar o tempo de parsing da DAG em 10 vezes
- [Como SSENSE está usando Apache Airflow para dazer linhagem de dados na AWS](https://medium.com/ssense-tech/principled-data-engineering-part-ii-data-governance-30297abb2446) - O texto explora os temas fundamentais de arquitetura e governança de um data lake na AWS usando Apache Airflow.
- [Monitorando Airflow com Prometheus, StatsD e Grafana](https://databand.ai/blog/everyday-data-engineering-monitoring-airflow-with-prometheus-statsd-and-grafana/) - Um guia de como agrupar dashboards operacionais para um cluster de produção por  [Databand](http://databand.ai)e conseguir uma visibilidade de alto nivel no Airflow.
- [Orquestração de tarefas complexas em Hurb com Apache Airflow](https://medium.com/hurb-engineering/complex-tasks-orchestration-at-hurb-with-apache-airflow-dcb423c4dee6) - Este post mostra como  [Hurb](https://hurb.com) utiliza Apache Airflow para orquestrar tarefas complexas e como ele alavanca a criação dinamica da DAG para melhorar a velocidade do desenvolvimento.
