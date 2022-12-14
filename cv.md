# rsschool-cv
## Gregory Ponomaryov

# contacts
+ Location: Petropavlovsk, Kazakhstan
+ Phone: +7 707 037 2609
+ Email: pvg9kz@gmail.com
+ GitHub: GPonomarev
---
## About me
I'm trying to learn new technologies. I have experience of working in a team. I want to become a full stack developer.
## Skills
+ JavaScript, [TypeScript](https://www.typescriptlang.org/docs/)
+ [React](https://reactjs.org/docs/getting-started.html), [NextJS](https://nextjs.org/docs)
+ [PostgreSQL](https://www.postgresql.org/docs/current/index.html)
+ HTML, CSS
+ GIT
+ Some basic things from [Node.js](https://nodejs.org/en/docs/)
## Code example
You are given an array (which will have a length of at least 3, but could be very large) containing integers. The array is either entirely comprised of odd integers or entirely comprised of even integers except for a single integer N. Write a method that takes the array as an argument and returns this "outlier" N.

```
//isOdd return 1 if argument number is odd, otherwise 0
function isOdd(number){
  return Math.abs(number%2);
}

function findOutlier(integers){
  /*Here we try to figure out wich value we should find, depending on array type*/
  let arrayIsOdd = false;
  let oddSum = 0;
  oddSum = isOdd(integers[0]) + isOdd(integers[1]) + isOdd(integers[2]);
  oddSum > 1 ? arrayIsOdd = true : arrayIsOdd = false;
  
  for (let i=0; i<integers.length; i++){
    if (arrayIsOdd) {
      if (!isOdd(integers[i])){
        return integers[i];
      };
    } else {
      if (isOdd(integers[i])){
        return integers[i];
      };
    }
  }
}
```
## Experience
For a year and a half, I participated in two startups, unfortunately the funding ran out.
## Education
+ [Manash Kozybayev North Kazakhstan University](http://nku.edu.kz/), Bachelor of Computer Science
+ [Omsk State Pedagogical University](https://omgpu.ru/en/),
M.Ed.
---
## English
EF SET considers that b1