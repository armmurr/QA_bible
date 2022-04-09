# Разница тестирования ПО и железа (Software Vs. Hardware testing)

**Программное обеспечение** ([Software](https://en.wikipedia.org/wiki/Software)) - это управляющий набор инструкций и данных. В информатике и разработке программного обеспечения программное обеспечение - это вся информация, обрабатываемая компьютерными системами, включая программы и данные. Программное обеспечение включает программы, библиотеки и связанные с ними неисполняемые данные, такие как онлайн-документация или цифровые носители. Программное обеспечение и оборудование требуют друг друга, и ни одно из них не может реально использоваться по отдельности. На самом низком уровне программирования исполняемый код состоит из инструкций машинного языка, поддерживаемых отдельным процессором - обычно центральным процессором (ЦП) или графическим процессором (ГП). Машинный язык состоит из групп двоичных значений, обозначающих инструкции процессора, которые изменяют состояние компьютера по сравнению с его предыдущим состоянием.

**Аппаратное обеспечение** (Hardware) - это физическое электронное устройство, промышленное оборудование или компонент компьютера. Примерами оборудования компьютера являются CPU, MB, устройства ввода/вывода и хранения данных (HDD или SSD). Без оборудования программному обеспечению не на чем будет работать. Аппаратное и программное обеспечение взаимодействуют друг с другом, и программное обеспечение сообщает аппаратному обеспечению, какие задачи оно должно выполнять.

**Разница в тестировании ПО и железа**:

В глобальном смысле нам не сильно важна природа объекта тестирования, т.к. принципы особо не меняются. Однако, как говорится, есть нюансы:

* “Железный” баг может легко физически безвозвратно сломать единственный рабочий прототип. Критерии отбора тестов должны учитывать и анализ рисков;
* Само взаимодействие с железом, как и снятие показателей результатов / метрик может потребовать дополнительное оборудование, физические модификации, а также почти наверняка инженерный ум и прямые руки из нужного места;
* Тесты программного обеспечения в отличии от тестов железа виртуальны, их можно копировать и переиспользовать и прогонять сколько потребуется. ПО можно легко изменить и развить с помощью нескольких релизов, в то время как оборудование требует более высоких затрат на изменение и не может быть подвергнуто рефакторингу после производства. Тестировщики должны понимать, что когда оборудование создается, они не могут добавлять к нему новые возможности. Таким образом, тесты подходят только для этой линейки оборудования, и для следующего продукта необходимо будет создать другой набор критериев оценки. Конструкции оборудования также значительно более ограничены из-за конкретных деталей или отраслевых рекомендаций;
* В результате первого различия существуют в тест-кейсах. При использовании кейсов для ПО для выполнения всех запланированных тестов может потребоваться от 50 до 100 шагов, это результат того, что нужно учесть бесчисленное множество вещей и высокого уровня автоматизации тестирования, связанного с гибкой разработкой программного обеспечения. Команды могут использовать инструменты тестирования качества, чтобы отслеживать эти операции и гарантировать, что все идет так, как ожидалось. С другой стороны, этапы тестирования оборудования намного короче и проще и включают всего несколько этапов, чтобы проверить, работает ли продукт. Во-первых, прошивка может быть проверена на исправность. Затем оборудование оценивается, чтобы убедиться, что оно хорошо интегрируется с другими системами и должным образом работает с необходимыми приложениями и операционными системами. Наконец, вся система оценивается по тому, насколько хорошо она соответствует требованиям заказчика и высокоуровневым спецификациям, таким как соответствие (compliance). Аппаратное обеспечение нельзя сильно менять перед выпуском, поэтому важно, чтобы группы выполняли полные тесты для выявления любых слабых мест, которые могут быть присущи продукту.
* Что касается программного обеспечения, управляющего оборудованием, здесь резко может возрасти необходимый технический уровень для тестирования (низкоуровневое понимание работы железа, связки с прошивкой, программирование микроконтроллеров, ассемблер и вот это всё):
  * Embedded operating systems;
  * Device driver and service testing;
  * Multi threaded communications;
  * Synchronising data from multiple external sources;
  * Using data scopes to isolate errors (Hardware vs Software);

Источники:

* [Difference between Hardware and Software](https://www.guru99.com/hardware-vs-software-difference.html)
* [The Difference between Software Testing and Hardware Testing](https://www.techwell.com/techwell-insights/2017/03/difference-between-software-testing-and-hardware-testing?\_\_cf\_chl\_captcha\_tk\_\_=pmd\_dMswbG.OAQqO6tWy60YvKfgPLiHrKsEnWLd1kCA6LF0-1632916018-0-gqNtZGzNAxCjcnBszQjR)
* [software vs hardware testing](http://www.sqaforums.com/forums/general-discussion/43191-software-vs-hardware-testing.html)

Доп. материал:

* [Hardware vs Software Product Testing](https://medium.com/somiacx/hardware-vs-software-product-testing-7c61fb083ddf)
* [Siemens hardware and software testing solutions](https://www.plm.automation.siemens.com/global/en/products/simulation-test/testing.html)