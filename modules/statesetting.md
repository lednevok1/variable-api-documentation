# Настройка (выключатель): конструктор
```js
StateSetting(String name, Boolean state);
```

# Настройка (кнопка): методы
## ``StateSetting.getName();``
**Описание:** получает имя настройки

<details>
<summary> Доп. информация</summary>

**Аргумент(-ы)**: 
| Аргумент | Значение |
| -------- | -------- |
| StateSetting setting | Настройка |

**Возвращает:** ``String settingName``

**Пример:**
```js
var setting = new StateSetting("Fix \"Дуели\"");

setting.getName();  // "Fix "Дуели""
```
</details>

## ``StateSetting.getType();``
**Описание:** возвращает тип настройки (``"state"``)

<details>
<summary>Доп. информация</summary>

**Аргумент(-ы)**:
| Аргумент | Значение |
| -------- | -------- |
| StateSetting setting | Настройка |

**Возвращает:** ``String settingType``

**Пример:**
```js
var setting = new StateSetting("Include mobs", true);

setting.getType();  // "state"
```
</details>

## ``StateSetting.isVisible();``
**Описание:** Определяет видимость настройки

<details>
<summary>Доп. информация</summary>

**Аргумент(-ы)**:
| Аргумент | Значение |
| -------- | -------- |
| StateSetting setting | Настройка |

**Возвращает:** ``Boolean isVisible``

**Пример:**
```js
var setting = new StateSetting("Delay", false);

setting.isVisible();  // true
```
</details>

## ``StateSetting.setVisibility(Boolean visibility);``
**Описание:** Устанавливает (не-)видимость настройке

<details>
<summary>Доп. информация</summary>

**Аргумент(-ы)**:
| Аргумент | Значение |
| -------- | -------- |
| StateSetting setting | Настройка |
| Boolean visibility | Видимость настройки |
</details>

**Пример:**
```js
var setting = new StateSetting("Ignore friends", false);

setting.setVisibility(false);
setting.isVisible();  // false
```

## ``StateSetting.isActive();``
**Описание:** определяет, включён ли выключатель

<details>
<summary>Доп. информация</summary>

**Аргумент(-ы)**:
| Аргумент | Значение |
| -------- | -------- |
| StateSetting setting | Настройка |

**Возвращает:** ``Boolean isActive``

**Пример:**
```js
var setting = new StateSetting("Visibility check", true);

ModeSetting.getCurrentValue(); // true, если ранее не менялось
```
</details>

## ``StateSetting.setOnStateToggleListener(Function callback);``
**Описание:** устанавливает действие при включении (выключении) настройки
<details>
<summary>Доп. информация</summary>

**Аргумент(-ы)**:
| Аргумент | Значение |
| -------- | -------- |
| StateSetting setting | Настройка |
| Function callback | Действие |

**Пример:**
```js
var setting = new ModeSetting("Поиск пидорасов", false);

ModeSetting.setOnStateToggleListener(function(isActive) {
    if (isActive) {  // лично у меня приколы с isActive, поэтому можно воспользоваться (State-)Setting.isActive()
        getContext().runOnUiThread({ run() {
            print("Функция поиска пидорасов активирована...");
        }});
    }
});
```
</details>

