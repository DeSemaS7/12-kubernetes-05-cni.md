# Задание 1: установить в кластер CNI плагин Calico

Собрал кластер через kubespray. Calico по умолчанию.
<br> Cделал 3 деплоймента (hello-world, permitted, restricted) на базе образа praqma/network-multitool
![pods](pods.png)

<br> После этого применил две сетевых политики, [первая](default.yaml) с полный запретом, а [вторая](hello-world.yaml) разрешает ингресс от подов permitted к hello-world по порту 80.
<br> ![policies](policies.png)

<br>Попробовал курл в разных направлениях. убедился что политика работает корректно.
![curls](curls.png)


# Задание 2: изучить, что запущено по умолчанию

Поигрался с командами. заскринил 3 требуемых вывода.
<br>
![calicoctl](calicoctl.png)
