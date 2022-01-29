[<img src="https://raw.githubusercontent.com/masuta16/awesome-apache-airflow-br/main/master/images/apache-airflow.png" align="right">](https://airflow.apache.org/)
# Awesome Apache Airflow
<!-- ![contrib badge](https://img.shields.io/github/contributors/jghoman/awesome-apache-airflow.svg) ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/jghoman/awesome-apache-airflow?style=plastic) -->

Essa é uma lista de referências sobre o [Apache Airflow](https://airflow.apache.org/).
Por favor sinta-se livre para contribuir com qualquer item que voce gostaria de incluir. Os items são geralmente adicionados no topo de cada seção.

## Conteúdo (Ingles)
- [Links Essenciais](#links-essenciais)
- [Soluções para deploy no Airflow](#soluções-de-deployment-do-Airflow)
<!-- - [Introdução e tutoriais](#introdução-e-tutoriais)
- [Videos da conferencia Airflow Summit](#airflow-summit-2020-videos)
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

- [airflow-k8s-executor-on-GKE](https://github.com/EamonKeane/airflow-GKE-k8sExecutor-helm) - A detailed tutorial to get a scalable, low maintenance airflow kubernetes executor environment deployed on [Google Kubernetes Engine](https://cloud.google.com/kubernetes-engine/) with [helm](https://helm.sh/).
Um tutorial para ter um executor do airflow no ambiente do kubernetes para ser feito o deploy na [Google Kubernetes Engine](https://cloud.google.com/kubernetes-engine/) com [helm](https://helm.sh/).
- [airflow-cookbook](https://github.com/bahchis/airflow-cookbook) - Receitas de como fazer o deploy do Airflow
- [Executando Airflow com Apache Mesos](http://agrajmangal.in/blog/big-data/running-airflow-on-top-of-apache-mesos/) - 
Blog descrevendo como configurar [Mesos](http://mesos.apache.org/) para executar todos os componentes do Airflow. 
- [Integrando Apache Airflow com Apache Ambari ](https://medium.com/@mykolamykhalov/integrating-apache-airflow-with-apache-ambari-ccab2c90173) - [Mykola Mykhalov](https://www.linkedin.com/in/mykola-mykhalov-9079a8107/) explica como usar o [Apache Ambari](https://ambari.apache.org/) para configurar e fazer o deploy de uma instancia do Airflow.
- [Platforma Astronomer ](https://github.com/astronomerio/astronomer) - 
Apache Airflow como um serviço no Kubernetes. Para maiores informações visite https://www.astronomer.io.
- [Imagem Docker Bitnami Airflow ](https://github.com/bitnami/bitnami-docker-airflow) - Uma imagem docker segura e atualizada para Airflow fornecida por Bitnami
- [Imagem Docker de Agendador do Bitnami Airflow ](https://github.com/bitnami/bitnami-docker-airflow-scheduler) - Uma imagem docker segura e atualizada para o agendador de tarefas do Airflow fornecida por Bitnami
 
