# Proof-of-Work (PoW) Mining 

---

## Обзор  

Майнинг на основе принципа Proof-of-Work, более известный, как PoW Mining - это процесс
предоставления своего компьютерного оборудования и ресурсов для обработки сетевых
транзакций и создания блоков, составляющих блокчейн (блок-цепочку) в сети Decred.
Каждый раз при создании блока майнером вырабатывается около 30 новых Decred 
монет. Эти монеты затем распределяются следующим образом:

Субсидия | Группа
---     | ---
60%   | PoW майнеры
30%   | PoS голосующие
10%   | Субсидия на развитие Decred

В среднем Вы получите вознаграждение, которое примерно пропорционально
хэшрейту (Hashrate) Вашего майнера и общему хэшрейту сети, когда Вы подключаете
Ваш компьютер для PoW майнинга. Для начала работы у Вас должен быть компьютер с
видеокартой. Большинство видеокарт можно использовать для майнинга (включая "мобильные"
разновидности в некоторых ноутбуках). В целом, последние модели видеокарт работают с
более высокими хешрейтами и, следовательно, получают более высокое вознаграждение (rewards).
---

## Solo Mining или Pool Mining  

> <i class="fa fa-male"></i> индивидуальный майнинг

<i class="fa fa-exclamation-triangle"></i> **индивидуальный майнинг не рекомендуется и не рассмативается в данной документации!** В Decred Network регулярно наблюдается уровень хэша сети до 10 000 Gh/s. индивидуальный майнинг iобычно осуществляется только опытными специалистами или организованными группами с большим количеством GPU, поэтому здесь не рассматривается.

> <i class="fa fa-users"></i> майнинг в пуле

Когда Вы майните в пуле, Ваш хешрейт объединяется с хешрейтами остальными майнеров пула в поисках корректного решения для блока. Вы получите вознаграждение в зависимости от объема работы, которую Ваш майнер выполнит в пуле.
майнинг в пуле распределяет доли на основе найденных блоков, поэтому Вы можете постоянно получать некоторое количество Decred, а не "все или ничего", как в соло-майнинге.

---

## Получение адреса Decred для выведения средств  

Следуя руководству [dcrctl Basics](/getting-started/user-guides/dcrctl-basics.md) создайте адрес для вывода вознаграждения за майнинг.

---

## <i class="fa fa-life-ring"></i> Зарегистрируйтесь на майнинг-пуле

Decred поддерживают следующие майнинг-пулы:

* [<i class="fa fa-external-link-square"></i> http://decredpool.org](http://decredpool.org)
* [<i class="fa fa-external-link-square"></i> http://yiimp.ccminer.org](http://yiimp.ccminer.org)
* [<i class="fa fa-external-link-square"></i> http://coinmine.pl/dcr](http://coinmine.pl/dcr)
* [<i class="fa fa-external-link-square"></i> https://dcr.maxminers.net](https://dcr.maxminers.net)
* [<i class="fa fa-external-link-square"></i> https://dcr.suprnova.cc](https://dcr.suprnova.cc)
* [<i class="fa fa-external-link-square"></i> https://pool.mn/dcr](https://pool.mn/dcr)
* [<i class="fa fa-external-link-square"></i> https://zpool.ca](https://zpool.ca)

Все пулы работают более или менее одинаково, но Вы можете зарегистрироваться в нескольких и посмотреть, какой из них подходит Вам лучше всего.

Выбирайте для майнинга меньший пул, чтобы хешрейт сети был распределен для лучшей децентрализации мощности майнинга!

---

## Драйверы/Программное обеспечение GPU  

Драйверы GPU обычно содержат библиотеки, необходимые для майнинга. Если у Вас возникли трудности с запуском программного обеспечения, возможно, потребуется переустановить и, в частности, проверить, что выбраны именно библиотеки OpenCL (AMD) или CUDA (NVIDIA).

---

## <i class="fa fa-download"></i> Выбор и загрузка программного обеспечения для майнинга

### Официальный Decred Miner (gominer)

Gominer официальный майнер Decred, разработанный и поддерживаемый командой Decred. Это майнер, самый простой в настройке и запуске майнинга, поэтому рекомендуется большинству пользователей. В настоящее время последней версией gominer является **<i class="fa fa-github"></i> [v1.0.0](https://github.com/decred/gominer/releases/)** и Официальные бинарные файлы можно загрузить с **[https://github.com/decred/decred-binaries/releases/tag/v1.0.0](https://github.com/decred/decred-binaries/releases/tag/v1.0.0)**

Обязательно выберите правильную операционную систему (Windows / Linux) и правильную версию для Вашего типа GPU (CUDA для карт NVIDIA, OpenCL / OpenCLADL для карт AMD). Gominer доступен только для 64-битных операционных систем. Руководства пользователя для запуска майнинга с помощью gominer здесь:

- [Windows Pool-Mining](/mining/proof-of-work/pool-mining/gominer/windows.md)

### Неофициальные майнеры

* <i class="fa fa-github"></i> [cgminer](https://github.com/kR105-zz/cgminer) - cgminer популярный майнер для GPU **AMD**, имеющий долгую историю применения для множества различных криптовалют. Более сложен в использовании, чем decred gominer.

* <i class="fa fa-github"></i> [ccminer](https://github.com/tpruvot/ccminer) - ccminer популярный майнер для GPU **NVIDIA**, который также имеет долгую историю использования для множества различных криптовалют. Более сложен в использовании, чем decred gominer.

* <i class="fa fa-github"></i> [sgminer](https://github.com/tpruvot/sgminer) - пользователи GPU **AMD**, работающей под Windows, возможно, захотят загрузить sgminer.

---

## Запуск программного обеспечения 

* Разархивируйте и установите программное обеспечение в выбранное Вами место.
* Откройте путь в командной строке.
* Следуйте инструкциям пула для настройки.
* Запустите майнер.

Перейдите к [PoW Mining FAQ](/faq/proof-of-work-mining.md)
