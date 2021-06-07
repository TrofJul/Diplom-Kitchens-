# Diplom-Kitchens
Дипломный проект "Автоматизированная система определения параметров кухонной мебели по фотографии"

Для запуска проекта необходимо установить зависимости
> pip install -r requirements.txt <
и выполнить
> streamlit run streamlit_app.py <

Реализован с ипользованием технологий машинного обучения и нейронных сетей, используемые фреймфорки: PyTorch, TensorFlow.
Решаются задачи:
детекции на изображении объектов, свойственных кухням, и их подсчет,
классификации помещения по типу кухня/не кухня,
определения основной цветовой палитры изображения,
классификации кухни по конфигурации (прямая, угловая, островная).

Для задачи классификации по конфигурации использовался прием transfer learning с предобученной сетью VGG16, для детекции используется предобученная
на датасете COCO сеть faster_rcnn_inception_resnet/
