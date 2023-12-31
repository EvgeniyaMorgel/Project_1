## Моделирование изменения балансов студентов при помощи SQL

<p>Что нужно было сделать:<p>
<ol>
  <li>Посмотреть на изменения балансов студентов, собранных из CTE</li>
  <li>Создать визуализацию итогового результата</li>
</ol>

<p>Краткое описание решения <p>
  <li>Узнаем, когда была первая транзакция для каждого студента</li>
  <li>Собераем таблицу с датами за каждый календарный день 2016 года</li>
  <li>Создаем CTE, где будут храниться все даты жизни студента после того, как произошла его первая транзакция</li>
  <li>Находим все изменения балансов, связанные с успешными транзакциями</li>
  <li>Находим изменения балансов из-за прохождения уроков</li>
  <li>Создаем CTE «balances» с вычисленными балансами каждого студента</li>
  <li>Посмотрим, как менялось общее количество уроков на балансах студентов</li>
<p>
<p> > <a href="https://github.com/EvgeniyaMorgel/Project_1/blob/main/запрос%201.txt">Запрос</a> <p>
<p>
<p> > <a href="https://github.com/EvgeniyaMorgel/Project_1/blob/main/проект%201.xlsx">Результат запроса</a> <p>  
<p>
<p> > <a href="https://github.com/EvgeniyaMorgel/Project_1/blob/main/проект%201.png">Визуализация</a> <p>



<p>Выводы:<p>
<p>В итоговой таблице можно увидеть, что к концу 2016 года накопительный итог по урокам был: 4534, студентам было начислено больше уроков, чем было пройдено. Если рассматривать прохождение уроков по месяцам, то можно увидеть, что в начале 2016 года интенсивность была небольшой, по сравнению с концом года.
Можно сделать вывод, что к концу года ученики пытались нагнать отставания по урокам, поэтому интенсивность намного выше.
Исходя из выводов выше, можно сказать ,что студенты бросают обучение или медленно проходят уроки, провоцируя тем самым возникновение "хвостов", которые идут на следующий год.
<ol>
