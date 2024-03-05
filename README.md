Проект GitOps включает следующие задачи: 
1.  Установку Argo CD в кластер K8S;
2.  Создание github pages для репозитория;
3.  Создание Dockerfile.multi для сборки и запуска приложения wcg;
4.  Создание Helm Chart для развёртывания приложения wcg в кластер миникуба;
5.  Создание workflow для GitHub Actions со следующими задачами:
     - создание тега новой версии в ветке main;
     - создание docker image из Dockerfile.multi и загрузка его в GitHub packages с тегом новой версии;
     - тестирование Helm Chart, упаковка этого чарта в Helm package с тегом новой версии, добавление Helm package в репозиторий с обновлением helm repo index.
6.  Настройку Argo CD на деплоймент упакованного выше Helm Chart
