Манифесты для деплоя в k8s сервиса из hw_2.

Манифесты описывают сущности: Deployment, Service, Ingress.

Все манифесты можно применить одной командой 
    
    kubectl apply -f

После применения манифестов GET запрос на http://arch.homework/health отдает {“status”: “OK”}.

В Ingress-е указан  rewrite, который форвардит все запросы с /otusapp/amlet/* на сервис с rewrite-ом пути.