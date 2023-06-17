# rsschool-cv

## Имя и фамилия
Илья Переселяк
## Контактная информация
* +375 (44) 7929591
* ilyapereselyakby@gmail.com 
## Обо мне
_Работал с с++, java, Microsoft SQL Manager. Наверное знаю c# на уровне june. Редактировал изображения в Adobe Photoshop, ilustrator, так-же занимался анимацией в Adobe animate. Умею в frontend(HTML, CSS, JS). Есть некоторые знания в  PHP. Ознакомлен с CMS WordPress Имею небольшой опыт в unity, еще не освоил развертки и шейдеры. Я неконфликтный, усердный, пунктуальный и коммуникабельный._
## Навыки
* Знание языков	Русский — Родной
    * Английский — A2 — Элементарный
* Навыки
    * JavaScript, HTML, MySQL, CSS3, PHP  
    * Adobe,Photoshop, Adobe Illustrator, Figma  
    * Unity, 3D Max, Blender 3D 
    * C#, Windows Forms
## Примеры кода
```PHP, проект-электронная книга рецептов, функция для добавления рецептов в базу данных
<?php
//Вставка рецептов
if (isset($_POST["image"]) && isset($_POST["Nazva"]) && isset($_POST["Author"]) && isset($_POST["Ingrid"]) && isset($_POST["Wayofcook"])) {
  $mysqli = new mysqli("localhost", "root", "root", "project");

  // Check connection
  if ($mysqli->connect_errno) {
    echo "Подключение: 0, в следстии следующей ошибки: " . $mysqli->connect_error;
    exit();
  } else
    printf("Подключение: 1, ваш рецепт добавлен.\n");

  $image = $mysqli->real_escape_string($_POST["image"]);
  $nazva = $mysqli->real_escape_string($_POST["Nazva"]);
  $author = $mysqli->real_escape_string($_POST["Author"]);
  $ingrid = $mysqli->real_escape_string($_POST["Ingrid"]);
  $way = $mysqli->real_escape_string($_POST["Wayofcook"]);
  $sql = "INSERT INTO recepies (photo,author,nazva,ingridients,wayofcooking) VALUES ('$image','$author','$nazva','$ingrid','$way')";
  if(empty($image)||empty($nazva)||empty($ingrid)||empty($way)||empty($image)&&empty($nazva)&&empty($ingrid)&&empty($way)){
    echo "Введите данные"; 
  }
  else{
  $mysqli->query($sql);
  }
  $mysqli->close();
}
?>
```
## Курсы
__JS/FE Pre-School 2023Q2(in progress)__
## Английский язык
__A1, Epam test__
![Это опциональный alt-текст](/assets/images/EpamEngTest.png.png)
