
![plot](/img/Sections.PNG)


Этот репозиторий представляет собой сборник заготовок, лайфхаков и практик, которые я использую в своей работе при анализе данных.


## Структура 

### 1. Jupyter - в этом разделе собраны приемы работы в Jupyter notebooks.
- [**Start.ipynb**](https://github.com/Saxsafon/Analysis/blob/master/0_Jupyter/Start.ipynb) - в этом ноутбуке содержится илюстрированная инструкция по установке и настройке рабочего окружения.
  - Как добавить python в список системных переменных?
  - Как создать рабочую среду Python?
  - Как установить Jupyter и другие пакеты?
  - Как запустить Jupyter, в том числе через ярлык на рабочем столе?

- [**Jupyter_IPython.ipynb**](https://github.com/Saxsafon/Analysis/blob/master/0_Jupyter/Jupyter_IPython.ipynb) - здесь рассматриваются возможности оболочки IPython
  - Магические команды (как импортировать ноутбук?)
  - Доступ к документации
  - Автозаполнение

- [**external_code_example.ipynb**](https://github.com/Saxsafon/Analysis/blob/master/0_Jupyter/external_code_example.ipynb) - код в этом ноудбуке используется в файле Jupyter_IPython.ipynb

- [**Jupyter_settings**](https://github.com/Saxsafon/Analysis/blob/master/0_Jupyter/Jupyter_settings.ipynb) - ноутбук содержит конструкции, позволяющие настроить ноутбук для более удобной работы. 
  - Как изменить количество символов, выводимых в ячейках датафреймов?
  - Как изменить ширину ячеек ноутбука?
  - Как скрыть предупреждения?

- **shortcuts.ipynb** - здесь собран список удобных горячих клавиш

- [**Jupyter_lifehacks.ipynb**](https://github.com/Saxsafon/Analysis/blob/master/0_Jupyter/Jupyter_lifehacks.ipynb) - здесь содержатся дополнительные лайфхаки и практики, полезные при работе в ноутбуках
  - Как вывести датафреймы рядом друг с другом?
  - Как сохранить ноутбук изнутри ячейки?

### 2. Terminal
- [**os.ipynb**](https://github.com/Saxsafon/Analysis/blob/master/0_Terminal/os.ipynb) - в этом ноутбуке собраны функции и методы пакета os, используемые для взаимодействия с командной строкой

- [**Commands.txt**](https://github.com/Saxsafon/Analysis/blob/master/0_Terminal/Commands.txt) - в файле собран список полезных команд терминала Linux
  - команды для работы с файлами и папками
  - команды менеджера пакетов pip
  - ...

### 3. Storing
- [**Archives.ipynb**](https://github.com/Saxsafon/Analysis/blob/master/I_Storing/Files.ipynb) - здесь собраны python-пакеты для работы с .7z и .zip архивами (py7zr, zipfile, shutil)
  - Как распаковать архивы различных форматов?
  - Как упоковать один или несколько файлов в архив?

- [**Files.ipynb**](https://github.com/Saxsafon/Analysis/blob/master/I_Storing/Files.ipynb) - файл содержит несколько функций, с помощью которых можно считать содержимое нескольких файлов

- [**Formats.ipynb**](https://github.com/Saxsafon/Analysis/blob/master/I_Storing/Formats.ipynb) - здесь перечислены различные форматы для хранения данных, продемонстрированы их преимущества и недостатки
  - .xlsx - удобный для просмотра глазами, но объемный и долго считывается
  - .csv - распространенный формат, который можно очень хорошо сжать архиватором. Но в обычном состоянии объемный и тоже долго считывается.
  - .feather - не открывается. Зато занимает мало места и очень быстро считывается.

- [**Pickle.ipynb**](https://github.com/Saxsafon/Analysis/blob/master/I_Storing/Pickle.ipynb) - содержит примеры сохранения объектов python в .pkl-файлах с помощью пакета Pickle

### 4. Processing
- **Groupby.ipynb** - в ноутбуке собраны полезные практики использования метода .groupby() 
  - .groupby() + .apply()
  - .groupby() + .agg()
  - .groupby() + .filter()
  - .groupby() + .transform()
  - Как посчитать и вывести сумму элементов на каждом уровне группировки?

- **Pivot_tables.ipynb** - здесь собраны практики использования метода .pivot_table() (ОЧЕНЬ полезная штука)

- [**Manipulation.ipynb**](https://github.com/Saxsafon/Analysis/blob/master/II_Processing/Manipulation.ipynb) - методы и практики для работы с данными 
  - value_counts() - количественное и процентное соотношение + бины, в том числе и кастомные
  - Маски, их сохранение и комбинирование
  - Векторизованные операции над строками
  - ReGex и методы, использующие регулярные выражения

- [**Datetime.ipynb**](https://github.com/Saxsafon/Analysis/blob/master/II_Processing/Datetime.ipynb) - ноутбук содержит практики работы с пакетом datetime
  - Объекты date, time и datetime
  - Перевод datetime-объектов в строки и наоборот
  - Объекты timestamp и timedelta
  - Как быстро посчитать количество секунд между записями в таблице?
  - Как посчитать количество записей за временной период? _(здесь используются pivot_table)_

- **Generation.ipynb** - при разработке обрабатывающих pipeline-ов, бывает полезно сгенерить тестовые данные. В этом ноудбуке собраны практики и примеры генерации данных различного вижа
  - Пакет random, а также numpy-рандомайзер
  - Как сгенерить данные с внутренними зависимостями _(пока в разработке)_

- **Lifehacks.ipynb** - здесь хранятся дополнительные небольшие лайфхаки. А также практики требующие разбора.
  - Как добавить несколько колонок с помощью одной функции?
  - Как заменить или сбросить header датафрейма?
  - Как вывести датафрейм в виде строки, чтобы его было удобно читать?
### 5. Visualization
- **Matplotlib.ipynb** - приемы построения графиков средствами пакета matplotlib
  - Встроенные методы Pandas - самый быстрый способ визуализировать данные 

- **Plotly.ipynb** - приемы построения различных графиков средствами пакета plotly
  - Столбчатый (в том числе горизонтальный), линейный, круговой графики
  - Управление подписями к графикам
  - Скользящее среднее
  - Визуализация деревьев _(пока в разработке)_

- **Table.ipynb** - здесь подробно разобраны возможности стилизации датафреммов с помощью атрибута .style. А также работа с объектами Styler
  - Как выделить границы датафрейма?
  - Как добавить несеколько heatmap-градиентов в одну таблицу?

### 6. AutoExcel - пакет OpenPyxl используется для настройки файлов excel с помощью Python. С его помощью можно представлять результаты анализа в виде красивых автоматических excel-отчетов.
 - **Openpyxl_offloading.ipynb** - в этом ноутбуке собраны практики выгрузки датафреймов файл excel. А также дополнительной настройки этих файлов.
  - Как автоматически масштабировать ширину колонок, в соответствии с их содержанием?
  - Как выгрузить данные с многоуровневой шапкой таблицы?
  - Как добавить фильтры в excel-файлы?
  - Как сгруппировать строки или колонки в excel-файлах? 

### 7. Presentation
- **Presentation Builder.pptx** - в этом файле собрана коллекция фигур и изображений, с помощью которыз можно легко и быстро собрать схему или макет идеи.

