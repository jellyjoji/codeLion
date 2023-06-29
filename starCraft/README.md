# jQuery 를 활용한 starCraft 게임 만들기

## .animate(properties)
.animate(필수요소 [선택요소] [선택요소] ) 로 구성되어 필수요소인 properties 를 반드시 써줘야 합니다.
```js
.animate( properties [, duration ] [, easing ] [, complete ] )
```

## callback 함수
함수 안에서 실행하는 또 다른 함수이며, 지금 바로 실행되지 않지만 다른 함수의 입력 값으로 전달되어 다른 함수에 의해서 나중에 호출되게 되는 것입니다. 
```js
      $('#spit').fadeOut(function () {
        hp = hp - 1;
        $('#hp').text('HP: ' + hp);
        // hp:3 이 hp:0 이 되면 bunker 가 사라지게하겠다 : call back
        if (hp == 0) {
          $('#bunker').fadeOut();
        }
      });
```

## .text()
선택한 요소 안의 내용을 가져오거나, 다른 내용으로 바꾸는 메서드입니다.
```js
$('#hp').text('HP: ' + hp);
```

## .css() 
선택한 요소의 css 속성값을 가져오거나, 속성을 추가하는 메서드입니다.
```js
$('#spit').css({ left: 150 });
```



https://github.com/jellyjoji/codeLion/assets/74365275/3bf1af96-c469-4a59-a10d-09ddce394597

