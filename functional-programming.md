```javascript	
const x = {
  val: 2
};

const x1 = x => Object.assgin({}, x, {val: x.val + 1})

// 위와 같은 방법을 사용하면 원래의 x를 변형시키지 않을 수 있는데 
// 참고로 Object.assign 첫 번째 argument는 최종 return 값과 같은 메모리를 참조한다. (e.g. 
// 	let a = {b:1} a === Object.assign(a, {}) // true
// )
```



const가 immutable을 의미하는 것은 아니다. 그 이유는 const는 reassign 할 수 없는 변수를 지정하는 것이지 object의 property를 변경할 수 없는 것은 아니기 때문.

Object.freeze는 one depth만 immutable하게 만들 수 있다. object 안에 object는 mutable함.



