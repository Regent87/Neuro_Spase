# Neuro_Spase
Логика работы программы:
1) На вход поступают данные в TXT формате:
   - Файлы видимости спутник-станция
   - Фалы расписание пересечения границ
2) Файлы из txt преобразуются в один отсортированный датафрейм
3) Дальше по этому датафрейму пробегается алгоритм окном в 1,5 минуты:
   - На горизонте в 1,5 минуты для каждой станции ищем свободные спутники, которые наиболее эффективно отдадут данные.
   - Дальше будем переключаться по станциям которые закончили передачу и повторять цикл.
5) Полученное расписание переводим в txt по формату задачи

Сама процедура составления расписания занимает в среднем 1,5 минуты. 
Много времени уходит на преобразование данных в удобный формат для работы с ними.

Наш лучший результат при оптимизации расписания выглядит так:
Kinosat передали 333.281ТБ
Zorkii передали 259.22ТБ
Все спутники передали 592.501ТБ
все спутники приняли 654.172ТБ
Ссылка на колаб с демовермией программы прилагается. 
Переходите и пробуйте:
https://colab.research.google.com/drive/1z_KSM4KUoXQwpDFHVTxUWJIh4GImmNO3?usp=sharing
