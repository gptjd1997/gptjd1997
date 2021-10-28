# AWS

### S3
>Static Files

# React


```
npm i styled-components react-hook-form react-router-dom @apollo/client graphql react-helmet-async
npm i --save @fortawesome/fontawesome-svg-core
npm install --save @fortawesome/free-solid-svg-icons
npm install --save @fortawesome/react-fontawesome
npm install --save @fortawesome/free-brands-svg-icons
npm install --save @fortawesome/free-regular-svg-icons
```


# 자바 스크립트

### Optional Chaining

```
const person = {
  name: 'Alice',
  job: {
    companyName: 'abc',
    title: 'developer'
  }
};

console.log(person.job.companyName); // 'abc'
console.log(person.pet?.name); // undefined
```
 

> 이 때 Optional Chaining을 사용하면 에러가 발생하는 대신 undefined가 리턴된다. 
> (만약 Person.pet.name이 존재 할 경우 그 값이 리턴된다)
