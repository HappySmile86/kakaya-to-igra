Единственной сценой в проекте является PlatformerDemo.unity, она же является основной сценой. 

Элементы сцены:
1. камера, через котороую мы видим игровое пространство
2. персонаж (объект игрока, player)
3. задний фона
4. источник света 
5. тайловый уровень (tilemap). Тайловый уровень состоит из большого количества заранее заготовленых объектов (тайлов)
6. декоративная трава
7. также в файлах проекта лежит рычаг, но на сцене я его не нашел

Из них префабами являются:
1. персонаж
2. задний фон
3. трава
4. рычаг

Компоненты объекта игрока:
1. SpriteRenderer, спрайт персонажа
2. Animator, анимации
3. Rigidbody 2D, физика объекта
4. Capsule Collider 2D, колизия сапсульной формы
5. Player Character (Script), характеристики персонажа (хп, высота прыжка, урон от падения и т.д.)
6. Character Anim (Script), связь действий и анимаций
7. Character Hold item (Script), что-то вроде держания объекта (?)

Через инспектор можно настроить:
Position, Rotation, Scale, Color, Flip, Draw mode, Mask Interaction, Sprite Sort Point, Material, Sorting Layer, Order in Layer, Conroller (Animator), Body Type, Mass, Linear Damping, Angular Damping, Gravity Scale, Collusion Detection, Sleeping mode, Interpolate, (offset, Size (Collider)), Direction, Player_id, Max_hp, Invunerable, Move_accel, Move_deccel, Move_max, Can_jump, Double_jump, Jump_strength, Jump_time_min, Jump_time_max, Jump_gravity, Jump_fall_gravity, Jump_move_percent, Ground_layer, Ground_raycast_dist, Can_crouch, Crouch_coll_percent, Reset_when_fall, Fall_pos_y, Fall_damage_percent

Скрипты в проекте:
1. CarryItem - описывает свойство объекта, быть взятым игроком
2. CharacterAnim - свзывает анимации персонажа с его действиями
3. CharacterHoldItem - способность персонажа брать объект
4. FollowCamera - описывает движение камеры (зафиксирована на игроке)
5. Lever - описывает работу рычага (переключателя)
6. ParallaxBackground - добавляет эффект параллакса
7. PlayerCharacter - описывает основные характеристики персонажа
8. PlayerControls - управление персонажем, смотрит ввод пользователя
9. TheAudio - скрипт для проигрывания звука