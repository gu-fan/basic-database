DATABASE
========


Simple DataBase Store


Dev:


docker-compose


Deploy:

k8s


======

postgresql
redis
elastic-search


-----

ik
https://github.com/medcl/elasticsearch-analysis-ik

https://www.elastic.co/guide/en/elasticsearch/reference/6.3/docker.html

curl -XPOST http://localhost:9200/pud/pud/_mapping -H 'Content-Type:application/json' -d'
{
        "properties": {
            "text": {
                "type": "text",
                "analyzer": "ik_max_word",
                "search_analyzer": "ik_smart"
            }
        }

}'

curl -XPOST http://localhost:9200/pud/pud/_mapping -H 'Content-Type:application/json' -d'
{
        "properties": {
            "title": {
                "type": "text",
                "analyzer": "ik_max_word",
                "search_analyzer": "ik_smart"
            }
        }

}'


curl http://localhost:9200/pud/pud/_mapping -H 'Content-Type:application/json'

https://n3xtchen.github.io/n3xtchen/elasticsearch/2017/07/05/elasticsearch-23-useful-query-example
