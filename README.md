# hse_hw2_chip
### Введение
В данном практическом задании мы научились определять участки генома, где присутствует определенная гистоновая модификация в конкретном типе клеток с помощью анализа ChIP-Seq данных.

Ссылка на мой google colab: https://colab.research.google.com/drive/1gEAN0uXJMnAyRK_XTCmjVKJ630DFqUsT?usp=sharing
 
 ### Вводные данные для исследования
 > Клеточная линия: PC-9
 > 
 > Гистоновая метка: H3K4me3
 
 ### Анализ FastQC
 Все html-файлы, полученные в ходе выполнения исследования из домашнего задания, находятся в папке [reports](https://github.com/galkinamariia/hse_hw2_chip/tree/main/reports).
 
 ### Реплика №1 - ENCFF792HPJ

![image](https://user-images.githubusercontent.com/59726719/157740692-6019429e-039e-4f87-b9c0-db7a11e60858.png)
![image](https://user-images.githubusercontent.com/59726719/157740916-76cf11ef-8032-40f2-9630-b34c5b8157ce.png)
![image](https://user-images.githubusercontent.com/59726719/157740981-80a4d3d8-c38c-42bf-a70d-88e690479d27.png)
![image](https://user-images.githubusercontent.com/59726719/157741086-43a8d060-f48c-4f2f-ae8d-91a1bd6160c8.png)
![image](https://user-images.githubusercontent.com/59726719/157741180-7cd542fc-1ebd-4939-a496-4c8909859e30.png)
![image](https://user-images.githubusercontent.com/59726719/157741265-621fa323-4db5-4dbe-b6be-cd17944467c6.png)

> Вывод: качество прочтений хорошее, всё находится в зеленой зоне, также нет лишних адаптеров.

 ### Реплика №2 - ENCFF920HHA

![image](https://user-images.githubusercontent.com/59726719/157741782-a186b596-2225-4ca1-9a56-f13a74315e55.png)
![image](https://user-images.githubusercontent.com/59726719/157741926-22946607-1c89-480f-9cfd-8171f8f930d8.png)
![image](https://user-images.githubusercontent.com/59726719/157741955-1715956d-d2cf-48d3-bbb7-57e59c2969ba.png)
![image](https://user-images.githubusercontent.com/59726719/157742270-a01b2364-da35-4178-ab15-e0debf87d273.png)
![image](https://user-images.githubusercontent.com/59726719/157742086-75e44f15-8b97-4228-b7db-f75e7f71c274.png)
![image](https://user-images.githubusercontent.com/59726719/157742134-e7168d6a-f513-498a-9855-4b36b8a25d70.png)

> Вывод: также качество прочтений хорошее, всё находится в зеленой зоне, также нет лишних адаптеров.

 ### Контроль - ENCFF486LTO
 
![image](https://user-images.githubusercontent.com/59726719/157742518-fd180ce2-336e-4d37-b93b-6c6af0185649.png)
![image](https://user-images.githubusercontent.com/59726719/157742554-50ea88b7-eaf3-46ff-8f47-56cc22e05bd6.png)
![image](https://user-images.githubusercontent.com/59726719/157742588-143d5c99-67ba-437a-aacc-f8a0a323d9f0.png)
![image](https://user-images.githubusercontent.com/59726719/157742624-79caf26c-ff68-4210-b1b0-db67d0ade449.png)
![image](https://user-images.githubusercontent.com/59726719/157742674-372a51fb-2e92-4423-991a-890b76da00d7.png)
![image](https://user-images.githubusercontent.com/59726719/157742718-c9484ea2-4429-4a3b-9bbf-e9d39051c4dd.png)

> Вывод: качество прочтений также хорошее, всё находится в зеленой зоне, лишние адаптеры отсутствуют.

### Подрезание чтений

![image](https://user-images.githubusercontent.com/59726719/157743502-36c81bac-9007-4ffc-a97a-c8e0254bfd1d.png)
![image](https://user-images.githubusercontent.com/59726719/157743561-22dbbf30-0508-44e4-995b-c2c13d6629ec.png)
![image](https://user-images.githubusercontent.com/59726719/157743592-f80e8c11-23a4-433e-ac9c-0ede3b5d6202.png)
![image](https://user-images.githubusercontent.com/59726719/157743631-4caf9365-cee0-4177-8c0f-6750344cfbf0.png)
![image](https://user-images.githubusercontent.com/59726719/157743693-a17cd7b9-15f6-4066-ad91-81d1c8d4f8de.png)
![image](https://user-images.githubusercontent.com/59726719/157743727-09cfe503-957a-4f8e-a420-eb2997d4c2c9.png)

> Вывод: аналогично, качество прочтений хорошее, всё находится в зеленой зоне, лишние адаптеры отсутствуют.

### Полученная статистика по выравниванию на 14-ю хромосому
> ID - ENCFF792HPJ: всего ридов - , уникально выровнялось - , неуникально выровнялось - , не выровнялось - .
> ID - ENCFF920HHA: всего ридов - , уникально выровнялось - , неуникально выровнялось - , не выровнялось - .
> ID - ENCFF486LTO: всего ридов - , уникально выровнялось - , неуникально выровнялось - , не выровнялось - .

Процент выравниваний получился таким из-за того, что была взята одна хромосома незначительного размера.
 
 ### Диаграммы Эйлера-Венна


