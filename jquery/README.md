  # jQuery 기초

## 1st. jQuery 문법 사용법
```js
$('클래스').val()
```

## 2nd. jQuery 함수 생성
```js
// 함수생성
function 함수이름() {
  함수 내용
};
// 생성한 함수 사용
$('클래스').val(함수이름)
```
예시
```js
    // function 함수() 생성
    function hello() {
      console.log('hello');
    }
    // jQuery .click 이벤트 : 클릭하면 작동하겠다
    $('#click').click(hello);
```

## 3rd. jQuery 익명 함수
익명 함수 : 함수를 한번만 사용할때 
```js
$('클래스').val(function(){
  함수 내용
})
```
길게 써야했던 jQuery 함수 를 한번만 사용할때 이름없이 익명 함수로 생성
```js
function hello() {
console.log('hello');
}
$('#click').click(hello);

//해당 코드가 아래와 같이 익명함수(함수이름을 지정하지 않음)로 변화

$('#click').click(function(){
console.log('hello');
});
```