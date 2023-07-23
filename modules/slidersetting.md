# Настройка (слайдер): конструктор
```js
SliderSetting(String name, Double[] parameters); // [стандарт, мин., макс., шаг слайдера]
```

# Настройка (кнопка): методы
## ``SliderSetting.getName();``
**Описание:** получает имя настройки

<details>
<summary> Доп. информация</summary>
**Аргумент(-ы)**:
| Аргумент | Значение |
| -------- | -------- |
| SliderSetting setting | Имя настройки |

**Возвращает:** ``String settingName``

**Пример:**
```js
var setting = new SliderSetting("Позиция по X", [512, 0, 1024, 1]);

setting.getName(); // "Позиция по X"
```
</details>

## ``SliderSetting.getType();``
**Описание:** возвращает тип настройки (``"slider"``)

<details>
<summary>Доп. информация</summary>
**Аргумент(-ы)**:
| Аргумент | Значение |
| -------- | -------- |
| SliderSetting setting | Настройка |

**Возвращает:** ``String settingType``

**Пример:**
```js
var setting = new SliderSetting("Расстояние", [15, 0, 25, 1]);

setting.getType() // "slider"
```
</details>

## ``SliderSetting.isVisible();``
**Описание:** Определяет видимость настройки

<details>
<summary>Доп. информация</summary>

**Аргумент(-ы)**:
| Аргумент | Значение |
| -------- | -------- |
| SliderSetting setting | Настройка |

**Возвращает:** ``Boolean isVisible``

**Пример:**
```js
var setting = new SliderSetting("Задержка (сек.)", [3, 0, 10, 0.5]);
setting.setVisibility(false);

setting.isVisible(); // false
```
</details>

## ``SliderSetting.setVisibility(Boolean visibility);``
**Описание:** Устанавливает (не-)видимость настройке

<details>
<summary>Доп. информация</summary>
**Аргумент(-ы)**:
| Аргумент | Значение |
| -------- | -------- |
| SliderSetting setting | Настройка |
| Boolean visibility | Видимость настройки |
</details>

## ``SliderSetting.getCurrentValue();``
**Описание:** определяет текущее значение слайдера

<details>
<summary>Доп. информация</summary>
**Аргумент(-ы)**:
| Аргумент | Значение |
| -------- | -------- |
| SliderSetting setting | Настройка |

**Возвращает:** ``Double value``

**Пример:**
```js
var setting = new SliderSetting("Количество", [64, 1, 64, 1]);

SliderSetting.getCurrentValue(); // 64, если ранее не менялось
```
</details>

## ``SliderSetting.setOnCurrentValueChangedListener(Function callback);``
**Описание:** устанавливает действие при изменении значения настройки
<details>
<summary>Доп. информация</summary>

**Аргумент(-ы)**:
| Аргумент | Значение |
| -------- | -------- |
| SliderSetting setting | Настройка |
| Function callback | Действие |

**Пример:**
```js
var setting = new SliderSetting("Я - гуль", [990, 990, 1010, 1]);

SliderSetting.setOnCurrentValueChangedListener(function(value) {
    if (value == 993) {
        print("Le-le-let me die");
        Memory.getBoolean(5, 29);
    }
});
```
</details>

