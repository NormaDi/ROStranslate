# 4.5 Добавление камеры

Процедура добавления камеры к роботу практически идентична процедуре добавления туловища. Мы добавим камеру к туловищу, но вы можете использовать тот же метод для добавления непосредственно к основанию, если у вашего робота нет туловища. Для нашего Box Robot мы начнем с модели, которая использует те же размеры, что и Kinect для камеры.

Перед просмотром URDF-файлов давайте посмотрим конечный результат, используя следующую команду:

```text
 $ roslaunch rbx2_description box_robot_with_kinect.launch
```

Если _RViz_ все еще не работает:

```text
$ rosrun rviz rviz -d `rospack find rbx2_description`/urdf.rviz
```

Вид в RViz должен выглядеть так:

![](../.gitbook/assets/image%20%2834%29.png)

Как видите, мы смоделировали Kinect, используя три штуки: коробку для основания, цилиндр для опорной стойки и еще одну коробку для корпуса камеры. Давайте теперь рассмотрим детали.





