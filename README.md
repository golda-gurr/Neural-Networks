# GB Курс Введение в нейронные сети

### Урок 1. Основы обучения нейронных сетей

1.	Попробуйте видоизменить параметры разобранной на уроке двухслойной нейронной сети таким образом, чтобы улучшить ее точность (число нейронов, число эпох , можно изменять число слоев).
2.	Проведите анализ — что приводит к ухудшению точности нейронной сети? Что приводит к увеличению ее точности?


### Урок 2. Keras

Используем набор примеров fashion-MNIST

1. Опишите - какой результат получен в нейросети в зависимости от: 
* числа нейронов в слое (для 2-хслойной сети), 
* числа слоев (2, 3, 5, 10) при близких размерах сети (близкое число тренируемых парметров). 
* фиксируйте для тренировочного и тестового набора метрики accuracy. 
2. Проверьте работу разных оптимизаторов (SGD, Adam, RMSProp) для одной из моделей п.1.Фиксируйте для тренировочного и тестового набора метрики accuracy. 
3. Сделайте вывод - что помогло вам улучшить качество классификации в нейросети на тестовом наборе? 
4. Для одного варианта сетей сформируйте матрицу ошибок по классам. Оцените качество модели по каждому классу отдельно (полнота , точность) 

* Поработайте с документацией Keras. Найдите полезные команды не разобранные на уроке


### Урок 3. TensorFlow

1.	Постройте нейронную сеть (берем простую линейную сеть, которую разбирали на уроке: меняем число слоев, число нейронов , типы активации, тип оптимизатора) на датасет from sklearn.datasets import load_boston.
2.	Измените функцию потерь и метрику для этой задачи. Постройте 10-15 вариантов и сведите результаты их работы в таблицу Опишите, какого результата вы добились от нейросети? Что помогло вам улучшить ее точность?
3.	Поработайте с документацией TensorFlow 2. Найти 2-3 полезные команды TensorFlow, не разобранные на уроке (полезные для Вас).


### Урок 4. Сверточные нейронные сети

*	обучить сверточную нейронную сеть в стиле AlexNet (с падением размера ядра свертки и последовательностью блоков свертка-пулинг (conv-pool)-(conv-pool)-...) на датасете fashion-mnist
*	оценить рост точности при увеличении ширины сети (больше ядер)
*	оценить рост точности при увеличении глубины сети (больше слоев)
*	сравнить с точностью полносвязной сети для этой выборки


### Урок 5. Рекуррентные нейронные сети

1.	Попробуйте обучить нейронную сеть LSTM на любом другом датасете (любимый временной ряд, текст на русском (другом языке) как генератор или классификатор, или прилагаемый набор airline-passengers - пасажиропоток для авиалиний). Опишите, какой результата вы получили? Что помогло вам улучшить ее точность?
2.	*Попробуйте на numpy реализовать нейронную сеть архитектуры LSTM
3.	*Предложите свои варианты решения проблемы исчезающего градиента в RNN


### Урок 6. Сегментация и автоэнкодер
1.	Попробуйте обучить нейронную сеть U-Net на любом другом датасете. Опишите в комментарии к уроку - какой результата вы добились от нейросети? Что помогло вам улучшить ее точность?


### Урок 7. Детектирование объектов
1.	Сделайте краткий обзор какой-нибудь научной работы посвященной тому или иному алгоритму для object detection, который не рассматривался на уроке. Проведите анализ: Чем отличается выбранная вами на рассмотрение архитектура нейронной сети от других архитектур? В чем плюсы и минусы данной архитектуры? Какие могут возникнуть трудности при применении данной архитектуры на практике?
2.	Запустите детектор (ssdMobile_v2 или faster_rcnn, или любой другой детектор) для своей картинки и попробуйте найти 10 объектов, 100 объектов.


### Урок 8. GAN

1. Попробуйте улучшить работу нейронной сети рассмотренной в методическом пособии. 
Приложите анализ. Приложите лучшее сгенерированное изображение к уроку.  
* Обратите внимание для запуска нейронной сети понадобиться tensorflow 2.1.0 и минимум 8gb опер. памяти(если запускать на процессоре).


### Практическое задание к курсу:
1.	Обучите нейронную сеть любой архитектуры которой не было на курсе, либо обучите нейронную сеть разобранной архитектуры, но на том датасете, которого не было на уроках. Сделайте анализ, того, что вам помогло в улучшения работы нейронной сети.
* вариант для 1) Обучите VAE на fashion_mnist

2.	Сделайте краткий обзор какой-нибудь научной работы, посвященной тому или иному алгоритму нейронных сетей, который не рассматривался на курсе. Проведите анализ: Чем отличается выбранная вами на рассмотрение архитектура нейронной сети от других архитектур? В чем плюсы и минусы данной архитектуры? Какие могут возникнуть трудности при применении данной архитектуры на практике?

