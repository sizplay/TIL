## Object를 Array로 변환 방법

Object methods를 통해 간단히 Array로 변경 가능

```javascript
const bag = {
  small: "handbag",
  medium: "backpack",
  large: "carrier"
};

const keys = Object.keys(bag);
const values = Object.values(bag);
const keyNvalues = Object.entries(bag);

console.log(keys); // ['small', 'medium', 'large']
console.log(values); // ['handbag', 'backpack', 'carrier']
console.log(keyNvalues); // [['small', 'handbag'], ['medium', 'backpack'], ['large', 'carrier']]
```

좀 더 복잡한 구조도 Object.entries를 통해 쉽게 변환 가능하다

```javascript
const myApp = {
  chat: "kakaotalk",
  browser: ["chrome", "firefox", "safari"],
  navigation: {
    food: "kakaomap",
    traffic: "tmap"
  }
};

let arr = Object.entries(myApp);
console.log(arr);
// [["chat", "kakaotalk"], ["browser", ["chrome", "firefox", "safari"]], ["navigation",{ food: "kakaomap", traffic: "tmap"}]]
```

반대로 [['chat', 'kakaotalk']] 포멧의 array를 object로 변환 하는 방법은 Object.fromEntries를 사용 하면 된다.

```javascript
const myAppArr = [
  ["chat", "kakaotalk"],
  ["browser", ["chrome", "firefox", "safari"]],
  ["navigation", { food: "kakaomap", traffic: "tmap" }]
];

let obj = Object.fromEntries(myAppArr);
console.log(obj);

/*
{
  browser: ["chrome", "firefox", "safari"],
  chat: "kakaotalk",
  navigation: {
    food: "kakaomap",
    traffic: "tmap"
  }
}
*/
```
