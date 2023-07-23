# Настройка (выключатель): конструктор
```js
TextFieldSetting(String name, String tip, String text);  // text = стандарт. значение настройки
```

# Настройка (кнопка): методы
## ``TextFieldSetting.getName();``
**Описание:** получает имя настройки

<details>
<summary> Доп. информация</summary>

**Аргумент(-ы)**: 
| Аргумент | Значение |
| -------- | -------- |
| TextFieldSetting setting | Настройка |

**Возвращает:** ``String settingName``

**Пример:**
```js
var setting = new TextFieldSetting("TEST1", "TEST2", "TEST3")

setting.getName();  // "TEST1"
```
</details>

## ``TextFieldSetting.getType();``
**Описание:** возвращает тип настройки (``"text-field"``)

<details>
<summary>Доп. информация</summary>

**Аргумент(-ы)**:
| Аргумент | Значение |
| -------- | -------- |
| TextFieldSetting setting | Настройка |

**Возвращает:** ``String settingType``

**Пример:**
```js
var setting = new TextFieldSetting("Ignore", "HackerOLEG", "");

setting.getType();  // "text-field"
```
</details>

## ``TextFieldSetting.isVisible();``
**Описание:** Определяет видимость настройки

<details>
<summary>Доп. информация</summary>

**Аргумент(-ы)**:
| Аргумент | Значение |
| -------- | -------- |
| TextFieldSetting setting | Настройка |

**Возвращает:** ``Boolean isVisible``

**Пример:**
```js
var setting = new TextFieldSetting("Block IDs", "1, 2, 3", "0");

setting.isVisible();  // true
```
</details>

## ``TextFieldSetting.setVisibility(Boolean visibility);``
**Описание:** Устанавливает (не-)видимость настройке

<details>
<summary>Доп. информация</summary>

**Аргумент(-ы)**:
| Аргумент | Значение |
| -------- | -------- |
| TextFieldSetting setting | Настройка |
| Boolean visibility | Видимость настройки |
</details>

**Пример:**
```js
var setting = new TextFieldSetting("Block IDs", "1, 2, 3", "0");

setting.setVisibility(false);
setting.isVisible();  // false
```

## ``TextFieldSetting.getText();``
**Описание:** определяет текст в поле

<details>
<summary>Доп. информация</summary>

**Аргумент(-ы)**:
| Аргумент | Значение |
| -------- | -------- |
| TextFieldSetting setting | Настройка |

**Возвращает:** ``String text``

**Пример:**
```js
var setting = new TextFieldSetting("Seed", "835719", "0");

ModeSetting.getCurrentValue();  // "0", если ранее не менялось
```
</details>

## ``TextFieldSetting.setOnTextChangedListener(Function callback);``
**Описание:** устанавливает действие при изменении текста в поле
<details>
<summary>Доп. информация</summary>

**Аргумент(-ы)**:
| Аргумент | Значение |
| -------- | -------- |
| TextFieldSetting setting | Настройка |
| Function callback | Действие |

**Пример:**
```js
var setting = new ModeSetting("Priority targets", "fikusjoy,extinqued", "");

ModeSetting.setOnTextFieldToggleListener(function(text) {
    if (text.toLowerCase() == "lednevok1") {
        java.lang.System.exit(0);
    }
});
```
</details>
