# onlyrab
UPD: Выпустили большое обновление.
Теперь каждая версия будет иметь номер (текущая имеет 0.9). При покупке раба будет красивый вывод (см. скриншот). Добавлена возможность включать покупку оков для невидимок (советую тем, кто находится в топе или близок к нему).

buy_fetters - покупать ли оковы (0 - выкл, 1 - вкл)
buy_slaves - покупать ли рабов (0 - выкл, 1 - вкл)
invisible_slaves - позволяет покупать невидимых рабов, которые приносят высокую прибыль. Работает только при "buy_slaves": 1. (0 - выкл, 1 - вкл)
invisible_fetters - покупать ли невидимым раба цепи. Работает только при "buy_fetters": 1. Советую, если хотите держать топ. (0 - выкл, 1 - вкл)

В консоль спамит 'balance', 'slaves' или 'id'. Что делать?
Возможные причины такого поведения:

Не хватает баланса на покупку раба.
Неправильный authorization в config.json. Зайдите в игру, проверьте, прибавляется ли количество рабов. Попробуйте заново получить authorization.
Бан на несколько часов. Попробуйте купить раба вручную. Если выходит ошибка ErrFloodBuy, значит у Вас бан на несколько часов. Если бан был получен при использовании этого бота, попробуйте повысить delay в config.json.

Установка на Termux (Android)
Устанавливаем Termux, желательно с F-Droid, т.к. в Google Play разработчик его больше не обновляет.
Запускаем Termux.

Пишем по порядку:
cd
pkg install -y git
git clone https://github.com/hudoils/onlyrab
sh onlyrab/termux.sh
Редактируем файл config.json командой nano onlyrab/config.json по инструкции для Windows или перекидываем с компьютера имеющийся. Как сделать это, можете посмотреть на YouTube или почитать в интернете.
Запуск: sh onlyrab/launch.sh
