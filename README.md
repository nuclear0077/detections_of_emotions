# detections of emotions
Модель на основе keras-vggface
За основу взята модель https://github.com/rcmalli/keras-vggface с весами RESNET50.
Данная работа это сорвевнование на Kaggle https://www.kaggle.com/c/skillbox-computer-vision-project 
Данные для обучения - https://drive.google.com/file/d/1QdhIxh1QUEuLgRb7DWa7RA7CA08ybNRJ/view?usp=sharing
Метки классов для обучения https://drive.google.com/file/d/1iTqJrf5U0icPOJ1L7Ou8b5LdntFBKkju/view?usp=sharing
Данные для теста  - https://drive.google.com/file/d/1bGHeWeWYXj5biL9s-qTc9gyv91WNAbWE/view?usp=sharing
Файл neural network training.ipynb содержит подготовку данных и обучение модели.
Файл work_with_the_camera.ipynb содержит модель которая интегрирована с работой веб камеры в режиме realtime.
Максимальный private score = 0.52720, publick score = 0.54120 на платформе kaggle.
Все обучение происходило на платформе google colaboratory. 
Для запуска обучения необходимо установить следующие библиотеки, примеры с установкой ниже.
!pip install 'h5py==2.10.0' --force-reinstall
!pip install git+https://github.com/rcmalli/keras-vggface.git
!pip install keras_vggface
!pip install keras_applications
!pip install  image
!pip install gdown
!pip install livelossplot
!pip install q keras==2.2.4
%tensorflow_version 1.14.0
Для запуска интеграции модели с веб камерой необходимо установить следующие библиотеки.
Запуск должен происходить в локальной среде для этого можно использовать программу anaconda в которую встроен jupyter notebook, скачать ее можно по ссылке https://www.anaconda.com/products/individual
# !pip install git+https://github.com/rcmalli/keras-vggface.git
# !pip install keras_vggface
# !pip install keras_applications
# !pip install  image
# !pip install q keras==2.2.4
# conda install -c conda-forge keras-applications 
# pip install keras-vggface
