Основной сниппет компонента, который реализует вывод карты на фронте.

## Параметры

Название					| По умолчанию									| Описание
----------------------------|-----------------------------------------------|------------------------------------------------------------------------------------------
**parent**			        | `0`             								| Идентификатор родителя.
**class**					|    											| Класс объекта.
**list**		     		| `default`    									| Имя списка. К нему будет привязана карта.
**map**		     	    	| `ym2map`    									| ID блока с картой.
**center**		     	    | `[55.72, 37.64]`    							| Центральные координаты карты.
**zoom**		     	    | `10`                							| Приближение карты.
**objects**		     	    |               							    | Массив объектов карты. Если указан, выборка объектов из базы производиться не будет.
**mode**		     	    | `default`            							| Режим сниппета. Варианты: `default`, `mfilter2`
**scripts**		     	    | `1`            							    | Нужно ли подключать скрипты карты.
**jquery**		     	    | `1`            							    | Нужно ли подключать jQuery.
**tpl**		         	    | `tpl.YandexMaps2`        					    | Чанк вывода карты.

## Примеры
### Все объекты класса modDocument
```
{'!YandexMaps2' | snippet : [
    'class' => 'modDocument',
]}
```

### Все объекты класса msProduct
```
{'!YandexMaps2' | snippet : [
    'class' => 'msProduct',
]}
```

### Все объекты пользователей
```
{'!YandexMaps2' | snippet : [
    'class' => 'modUser',
    'map' => 'ym2map-users',
]}
```