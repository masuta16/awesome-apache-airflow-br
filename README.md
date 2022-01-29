[<img src="https://raw.githubusercontent.com/masuta16/awesome-apache-airflow-br/main/master/images/apache-airflow.png" align="right">](https://airflow.apache.org/)
# Awesome Apache Airflow
<!-- ![contrib badge](https://img.shields.io/github/contributors/jghoman/awesome-apache-airflow.svg) ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/jghoman/awesome-apache-airflow?style=plastic) -->

Essa é uma lista de referências sobre o [Apache Airflow](https://airflow.apache.org/).
Por favor sinta-se livre para contribuir com qualquer item que voce gostaria de incluir. Os items são geralmente adicionados no topo de cada seção.

## Conteúdo (Ingles)
- [Links Essenciais](#links-essenciais)
- [Soluções para deploy no Airflow](#soluções-de-deployment-do-Airflow)
- [Introdução e tutoriais](#introdução-e-tutoriais)
<!-- - [Videos da conferencia Airflow Summit](#airflow-summit-2020-videos)
- [Boas praticas, lições aprendidas e bons usos de casos](#best-practices-lessons-learned-and-cool-use-cases)
- [Livros, blogs, podcasts e mais](#books-blogs-podcasts-and-such)
- [Apresentação de videos online](#slide-deck-presentations-and-online-videos)
- [Bibliotecas, Hooks, Utilitarios](#libraries-hooks-utilities)
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
- [Tutorial de como instalar Apache Airflow na IBM Cloud](https://github.com/KissConsult/Apache-Airflow) - Tutorial de deploy feito de forma rapida e facil na nuvem IBM com IBM [Bitnami Charts](https://github.com/bitnami/charts)

- [Tres formas de executar o airflow no Kubernetes](https://fullstaq.com/blog/three-ways-to-run-airflow-on-kubernetes/) - [Tim van de Keer](https://www.linkedin.com/in/tim-van-de-keer-bb5a1966) explica por diversas formas como fazer o deploy do Airflow no Kubernetes.
- [Deploy Multi Tier gratuito do Apache Airflow na Azure ](https://azure.microsoft.com/en-us/blog/bitnami-apache-airflow-multi-tier-now-available-in-azure-marketplace/) - Um template gratuito ARM ou Azure Resource Manager feito pela Bitnami oferecendo uma solução de um clique para o deployment para estudos de caso.

- [KubernetesExecutor Helm Chart](https://github.com/tekn0ir/airflow-chart) - Um Helm Chart mais simples usando o KubernetesExecutor para uma experiencia nativa com o Kubernetes ou k8s e que tambem serve para complementar
[KubernetesExecutor Docker Image](https://github.com/tekn0ir/airflow-docker).
- [Stable Celery Helm Chart](https://github.com/helm/charts/tree/master/stable/airflow) - 
Chart Helm do Celery no repositorio oficial

- [Puckel's Docker Image](https://github.com/puckel/docker-airflow) - Feita pelo usuario do twitter [@Puckel_](https://twitter.com/Puckel_) é
uma imagem Docker muito bem planejada que tem chegado como base para muitas instalações no Airflow. Ela é normalmente atualizada e segue muito proxima dos releases oficiais do Apache.
- [Operador customizado do Kubernetes para fazer deploy do Airflow](https://github.com/GoogleCloudPlatform/airflow-operator) - Controlador customizado do Kubernetes(tambem chamado de padrão de operador) para fazer o deploy do Airflow no Kubernetes.
- [airflow-pipeline](https://github.com/datagovsg/airflow-pipeline) - Container docker do Airflow que vem preconfigurado para Spark e Hadoop. Ele pode ser retirado de ``datagovsg/airflow-pipeline``.
- [aws-airflow-stack](https://github.com/villasv/aws-airflow-stack) -Um cluster de deploy baseado na AWS com o CeleryExecutor. Ele faz o deploy apos alguns cliques com CloudFormation

- [kube-airflow](https://github.com/mumoshu/kube-airflow) - Esse repositorio contem uma imagem Docker Airflow (que parece ter sido baseada no trabalho do Puckel) e a definição recente do serviço Kubernetes. O repositorio do usuario [mumoshu](https://github.com/mumoshu) não foi recentemente atualizado mas foram feitos muitos forks que podem ser baseados em mais releases recentes
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
- [Airflow-Component](https://github.com/noelmcloughlin/airflow-component#lightweight-federated-apache-airflow-installer) - Instalador leve da arquitetura  de referencia federated Airflow-Airflow (RabbitMQ) nos nós calculados.

## Introduções e tutoriais
- [Metricas de monitoramento do Apache Airflow](https://youtu.be/xyeR_uFhnD4) - Uma serie em duas partes feita por [maxcotec](https://maxcotec.com) em como voce pode utilizar as metricas existentes do Airflow para monitorar seu deploy da dashboard do Grafana via Prometheus. Tambem aprenda como criar metricas customizadas
- [Introdução ao Airflow](https://www.youtube.com/playlist?list=PLzKRcZrsJN_xcKKyKn18K7sWu5TTtdywh) - Um tutorial em serie web por [maxcotec](https://maxcotec.com) para usuarios iniciantes e intermediarios do Apache Airflow
- [ETL com Apache Airflow para analise de dados em dados transacionais](https://github.com/KimaruThagna/ml-pipelines-airflow). [Kimaru Thagana](https://www.linkedin.com/in/kimaru-thagana-4920b5181/) cobre um caso pratico de fazer o processo de ETL usando Apache Airflow usando um comercio dummy para transações, usuario e dados de produtos. Os dados são entregues via uma API flask.
- [Comece construindo pipelines de dados melhores com Apache Airflow](https://blog.delaplex.com/start-building-better-data-pipelines-with-apache-airflow) - Naman Gupta cobre o basico do Airflow e seus conceitos .
- [Template de repositorio do Airflow](https://github.com/soggycactus/airflow-repo-template) - 
  Um repositorio boilerplate para desenvolver localmente com Airflow com testes para DAGs validas e plugins. Só cole e execute `make start-airflow` para começar. Adicione alguns jobs CI para fazer o deploy do seu codigo quando voce tiver terminado.
- [Como Apache Airflow distribui jobs nos workers Celery](https://blog.sicara.com/using-airflow-with-celery-workers-54cb5212d405) - 
Uma curta descrição dos passos feitos para uma instancia de tarefas para o processo de agendamento ao sucesso em uma arquitetura distribuida
-[Submissão remota do spark para o YARN executando no EMR](https://medium.com/@tamizhgeek/remote-spark-submit-toyarn-running-on-emr-9804b89d82d2) - [Azhaguselvan](https://github.com/tamizhgeek) explica como submeter jobs do Spark para os cluster existentes EMR com Airflow
- [Executando Airflow no topo do Apache Mesos](http://agrajmangal.in/blog/big-data/running-airflow-on-top-of-apache-mesos/) e seu acompanhamento, [Mesos, Airflow & Docker](http://agrajmangal.in/blog/big-data/mesos-airflow-docker/) by [Agraj Mangal](https://twitter.com/agrajm) tem uma revisão rapida de como executar Airflow no Apache Mesos
- [Dustin Stansbury](https://twitter.com/corrcoef) do [Quizlet](https://quizlet.com/) escreveu uma serie de quatro partets que cobre o que gerenciadores de workflow fazer em geral, como Quizlet pegou Airflow um turismo dos conceitos chaves do Airflow e como Quizlet esta agora usando Airflow na pratica:
  - [Alem de CRON uma introdução para os sistemas de gerenciamento em workflow](https://medium.com/@dustinstansbury/beyond-cron-an-introduction-to-workflow-management-systems-19987afcdb5e)
  - [Porque Quizlet escolheu Apache Airflow para executar workflow de dados](https://towardsdatascience.com/why-quizlet-chose-apache-airflow-for-executing-data-workflows-3f97d40e9571)
  - [Entendendo os conceitos chave do Apache Airflow](https://medium.com/@dustinstansbury/understanding-apache-airflows-key-concepts-a96efed52b1a)
  - [Como Quizlet usa o Apache Airflow na pratica](https://medium.com/@dustinstansbury/how-quizlet-uses-apache-airflow-in-practice-a903cbb5626d)
  
- [Integrando Apache Airflow com Databricks](https://databricks.com/blog/2017/07/19/integrating-apache-airflow-with-databricks.html) -   Esse tutorial é focado especificamente nas soluções com Spark do databricks ele tem uma visão razoavel do basico do Airflow e demonstra como uma solução third party pode rapidamente integrar com Airflo
- [Tutorial do Apache Airflow 2.0](https://turbaszek.medium.com/apache-airflow-2-0-tutorial-41329bbf7211) - Esse artigo discute conceitos basicos de como ficar por tras de Airflow e discute os problemas que ele resolve. 
- [Testando e debugando Apache Airflow](https://blog.godatadriven.com/testing-and-debugging-apache-airflow) - Artigo explicando como aplicar teste unitario, mocking e debugging para o codigo do Airflow. 
- [Iniciando desenvolvimento de workflows com Apache Airfloww](http://michal.karzynski.pl/blog/2017/03/19/developing-workflows-with-apache-airflow/) - Esse breve tutorial de introdução cobre como criar um pipeline de dados e processar o workflow usando DAG, operadores, sensor, usar Xcoms para comunicar entre operadores.
- [Iniciando com Airflow + Plataforma Google Cloud + Docker](https://medium.com/@junjiejiang94/get-started-with-airflow-google-cloud-platform-docker-a21c46e0f797) - Introcdução passo a passo por [Jayce Jiang](https://medium.com/@junjiejiang94).
- [Como desenvolver um pipeline de dados no Airflow por teste TDD(test-driven development)](https://blog.magrathealabs.com/how-to-develop-data-pipeline-in-airflow-through-tdd-test-driven-development-c3333439f358) -Aprenda como construir um pipeline de dados usando TDD passo a passo e no fim como configurar um simples workflow CLI usando Github actions.


