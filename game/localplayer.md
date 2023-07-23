# локал. игрок
# локал. игрок: методы (статические)
**Примечание:** здесь практически не будет примеров, т.к. почти везде возвращаемые значения разные
## `LocalPlayer.getNameTag();`
**Описание:** определяет нэймтег (см. примечание) локал. игрока
<details>
<summary>Доп. информация</summary>

**Возвращает:** `String nameTag`

**Примечание:** имя, которое видит локал. игрок (может быть отредактировано сервером (к примеру, для отображения доната))
</details>

## `LocalPlayer.setNameTag(String nameTag);`
**Описание:** изменяет нэймтег (см. примечание) локал. игрока
<details>
<summary>Доп. информация</summary>

**Возвращает:** `String nameTag`

**Примечание:** имя, которое видит локал. игрок (может быть отредактировано сервером (к примеру, для отображения доната))
</details>

## `LocalPlayer.getYaw();` / `LocalPlayer.getPitch();`
**Описание:** определяет угол поворота головы локал. игрока по горизонтали / вертикали
<details>
<summary>Доп. информация</summary>

**Возвращает:** `Double yaw` / 'Double pitch'
</details>

## `LocalPlayer.setRot(Double yaw, Double pitch);`
**Описание:** устанавливает угол поворота головы локальному локал. игроку
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Double yaw | Угол поворота по горизонтали |
| Double pitch | Угол поворота по вертикали |
</details>

## `LocalPlayer.getPositionX();` / `LocalPlayer.getPositionY();` / `LocalPlayer.getPositionZ();`
**Описание:** определяет координату локал. игрока по оси X/Y/Z
<details>
<summary>Доп. информация</summary>

**Возвращает:** `Double posX` / `Double posY` / `Double posZ`
</details>

## `LocalPlayer.setPositionX(Double posX);` / `LocalPlayer.setPositionY(Double posY);` / `LocalPlayer.setPositionY(Double posZ);`
**Описание:** устанавливает координату локал. игрока по оси X/Y/Z
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Double posX / Double posY / Double posZ | Позиция по оси X/Y/Z |
</details>

## `LocalPlayer.setPosition(Double posX, Double posY, Double posZ);`
**Описание:** устанавливает координаты локал. игрока по всем осям
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Double posX | Позиция по оси X |
| Double posY | Позиция по оси Y |
| Double posZ | Позиция по оси Z |
</details>

## `LocalPlayer.getVelocityX();` / `LocalPlayer.getVelocityY();` / `LocalPlayer.getVelocityZ();`
**Описание:** определяет скорость локал. игрока по оси X/Y/Z
<details>
<summary>Доп. информация</summary>

**Возвращает:** `Double velX` / `Double velY` / `Double velZ`
</details>

## `LocalPlayer.setVelocityX(Double velX);` / `LocalPlayer.setVelocityY(Double velY);` / `LocalPlayer.setVelocityZ(Double velZ);`
**Описание:** определяет скорость локал. игрока по оси X/Y/Z
<details>
<summary>Доп. информация</summary>

| Аргумент | Значение |
| -------- | -------- |
| Double velX / Double velX / Double velX | Скорость по оси X/Y/Z | 

</details>

## `LocalPlayer.setVelocity(Double velX, Double velY, Double velZ);`
**Описание:** устанавливает скорость по всем осям
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Double posX | Скорость по оси X |
| Double posY | Скорость по оси Y |
| Double posZ | Скорость по оси Z |
</details>

## `LocalPlayer.getCollisionSize();`
**Описание:** определяет размер хитбокса локал. игрока по вертикали и горизонтали
<details>
<summary>Доп. информация</summary>

**Возвращает:** `Double[] collisionSize`
</details>

## `LocalPlayer.getStatusFlag(Integer flag);`
**Описание:** определяет значение флага локал. игрока
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer flag | ID флага |

**Возвращает:** `Boolean state`
</details>

## `LocalPlayer.setStatusFlag(Integer flag, Boolean status);`
**Описание:** устанавливает значение флага локал. игрока
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer flag | ID флага |
| Boolean status | Значение флага |

