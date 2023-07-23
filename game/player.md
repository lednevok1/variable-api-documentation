# Игрок
# Игрок: методы (статические)
**Примечание:** здесь практически не будет примеров, т.к. почти везде возвращаемые значения разные
## `Player.isLocalPlayer(Integer id);`
**Описание:** определяет, является ли игрок LocalPlayer'ом (см. [Игрок (локальный) (localplayer.md)](documentation/game/localplayer.md))
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `Boolean isLocalPlayer`
</details>

## `Player.getNameTag(Integer id);`
**Описание:** определяет нэймтег (см. примечание) игрока
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `String nameTag`

**Примечание:** имя, которое видит игрок (может быть отредактировано сервером (к примеру, для отображения доната))
</details>

## `Player.setNameTag(Integer id, String nameTag);`
**Описание:** изменяет нэймтег (см. примечание) игрока
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |
| nameTag | Новый неймтег |

**Возвращает:** `String nameTag`

**Примечание:** имя, которое видит игрок (может быть отредактировано сервером (к примеру, для отображения доната))
</details>

## `Player.getYaw(Integer id);`
**Описание:** определяет угол поворота головы игрока по горизонтали
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `Double yaw`
</details>

## `Player.getPitch(Integer id);`
**Описание:** определяет угол поворота головы игрока по вертикали
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `Double pitch`
</details>

## `Player.getPositionX(Integer id);`
**Описание:** определяет координату игрока по оси X
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `Double posX`
</details>

## `Player.getPositionY(Integer id);`
**Описание:** определяет координату игрока по оси Y
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `Double posY`
**Примечание:** значения могут быть очень странными, например, если игрок висит в полёте, его скорость >1000000, а если стоит на земле, ~-0.07
</details>

## `Player.getPositionZ(Integer id);`
**Описание:** определяет координату игрока по оси Z
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `Double posZ`
</details>

## `Player.getVelocityX(Integer id);`
**Описание:** определяет скорость игрока по оси X
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `Double velX`
</details>

## `Player.getVelocityY(Integer id);`
**Описание:** определяет скорость игрока по оси Y
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `Double velY`
</details>

## `Player.getVelocityZ(Integer id);`
**Описание:** определяет скорость игрока по оси Z
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `Double velZ`
</details>

## `Player.getCollisionSize(Integer id);`
**Описание:** определяет размер хитбокса игрока по вертикали и горизонтали
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `Double[] collisionSize`
</details>

## `Player.setCollisionSize(Integer id, Double horizontalSize, Double verticalSize);`
**Описание:** Устанавливает размер хитбокса игрока по вертикали и горизонтали
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |
| Double horizontalSize | Размер хитбокса по горизонтали |
| Double verticalSize | Размер хитбокса по вертикали |
</details>

## `Player.setShadowRadius(Integer id, Double radius);`
**Описание:** Устанавливает радиус (размер) тени игроку
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |
| Double radius | Радиус (размер) тени |
</details>

## `Player.getStatusFlag(Integer id, Integer flag);`
**Описание:** определяет значение флага (см. примечание) игрока
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |
| Integer flag | ID флага |

**Возвращает:** `Boolean state`
</details>

## `Player.getFallDistance(Integer id);`
**Описание:** определяет (текущую) высоту падения игрока
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `Double fallDistance`
</details>

## `Player.isInCreativeMode(Integer id);`
**Описание:** определяет режим игры игрока (ВАЖНО: см. примечание)
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `Boolean isInCreativeMode`
**Примечание:** может определить только режим креатива и выживания
</details>

## `Player.isInLava(Integer id);`
**Описание:** определяет, в лаве ли игрок (см. примечание)
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `Boolean isInLava`
**Примечание:** метод проверяет, находится ли игрок в лаве даже частично (находится ли хитбокс игрока в хитбоксе блока лавы)
</details>

## `Player.isInvisible(Integer id);`
**Описание:** определяет, невидим ли игрок
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `Boolean isInvisible`
</details>

## `Player.isInWall(Integer id);`
**Описание:** определяет, в блоке ли игрок (см. примечание)
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `Boolean isInBlock`
**Примечание:** метод проверяет, находится ли игрок в блоке даже частично (находится ли хитбокс игрока в хитбоксе блока)
</details>

## `Player.isInWater(Integer id);`
**Описание:** определяет, в воде ли игрок (см. примечание)
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `Boolean isInWater`
**Примечание:** метод проверяет, находится ли игрок в воде даже частично (находится ли хитбокс игрока в хитбоксе блока воды)
</details>

## `Player.isInWorld(Integer id);`
**Описание:** определяет ??? (см. примечание)
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `Boolean isInWorld`
**Примечание:** по сведениям офф. документации, метод проверяет, на сервере ли игрок, но возможно он проверяет на наличие игрока в зоне прорисовки, требует уточнения
</details>

## `Player.isOnFire(Integer id);`
**Описание:** определяет, горит ли игрок (см. примечание)
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `Boolean isOnFire'
</details>

## `Player.isOnGround(Integer id);`
**Описание:** определяет, на земле ли игрок (см. примечание)
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `Boolean isOnGround`
</details>

## `Player.isFalling(Integer id);`
**Описание:** определяет, падает ли игрок
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `Boolean isFalling`
</details>

## `Player.isImmobile(Integer id);`
**Описание:** определяет, может ли игрок двигаться (см. примечание)
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `Boolean isImmobile`
**Примечание:** `true` значит, что игрок не может двигаться и наоборот
</details>

**## `Player.isSitting(Integer id);`
**Описание:** определяет, сидит ли игрок (например, из-за плагина или в лодке)
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `Boolean isSitting`
</details>**

## `Player.isSneaking(Integer id);`
**Описание:** определяет, крадётся ли игрок ("шифтит")
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `Boolean isSneaking`
</details>

## `Player.isSneaking(Integer id);`
**Описание:** определяет, жив ли игрок (см. примечание)
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `Boolean isAlive`
</details>

## `Player.isOnLadder(Integer id);`
**Описание:** определяет, на лестнице ли игрок (см. примечание)
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `Boolean isInWater`
**Примечание:** метод не просто проверяет блок, в котором находится игрок
</details>

## `Player.canFly(Integer id);`
**Описание:** определяет, может ли игрок летать
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `Boolean canFly`
</details>

## `Player.canShowNameTag(Integer id);`
**Описание:** определяет, виден ли нэймтег игрока
<details>
<summary>Доп. информация</summary>

**Аргументы:**
| Аргумент | Значение |
| -------- | -------- |
| Integer id | UID игрока |

**Возвращает:** `Boolean canShowNameTag`
</details>
