1. Abramov Konstantin;  

2. e-mail:konstantin.orneo88@gmail.com; phone: +7 937 640 7857;

3. Learning ability, sociability, patience

4. A little knowledge of Photoshop, the initial level of HTML and Javascript.

5. My little practice on JavaScript:
```javascript
$(function() {
var uds='';
var $listItems=$('li');
var $headItems=$('ul');


  $('ul').on('click',function(){
    uds=this.class;
    $headItems.append('<p>' + 'Список обновлен!' + '</p>');
    $(uds).children('ul').remove();
  });

  $('li').on('click', function(){
$listItems.after('<a>' + ' без ГМО' + '</a>');
  $('li').find('a').remove();
  });

$listItems.on('mouseout',function(){
  $('a').remove();
});

$headItems.on('mouseout', function(){
  $(this).children('p').remove();
});
/*анимация*/
$(function() {
$('ul').hide().slideToggle();
var $Li = $('li');
$Li.hide().each(function(index){
  $(this).delay(200 * index).fadeIn(100);
});
});

$(function(){
  $('li').on('mouseover', function(){
    $(this).animate({
      fontSize:'34',
      fontFamily:'Arial',
        },250);
      });
    });
$(function(){
  $('li').on('mouseout', function(){
$(this).animate({
  fontSize: '25',
}, 500);
  });
});

/*работа с добавлением формы*/
$(function(){
var $newItemBut = $('#newItemButton');
var $newItemForm = $('#newItemForm');
var $textInput = $('input:text');

$newItemBut.show();
$newItemForm.hide();

$('#showForm').on('click', function(){
$newItemBut.hide();
$newItemForm.show();
});

$newItemForm.on('submit', function(e){
e.preventDefault();
var newText = $textInput.val();
$('li:last').after('<li>' + newText + '</li>');
$newItemForm.hide();
$newItemBut.show();
$textInput.val('');
});
  });
});
```

6. No experience. 

7. Technical College, Russian Railways Academy.

8. Intermediate (can translate some texts and spoken language with vocabulary)
