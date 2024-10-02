# PAK_project
<h1>Flowers classification project</h1>
<h2>1. Введение</h2>
<p>Цель раюоты - создать модель для классификации цветов. Датасет был взят с kagle, модель обучалась на этом же сайте.<br>
Согласно условиям соревнования требовалось создать файл с предсказаниями моделей в формате .csv и отправить его.<br></p>
<h2>2. Выполнение задания</2>
<p>Для выполнения задания была выбранна модель ResNet50.</p>
<img src="./model.png">
<p>Общая архитектура модели Resnet</p>
<img src="./arhitec.png">
<p>В своей программе, для обучение модели, я использовал оптимайзер Адам, функцию потерь CrossEntropy, а так же sheduler, для того, чтобы коррективовать learning rate. Информацию по последнему я взял по <a href="https://neptune.ai/blog/how-to-choose-a-learning-rate-scheduler">этой ссылке</a>.</p>
<h2>3. Процесс обучения</h2>
<h4>Accuracy в процессе обучения</h4>
<img src="training.png">
<p>Модель обучалась в течение 40ка эпох, это можно увидеть из скриншота выше. Исходя из тестового accuracy можно сделать вывод, что модель не переобучилась, а так же, что в последние 8 эпох резкультат почти не менялся. Именно поэтому конечное число эпох в модели 40. Ниже представленн график для accuracy и loss</p>
<img src="acc_graoh.png">
<h2>Результат</h2>
<p>Результат, который учитывался в соревновании, это метрика f1</p>
<img src ="f1.png">
<p>Результаты модели:</p>
<p><b>Accuracy</b> = 91</p>
<p><b>F1</b> = 62</p>
<p>По итогу я занял 43 место в таблице этого соревнования</p>
<img src="result_by_kag.png">
<img src="table_place.png">
