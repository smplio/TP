# Yet Another RTS Game
Игра будет предствалять собой идейное развитие, или же дополнение, к уже известной игре Rise of Nations

# Архитектура
В игре существует некоторый набора наций (возможно будет расширяться) у каждой из которых будут свои особенности.
На данный момент реализовано только 2 нации:
1) Швеция
2) Украина

Так же в игре пирисутсвуют определённые типы юнитов:
+ cavalryUnit
+ meleeUnit
+ archerUnit

Отличаются они, очевидно уроном, скоростью атаки, ренжом, итд, но для нас главное их отличие - 3Д модели, которые у них будут (честно).
Для каждой из наций для каждого типа юнитов используются фабрики, которые и создают юнитов. Создано их столько (колво наций * 3) из-за
необходимости изменять параметры юнитов в зависимости от текущей эпохи (да-да, это игра про эволюцию,или, скорее, развитие народа)
# Процесс игры
1. Игрок (Player) заходит игру, в некотором диалоге у него спрашивают, за какую нацию (Nation) он хочет играть
2. В зависисмости от выбора нации игроку присваиваются фабрики (Factories (на самом деле это 3 разных фабрики для 3 разных классов юнитов, но в схеме я их объеденил в 1 слово)) выбранной нации для всех типов юнитов
3. ???
4. Игра

# P.S.
Вопреки заявлению [Циона Михаила](https://github.com/MVCionOld) из его архитектуры я ничего не заимствовал, это всё клевета
