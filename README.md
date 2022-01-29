[<img src="https://github.com/jghoman/awesome-apache-airflow/raw/master/airflow-logo.png" align="right">](https://airflow.apache.org/)
# Awesome Apache Airflow
<!-- ![contrib badge](https://img.shields.io/github/contributors/jghoman/awesome-apache-airflow.svg) ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/jghoman/awesome-apache-airflow?style=plastic) -->

Essa é uma lista de referencias sobre o [Apache Airflow](https://airflow.apache.org/).
Por favor sinta-se livre para contribuir com qualquer item que voce gostaria de incluir. Os items são geralmente adicionados no topo de cada seção.

## Conteudo (Ingles)
- [Vital links](#vital-links)
- [Soluções para deploy no Airflow](#airflow-deployment-solutions)
- [Introdução e tutoriais](#introductions-and-tutorials)
- [Videos da conferencia Airflow Summit](#airflow-summit-2020-videos)
- [Boas praticas, lições aprendidas e bons usos de casos](#best-practices-lessons-learned-and-cool-use-cases)
- [Livros, blogs, podcasts e mais](#books-blogs-podcasts-and-such)
- [Apresentação de videos online](#slide-deck-presentations-and-online-videos)
- [Bibliotecas, Hooks, Utilitarios](#libraries-hooks-utilities)
- [Meetups](#meetups)
- [Airflow comercial como um provedor de serviços](#commercial-airflow-as-a-service-providers)
- [Referencias para o Cloud Composer](#cloud-composer-resources)
- [Non-English resources](#non-english-resources)

## Links Essenciais
- [Codigo Fonte](https://github.com/apache/airflow/) (latest stable release [1.10.12](https://github.com/apache/airflow/tree/1.10.12))
- [Documentação](https://airflow.apache.org/) (also the official website)
- [Pagina do confluence](https://cwiki.apache.org/confluence/display/AIRFLOW/Airflow+Home)
- [![Twitter Follow](https://img.shields.io/twitter/follow/apacheairflow?style=social)](https://twitter.com/ApacheAirflow)
- [Area de trabalho no Slack ](https://apache-airflow-slack.herokuapp.com/)

## Soluções de deployment do Airflow 
- [Tutorial de como instalar Apache Airflow na IBM Cloud](https://github.com/KissConsult/Apache-Airflow) - Tutorial de deploy feito de forma rapida e facil na nuvem IBM com IBM[Bitnami Charts](https://github.com/bitnami/charts)

- [Tres formas de executar o airflow no Kubernetes](https://fullstaq.com/blog/three-ways-to-run-airflow-on-kubernetes/) - [Tim van de Keer](https://www.linkedin.com/in/tim-van-de-keer-bb5a1966) explica por diversas formas como fazer o deploy do Airflow no Kubernetes.
- [Deploy Multi Tier gratuito do Apache Airflow na Azure ](https://azure.microsoft.com/en-us/blog/bitnami-apache-airflow-multi-tier-now-available-in-azure-marketplace/) - Um template gratuito ARM ou Azure Resource Manager feito pela Bitnami oferecendo uma solução de um clique para o deployment para estudos de caso.

- [KubernetesExecutor Helm Chart](https://github.com/tekn0ir/airflow-chart) - Um Helm Chart mais simples usando o KubernetesExecutor para uma experiencia nativa com o Kubernetes ou k8s e que tambem serve para complementar
[KubernetesExecutor Docker Image](https://github.com/tekn0ir/airflow-docker).
- [Stable Celery Helm Chart](https://github.com/helm/charts/tree/master/stable/airflow) - 
Chart Helm do Celery no repositorio oficial