</details>

## `LocalPlayer.getFallDistance();`
**Описание:** определяет (текущую) высоту падения локал. игрока
<details>
<summary>Доп. информация</summary>

**Возвращает:** `Double fallDistance`
</details>

## `LocalPlayer.isInCreativeMode();`
**Описание:** определяет режим игры локал. игрока (ВАЖНО: см. примечание)
<details>
<summary>Доп. информация</summary>

**Возвращает:** `Boolean isInCreativeMode`
**Примечание:** может определить только режим креатива и выживания
</details>

## `LocalPlayer.isInLava();` / `LocalPlayer.isInWater();` / `LocalPlayer.isInWall();`
**Описание:** определяет, в лаве/воде/блоке ли локал. игрок (см. примечание)
<details>
<summary>Доп. информация</summary>

**Возвращает:** `Boolean isInLava` / `Boolean isInWater` / `Boolean isInBlock`
**Примечание:** метод проверяет, находится ли локал. игрок в лаве/воде даже частично (находится ли хитбокс локал. игрока в хитбоксе блока лавы/воды/блока)
</details>

## `LocalPlayer.isInvisible();`
**Описание:** определяет, невидим ли локал. игрок
<details>
<summary>Доп. информация</summary>

**Возвращает:** `Boolean isInvisible`
</details>

## `LocalPlayer.isInWorld();`
**Описание:** определяет ??? (см. примечание)
<details>
<summary>Доп. информация</summary>

**Возвращает:** `Boolean isInWorld`
**Примечание:** по сведениям офф. документации, метод проверяет, на сервере ли локал. игрок, но возможно он проверяет на наличие локал. игрока в зоне прорисовки, требует уточнения
</details>

## `LocalPlayer.isOnFire();`
**Описание:** определяет, горит ли локал. игрок (см. примечание)
<details>
<summary>Доп. информация</summary>

**Возвращает:** `Boolean isOnFire'
</details>

## `LocalPlayer.isOnGround();`
**Описание:** определяет, на земле ли локал. игрок (см. примечание)
<details>
<summary>Доп. информация</summary>

**Возвращает:** `Boolean isOnGround`
</details>

## `LocalPlayer.isFalling();`
**Описание:** определяет, падает ли локал. игрок
<details>
<summary>Доп. информация</summary>

**Возвращает:** `Boolean isFalling`
</details>

## `LocalPlayer.isImmobile();`
**Описание:** определяет, может ли локал. игрок двигаться (см. примечание)
<details>
<summary>Доп. информация</summary>

**Возвращает:** `Boolean isImmobile`
**Примечание:** `true` значит, что локал. игрок не может двигаться и наоборот
</details>

## `LocalPlayer.isSitting();`
**Описание:** определяет, сидит ли локал. игрок (например, из-за плагина или в лодке)
<details>
<summary>Доп. информация</summary>

**Возвращает:** `Boolean isSitting`
</details>**

## `LocalPlayer.isSneaking();`
**Описание:** определяет, крадётся ли локал. игрок ("шифтит")
<details>
<summary>Доп. информация</summary>

**Возвращает:** `Boolean isSneaking`
</details>

## `LocalPlayer.isAlive();`
**Описание:** определяет, жив ли локал. игрок (см. примечание)
<details>
<summary>Доп. информация</summary>

**Возвращает:** `Boolean isAlive`
</details>

## `LocalPlayer.isOnLadder();`
**Описание:** определяет, на лестнице ли локал. игрок (см. примечание)
<details>
<summary>Доп. информация</summary>

**Возвращает:** `Boolean isInWater`
**Примечание:** метод не просто проверяет блок, в котором находится локал. игрок
</details>

## `LocalPlayer.canFly();`
**Описание:** определяет, может ли локал. игрок летать
<details>
<summary>Доп. информация</summary>

**Возвращает:** `Boolean canFly`
</details>

## `LocalPlayer.canShowNameTag();`
**Описание:** определяет, виден ли нэймтег локал. игрока
<details>
<summary>Доп. информация</summary>

**Возвращает:** `Boolean canShowNameTag`
</details>
