# ModuleManager: методы (статические)
## `ModuleManager.addModule(Module module);`
**Описание:** добавляет модуль в меню клиента
<details>
<summary>Доп. информация</summary>

**Аргументы:**

| Аргумент | Значение |
| -------- | -------- |
| Module module | Модуль |

**Возвращает:** нет

**Пример:**
```js
var module = new Module("AutoLava", true, true, ModuleCategory.PLAYER);

ModuleManager.addModule(module);
```
</details>

## `ModuleManager.addModules(Module[] modules);`
**Описание:** добавляет модули в меню клиента
<details>
<summary>Доп. информация</summary>

**Аргументы:**

| Аргумент | Значение |
| -------- | -------- |
| Module[] modules | Массив модулей |

**Возвращает:** нет

**Пример:**
```js
var module1 = new Module("PasswordCracker", true, true, ModuleCategory.MISC);
var module2 = new Module("ExploitFinder", true, true, ModuleCategory.OTHER);

ModuleManager.addModules([module1, module2]);
```
</details>

## `ModuleManager.removeModule(Module module);`
**Описание:** удаляет модуль из меню клиента
<details>
<summary>Доп. информация</summary>

**Аргументы:**

| Аргумент | Значение |
| -------- | -------- |
| Module module | Модуль |

**Возвращает:** нет

**Пример:**
```js
var module = new Module("BlockReplacer", true, true, ModuleCategory.PLAYER); ModuleManager.addModule(module);

ModuleManager.removeModule(module);
```
</details>

## `ModuleManager.removeModules(Module[] modules);`
**Описание:** удаляет модули из меню клиента
<details>
<summary>Доп. информация</summary>

**Аргументы:**

| Аргумент | Значение |
| -------- | -------- |
| Module[] modules | Массив модулей |

**Возвращает:** нет

**Пример:**
```js
var module1 = new Module("MobKiller", true, true, ModuleCategory.MISC); ModuleManager.addModule(module1);
var module2 = new Module("TEST", true, true, ModuleCategory.MISC); ModuleManager.addModule(module2);

ModuleManager.removeModules([module1, module2]);
```
</details>

## `ModuleManager.getModuleNames();`
**Описание:** даёт названия всех модулей в меню клиента
<details>
<summary>Доп. информация</summary>

**Аргументы:** нет

**Возвращает:** `String[] moduleNames`

**Пример:**
```js
ModuleManager.getModuleNames(); // [AimBot, AntiBot... Script manager]
```
</details>
