### 1. [Исполнитель: TODO]
Визуализировать порождение сэмплов из RBM на выборке MNIST (Gibbs sampling):
* x_0 - из выборки
* h_0 ~ p(h_0|x_0)
* x_1 ~ p(x_1|h_0)
...
* x_k ~ p(x_k|h_{k-1})
	
показать, как меняются сэмплы в зависимости от шага k (можно анимированным графиком).

* [DL book](https://www.deeplearningbook.org/contents/generative_models.html)
* [статья на medium](https://medium.com/datatype/restricted-boltzmann-machine-a-complete-analysis-part-3-contrastive-divergence-algorithm-3d06bbebb10c)


### 2. [Исполнитель: TODO] 
Просэмплировать варианты нейросетей по сетке, сделать 3d-график, каждая точка которого соответствует модели, а координаты:
* Количество параметров нейросети
* Точность модели
* Устойчивость модели под действием adverarial-атак (рекомендуется брать FGSM, параметр epsiilon подобрать самостоятельно из соображений наглядности графика)
На графике также отметить парето-оптимальный фронт. Допускается использование логарифмической шкалы для наглядности.

Сетка нейросетей: полносвязные нейросети с 1, 2, 3 и 0 (логистическая регрессия) количеством слоев. Количество точек на графике должно быть не менее 20.

Выборка: Fasion-MNIST.

* [Парето-оптимальный фронт](https://ru.wikipedia.org/wiki/%D0%9C%D0%BD%D0%BE%D0%B3%D0%BE%D0%BA%D1%80%D0%B8%D1%82%D0%B5%D1%80%D0%B8%D0%B0%D0%BB%D1%8C%D0%BD%D0%B0%D1%8F_%D0%BE%D0%BF%D1%82%D0%B8%D0%BC%D0%B8%D0%B7%D0%B0%D1%86%D0%B8%D1%8F#%D0%9A%D1%80%D0%B8%D1%82%D0%B5%D1%80%D0%B8%D0%B9_%D0%9F%D0%B0%D1%80%D0%B5%D1%82%D0%BE)
* [FGSM](https://pytorch.org/tutorials/beginner/fgsm_tutorial.html#fgsm-attack)


### 3. [Исполнитель: TODO]
Визуализировать апостериорное распределение параметров в логистической регрессии и двуслонйной нейронной сети. Сравнить дисперсии у полученных распределений. 

### 4. [Исполнитель: TODO] 
Просэмплировать варианты нейросетей по сетке, сделать 3d-график, каждая точка которого соответствует модели, а координаты:
* Количество параметров нейросети
* Точность модели
* Время обработки одного батча.
	
Построить графики с использованием CPU и GPU. 	
На графике также отметить парето-оптимальный фронт. Допускается использование логарифмической шкалы для наглядности.

Сетка нейросетей: сверточные нейросети. Количество точек на графике должно быть не менее 20.

Выборка: Fasion-MNIST или CIFAR-10.


### 5. [Исполнитель: TODO]
Визуализировать Lottery ticket:  построить график наилучшего качество от количества сэмплов подсети на выборке MNIST:
* ось x: количество сэмплирований подсети 
* ось y: наилучшее качество подсети из всех проведенных сэмплов
	
Сэмплирование проводить случайным образом.
Под подсетью понимается набор незануленных параметров в нейросети. Процент параметров определить самостоятельно исходя из наглядности.
* [Lottery ticket](https://arxiv.org/abs/1905.01067)
	
### 6. [Исполнитель: TODO]
Визуализировать Lottery ticket с добавлением MCMC:  построить график наилучшего качество от количества сэмплов подсети на выборке MNIST:
* ось x: количество сэмплирований подсети 
* ось y: наилучшее качество подсети из всех проведенных сэмплов

Под подсетью понимается набор незануленных параметров в нейросети. Сэмплирование производить с применением пакетов MCMC.
* [Lottery ticket](https://arxiv.org/abs/1905.01067)

### 7. [Исполнитель: TODO] 
Повторить эксперимент WANN: провести эволюционную процедуру построения нейросети для выборки MNIST. При построении эволюционного алгоритма ограничиться одним скрытым слоем константными значениями параметров "1", "-1".
* [WANN](https://arxiv.org/abs/1906.04358)
