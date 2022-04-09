# Тестирование на отказ и восстановление (Failover and Recovery testing)

_Тестирование отказоустойчивости (failover testing): Тестирование при помощи эмуляции отказов системы или реально вызываемых отказов в управляемом окружении. После вызванного отказа проверяется механизм отказоустойчивости с целью удостовериться, что данные не потеряны или не испорчены, и достигнут оговоренный уровень обслуживания (например, доступности функций или время отклика) (ISTQB)._

Тестирование на отказ и восстановление (Failover and Recovery testing, Disaster Recovery Testing) - подвид тестирования производительности, проверяет тестируемый продукт с точки зрения способности противостоять и успешно восстанавливаться после возможных сбоев, возникших в связи с ошибками ПО, отказами оборудования или проблемами связи/сети. Failover - проверка систем восстановления (или дублирующих основной функционал систем), которые, в случае возникновения сбоев, обеспечат сохранность и целостность данных тестируемого продукта. Методика подобного тестирования заключается в симулировании различных условий сбоя, последующем изучении и оценке реакции защитных систем. В процессе подобных проверок выясняется, была ли достигнута требуемая степень восстановления системы после возникновения сбоя. В отличие от тестирования надежности (Reliability Testing), которое проводится, чтобы найти отказ в конкретной точке, где он происходит, Recovery Testing проводится для проверки того, насколько хорошо система восстанавливается после сбоя или аварии.

Для наглядности рассмотрим некоторые варианты подобного тестирования и общие методы их проведения. Объектом тестирования в большинстве случаев являются весьма вероятные эксплуатационные проблемы, такие как:

* Проблемы с сетью;
* Сбой питания;
* Внешний сервер недоступен (External server not reachable);
* Сервер не отвечает (Server not responding);
* Отсутствует файл dll;
* Перегрузка базы данных;
* Остановленные сервисы/службы;
* Физические условия;
* Внешнее устройство не отвечает;
* Потеря сигнала беспроводной сети;

Источники:

* [What Is Recovery Testing In Software Testing](https://www.softwaretestinghelp.com/recovery-testing-tutorial/)

Доп. материал:

* [Importance of Failover Testing during Test Planning of Safety Critical Systems](https://www.softwaretestinggenius.com/importance-of-failover-testing-during-test-planning-of-safety-critical-systems/)