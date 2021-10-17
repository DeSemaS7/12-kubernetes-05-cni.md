# Задание 1: установить в кластер CNI плагин Calico

Собрал кластер через kubespray. Calico по умолчанию.
<br> Cделал 3 деплоймента (hello-world, permitted, restricted) на базе образа praqma/network-multitool
![pods](pods.png)

<br> После этого применил две сетевых политики, одна с полный запретом [ingress](default.yaml), другая разрешает ингресс от подов permitted к hello-world по порту 80
