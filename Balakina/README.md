Программа строит столбчатую диаграмму числа статей за указанный срок (за год), содержащих данное слово в название или аннотации, используя NASA ADS. 
Для работы с кодом необходимо получить API-ключ и записать его в файл apikey, для этого зарегистрируйтесь в системе NASA ADS https://ui.adsabs.harvard.edu и в настройках аккаунта Customize Settings в разделе API token создайте новый ключ. Учтите, что максимальное количество запросов для пользователя составляет 5000.
Параметры поиска в системе, которые можно задать в консоли:
		'-k' ('--keyword') задает ключевое слово поиска в NASA ADS -- обязателен для ввода в строке!
        '-p' ('--pages') задает число страниц для поиска (default=3)
        '-d' ('--days') задает число дней до настоящего момента, на основании которых собирается статистика (default=365)

Пример ввода в консоли для подсчета статей со словом supernova: ./ads_query.py -k supernova -p 10