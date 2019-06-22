[Levels Ranks] - Core
===========================

[Levels Ranks] Core - это плагин статистики, который для вас станет прекрасной заменой другим статистикам, как RankMe, Sod Stats и им подобные. Суть его проста, вы выполняете различные игровые действия и получаете/теряете за это очки опыта, при накоплении/потере определенного кол-ва которых, вы получаете определенный ранг.

ВИДЫ СТАТИСТИКИ:
------------

- Накопительный ( lr_type_statistics 0 )
	- Суть в том, что вы начинаете с самого низшего звания и вы должны накапливать очки опыта, начиная с 0. И чем больше вы играете, тем выше звание.
​
- Рейтинговый :: Расширенный ( lr_type_statistics 1 )
	- Данный вид статистики является аналогом HlstatsX. Суть его в том, что вы получаете среднее звание и 1000 очков опыта. И в зависимости от того, как вы умеете играть и насколько хорошо, зависит и ваше звание.
​
- Рейтинговый :: Простой ( lr_type_statistics 2 )
	- Данный вид статистики является аналогом RankMe. Суть данного вида такая же, как и у вида статистики выше (рейтинговый расширенный), но здесь отсутствуют дополнительные бонусы, отсутствует умножающий коэффициент для регулирования статистики, а также в этом виде заложена другая формула подсчета очков опыта.

УСТАНОВКА
------------

- Удалите прошлую версию плагина, если есть.

- Распакуйте содержимое по папкам.

- Настройте файлы:
	- addons/sourcemod/configs/databases.cfg
	- addons/sourcemod/configs/levels_ranks/settings.ini
	- addons/sourcemod/configs/levels_ranks/settings_ranks.ini
	- addons/sourcemod/configs/levels_ranks/settings_stats.ini​
	
- Перезапустить сервер

НАСТРОЙКА - databases.cfg
------------

- Если вы собираетесь использовать БД SQLite, то ничего не нужно настраивать и добавлять

- Если вы собираетесь использовать БД MySQL, то вы должны добавить строки, которые даны ниже, в "addons/sourcemod/configs/databases.cfg", а затем отредактировать как вам требуется:

```
	"levels_ranks"
	{
		"driver"	"mysql" 
		"host"	"host" 
		"database"	"database" 
		"user"	"login" 
		"pass"	"password"
	}
```
