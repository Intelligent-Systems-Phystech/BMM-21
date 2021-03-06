Дедлайн: 16 марта, 23.59.

Ноутбуки сохранять с названием в формате SurnameTask5.ipynb


Перед выполнением задания --- укажите себя в исполнителях, чтобы не было дублей.


# Оформление задания
Задание сдается в jupyter notebook. Структура:
* Заголовок ноутбука
* Описание задания
* Код
* Визуализация
* Краткий комментарий, выводы

Задание оценивается по критериям:
* Корректность
* Наглядность
* Адекватность кода
* Оформление результатов
* Перекрестная защита результатов


# Список заданий

1. [Исполнитель: Панкратов] Визуализировать (интерактивным графиком или анимацией) сходимость распределения invertible gaussian reparametrization. Провести оптимизацию вида KL(q|p) -> min, где q и p принадлежат одному семейству, параметры распределений должны сэмплироваться случайно при каждом запуске визуализации.
График: симплекс (треугольник) с изменением плотности в зависимости от шага оптимизации.
* [IGR](https://arxiv.org/pdf/1912.09588.pdf)
* [Пример визуализации плотности на симплексе](http://blog.bogatron.net/blog/2014/02/02/visualizing-dirichlet-distributions/)


2. [Исполнитель: Филатов] сравнить стратегии Probability of Improvement, Expected Improvement, GP Upper Confidence Bound для оптимизации гиперпараметров гауссовым процессом.  Визуализировать, аналогично рисункам 1.a,1.b,1.c из статьи. Проинтерпретировать полученные результаты
* [Статья](https://arxiv.org/pdf/1206.2944.pdf)

3. [Исполнитель: Сафиуллин] повторить эксперимент с оптимизацией функции "Expected Improvement per second" для выбора оптимальных параметров. Выборка: CIFAR-10 (допускатеся использование подвыборки меньшего объема). 
* [Статья](https://arxiv.org/pdf/1206.2944.pdf)

4. [Исполнитель: Бишук] повторить эксперимент с предобучением моделей RBM и без предобучения (рисунок 3 из статьи).
* [Статья](http://proceedings.mlr.press/v9/erhan10a/erhan10a.pdf)

5. [Исполнитель: Гребенькова] повторить эксперимент с предобучением моделей denoising-автокодировщика и без предобучения (рисунок 3 из статьи).
* [Статья](http://proceedings.mlr.press/v9/erhan10a/erhan10a.pdf)

6. [Исполнитель: TODO] Визуализировать порождение сэмплов из RBM на выборке MNIST (Gibbs sampling):
	* x_0 - из выборки
	* h_0 ~ p(h_0|x_0)
	* x_1 ~ p(x_1|h_0)
	...
	* x_k ~ p(x_k|h_{k-1})
	
показать, как меняются сэмплы в зависимости от шага k (можно анимированным графиком).

* [DL book](https://www.deeplearningbook.org/contents/generative_models.html)
* [статья на medium](https://medium.com/datatype/restricted-boltzmann-machine-a-complete-analysis-part-3-contrastive-divergence-algorithm-3d06bbebb10c)

7. [Исполнитель: Шокоров] визуализировать задачу регрессии с применением гауссового процесса. Показать, как меняется предсказание в зависимости от гиперпараметров гауссового процесса. 
Выборка: одна из стандартных выборок из sklearn.

* [выборки](https://scikit-learn.org/stable/datasets/toy_dataset.html)

