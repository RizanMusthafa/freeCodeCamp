---
id: bad87fee1348ce8acef08814
title: Warn Your Users of a Dangerous Action with btn-danger
challengeType: 0
videoUrl: ''
localeTitle: Предупреждать своих пользователей о опасном действии с опасностью btn
---

## Description
<section id="description"> Bootstrap поставляется с несколькими заранее определенными цветами для кнопок. Класс <code>btn-danger</code> - это цвет кнопки, который вы будете использовать, чтобы уведомить пользователей о том, что кнопка выполняет деструктивное действие, например удаление фотографии кота. Создайте кнопку с текстом «Удалить» и дайте ей класс <code>btn-danger</code> . Обратите внимание, что этим кнопкам по-прежнему нужны <code>btn</code> и <code>btn-block</code> . </section>

## Instructions
<section id="instructions">
</section>

## Tests
<section id='tests'>

```yml
tests:
  - text: Создайте новый элемент <code>button</code> с текстом «Удалить».
    testString: 'assert(new RegExp("Delete","gi").test($("button").text()), "Create a new <code>button</code> element with the text "Delete".");'
  - text: Все ваши кнопки Bootstrap должны иметь <code>btn</code> и <code>btn-block</code> .
    testString: 'assert($("button.btn-block.btn").length > 2, "All of your Bootstrap buttons should have the <code>btn</code> and <code>btn-block</code> classes.");'
  - text: Ваша новая кнопка должна иметь класс <code>btn-danger</code> .
    testString: 'assert($("button").hasClass("btn-danger"), "Your new button should have the class <code>btn-danger</code>.");'
  - text: 'Убедитесь, что все элементы <code>button</code> имеют закрывающий тег.'
    testString: 'assert(code.match(/<\/button>/g) && code.match(/<button/g) && code.match(/<\/button>/g).length === code.match(/<button/g).length, "Make sure all your <code>button</code> elements have a closing tag.");'

```

</section>

## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
  .red-text {
    color: red;
  }

  h2 {
    font-family: Lobster, Monospace;
  }

  p {
    font-size: 16px;
    font-family: Monospace;
  }

  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 50%;
  }

  .smaller-image {
    width: 100px;
  }
</style>

<div class="container-fluid">
  <h2 class="red-text text-center">CatPhotoApp</h2>

  <p>Click here for <a href="#">cat photos</a>.</p>

  <a href="#"><img class="smaller-image thick-green-border" src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>

  <img src="https://bit.ly/fcc-running-cats" class="img-responsive" alt="Three kittens running towards the camera.">
  <button class="btn btn-block btn-primary">Like</button>
  <button class="btn btn-block btn-info">Info</button>
  <p>Things cats love:</p>
  <ul>
    <li>cat nip</li>
    <li>laser pointers</li>
    <li>lasagna</li>
  </ul>
  <p>Top 3 things cats hate:</p>
  <ol>
    <li>flea treatment</li>
    <li>thunder</li>
    <li>other cats</li>
  </ol>
  <form action="/submit-cat-photo">
    <label><input type="radio" name="indoor-outdoor"> Indoor</label>
    <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
    <label><input type="checkbox" name="personality"> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Crazy</label>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</div>

```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
