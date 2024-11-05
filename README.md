# Описание:
Эта программа, помогающая запоминать лица людей. Она подойдет для тех, кто работает с большим количеством людей, которых нужно запомнить, например для преподавателей. Она работает по следующему принципу: в режиме редактирования Вы загружаете в программу фотографию человека, ФИО и при необходимости прочие данные. А затем в формате теста, Вам предлагается фотография и 4 варианта ФИО, Вам нужно выбрать верный вариант. Когда процент правильных ответов будет больше 95%, можно считать, что задача выполнена.

# ТЗ:
Нужно написать программу с графическим интерфейсом на PyQT для запоминания лиц. Все данные должны храниться в базе данных SQL. Данные о результатах предыдущего теста должны храниться в текстовом файле.
Программа должна быть в exe, при запуске исполняющего файла, откроется окно с выбором режима "Редактирование" или "Тест".
- Режим "Редактирование":
  Будет поле ввода данных (ФИО и при необходимости прочее) и окно с изображением, под которым будет кнопка "Открыть изображение" при нажатии которой будет открываться окно выбора файла.
  После добавления, изображение должно будет открыться в окне изображения. Снизу будет 3 кнопки: "Добавить элемент", "Найти элемент", "Удалить элемент".
  - При нажатии на кнопку "Добавить элемент", в базу данных добавиться элемент с учетом даных указанных в поле ввода данных и окне изображения.
    Если одна из ячеек пустая, должно появиться сообщение об ошибке с просьбой заполнить ячейки.
  - При нажатии на кнопку "Найти элемент", в окне изображения будет открываться картинка связанная с теми данными, которые указаны в поле ввода данных.
    Если такого изображения нет, будет выводиться сообщение об отсутствии такого элемента с предложением добавить.
  - При нажатии на кнопку "Удалить элемент" и наличии данных в поле ввода данных, будет появляться диалоговое окно с просьбой подтвердить удаление конкретного значения и в случае подтверждения, соответственно удаление
    Если значение не найдено, то вывеси сообщение об ошибке и просьбе проверить корректность введенных данных.
  Снизу должна быть кнопка "Вернуться в главное меню", возвращающая пользователя в главное меню.
- Режим "Тест":
  Должно быть сообщение о результате предыдущего теста (если первый запуск программы, то сообщения быть не должно) и кнопка начать. При начале будут поочередно предлагаться вопросы, до нажатия кнопки "Завершить".
  Вопрос выглядит следующим образом: слева окно изображения, справа 4 вертикально расположенных кнопки с вариантами ответа, только один из которых правильный. Картинки и варианты ответа расположены в рандомном порядке
  При выборе ответа выводится сообщение: корректен или нет выбранный ответ. Если нет, то пишется правильный ответ.
  При нажатии кнопки "Завершить" тест завершается и выводится процент правильных ответов.
  Снизу должна быть кнопка "Вернуться в главное меню", возвращающая пользователя в главное меню.
