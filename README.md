# Лабораторная работа №1
## Задание
<p align="justify">Разработать программу на языке CUDA С  (а также последовательный ее вариант на C/C++) в соответствии с вариантами заданий к лабораторной работе, приведенным в таблице 1.</p>
<p align="justify">Во всех заданиях требуется создать матрицу (вектор) или несколько матриц (векторов) одинаковой размерности, указанной в таблице 1, заполнить их считанными из текстового файла значениями. Текстовые файлы следует предварительно подготовить, заполнив их случайными числами. Затем реализовать задание, используя обработку данных на CUDA. В конце вывести результаты вычислений опять в текстовый файл.</p>
<p align="justify">Интерфейс программы – консольное приложение. В самом начале программа спрашивает имя входного и выходного файлов. Затем, после выполнения всех вычислений, печатает общее время работы (в секундах).</p>
<p align="justify">Также вычислить ускорение и эффективность. Эффективность определить с помощью профилировщика NVIDIA Visual Profiler.</p>
<table border="1">
  <caption>Вариант задания</caption>
  <tr>
    <th>№</th>
    <th>Размерность массива или матрицы</th>
    <th>Тип данных</th>
    <th>Описание задания</th>
  </tr>
  <tr align="center">
    <td>1</td>
    <td>10x10, 10000x10000</td>
    <td>float</td>
    <td>Вычислить матрицу C = ‖A‖ * A + B - A, ‖A‖ –  евклидова норма матрицы</td>
  </tr>
 </table>
 
 <table border="1">
  <caption>Время работы алгоритма</caption>
  <tr>
    <th>Размерность массива или матрицы</th>
    <th>Время линейного алгоритма, сек.</th>
    <th>Время параллельного алгоритма, сек.</th>
  </tr>
  <tr align="center">
    <td>1000x1000</td>
    <td>0.08</td>
    <td>0.03</td>
  </tr>
  <tr align="center">
    <td>5000x5000</td>
    <td>1.67</td>
    <td>0.4</td>
  </tr>
  <tr align="center">
    <td>10000x10000</td>
    <td>6.86</td>
    <td>1.55</td>
  </tr>
  <tr align="center">
    <td>20000x20000</td>
    <td>26.74</td>
    <td>2.25</td>
  </tr>
 </table> 
 
 <table border="1">
  <caption>Ускорение</caption>
  <tr>
    <th>Размерность массива или матрицы</th>
    <th>Ускорение</th>
  </tr>
  <tr align="center">
    <td>1000x1000</td>
    <td>2.67</td>
  </tr>
  <tr align="center">
    <td>5000x5000</td>
    <td>4.17</td>
  </tr>
  <tr align="center">
    <td>10000x10000</td>
    <td>4.42</td>
  </tr>
  <tr align="center">
    <td>20000x20000</td>
    <td>11.88</td>
  </tr>
 </table> 
