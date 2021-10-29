# AWS

> ### S3
>Static Files

---


# React


> ```
> npm i styled-components react-hook-form react-router-dom @apollo/client graphql react-helmet-async
> npm i --save @fortawesome/fontawesome-svg-core
> npm install --save @fortawesome/free-solid-svg-icons
> npm install --save @fortawesome/react-fontawesome
> npm install --save @fortawesome/free-brands-svg-icons
> npm install --save @fortawesome/free-regular-svg-icons
> ```

> ## React-hook-form
> #### react-hook-form 사용 방법

> ```
> const {
>     register,
>     handleSubmit,
>     watch,
>     formState: { errors },
>   } = useForm();
> const onSubmitValid = (data: any) => {
>   console.log(data);
> };
>
> const onSubmitInvalid = (data: any) => {
>   console.log(data);
> };
> 
> 
> <form onSubmit={handleSubmit(onSubmitValid, onSubmitInvalid)}>
>   <input
>             {...register("user", { required: true (or required: "이름 또는 이메일을 입력하세요" >> 유효성 검사가 실패 할 시 오브젝트에 전송 될 에러 메세지) })}
>             type="text"
>             placeholder="Placeholder"
>           />
></form>
>
> //(onSubmitValid = 유효성 검증이 완료 될 시 , onSubmitInvalid = 유효성 검증이 실패 할 시 )
> // user = 네임
> // required = 필수항목 지정 ox (최소 글자수, 정규식 지정 등 여러 유효성 검사를 할 수 있음 https://react-hook-form.com/kr/get-started/#Applyvalidation 참고)




#### console.log(watch());
>지정된 form 안의 input값이 onChange될 때마다 값을 가져옴
#### console.log(watch("user")
>user 네임을 지정해준 input값을 onChange시 마다 값을 가져옴

#### console.log(watch()) 결과
{user: 'q', password: ''}

{user: 'qw', password: ''}

{user: 'qwe', password: ''}

{user: 'qwe', password: 'a'}

{user: 'qwe', password: 'as'}

{user: 'qwe', password: 'asd'}

{user: 'qwe', password: 'asde'}



---

# 자바 스크립트

> ### Optional Chaining

> ```
> const person = {
>   name: 'Alice',
>  job: {
>     companyName: 'abc',
>     title: 'developer'
>   }
> };
> 
> console.log(person.job.companyName); // 'abc'
> console.log(person.pet?.name); // undefined
>  
> ```
>>  이 때 Optional Chaining을 사용하면 에러가 발생하는 대신 undefined가 리턴된다. 
>>   (만약 Person.pet.name이 존재 할 경우 그 값이 리턴된다)
>>
