# Numerical_methods_Interpolation

Интерполирование полиномами Лагранжа
---

                                                              Дана функция
                                                              
                                                       ![equation](https://latex.codecogs.com/gif.latex?f%28x%29%3D%5Cfrac%7B1%7D%7B1&plus;25x%5E2%7D)
где _x_ ∈ [-1; 1]

1. Разработана функцию `l_i(i, x, x_nodes)`, которая возвращает значение i-го базисного полинома Лагранжа, заданного на узлах с абсциссами _x_nodes_, в точке _x_.

2. Написана функция `L(x, x_nodes, y_nodes)`, которая возвращает значение интерполяционного полинома Лагранжа, заданного на узлах с абсциссами _x_nodes_ и ординатами _y_nodes_, в точке _x_.

3. Для равномерно расположенных узлов на экран были выведены одновременно графики `f(x)` и полученного интерполяционного полинома `L(x)` для нескольких различных количеств узлов. 

4. Предыдущий пункт был реализован также для чебышевских узлов.

Интерполяция кубическими сплайнами
---

1. Разработана функция `qubic_spline_coeff(x_nodes, y_nodes)`, которая посредством решения матричного уравнения вычисляет коэффициенты естественного кубического сплайна. 

2. Написана функция `qubic_spline(x, qs_coeff)` и `d_qubic_spline(x, qs_coeff)`, которые вычисляют соответственно значение кубического сплайна и его производной в точке _x_ ( _qs_coeff_ обозначает матрицу коэффициентов).

3. Используя материалы интернет-ресурса по адресу https://data.worldbank.org/indicator/NY.GDP.MKTP.CD, были найдены данные о динамике ВВП Российской Федерации. 

4. Для тех же данных была проведена интерполяция Лагранжа, используя уже написанный код.
