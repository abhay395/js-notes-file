# shorts notes and concept
## setIntervel()
the use of setintervel 
it's want a refrence of function and interval time whene it run 
```
 setInterval(butnfun,500)

```
how clear setinterval
seen this
 ```
 intervelid= setInterval(butnfun,500)
  clearInterval(intervelid)
 
 ```
 when we want to clear the interwla we use clearinterval methode its wants idname of setinterval 
## async keye word or async methode
when we want to do asyncrinate work in js we use async key word in function and then we use await key word to do work like this
```
 async createAccount({email,password,name}){
        try {
          const userAccount=await this.account.create(ID.unique(),email,password,name)
          if(userAccount){
            //call another method
          }else{
            return userAccount;
          }
        } catch (error) {
            throw error;
        }
    }
```
## getBoundingClientRect() 
is methode ka use kisi bhi partculer tage ya button ki position hight widht ka pata laga ne me kiya jata hai
```
const element = document.getElementById('myElement');

// getBoundingClientRect() ka use karke element ke rectangular region ki information retrieve kare
const rect = element.getBoundingClientRect();

// Retrieve ki gayi information ka istemal karen
console.log('Top:', rect.top);
console.log('Left:', rect.left);
console.log('Bottom:', rect.bottom);
console.log('Right:', rect.right);
console.log('Width:', rect.width);
console.log('Height:', rect.height);
```
isme jo parameters melete hai vo px me hote hai
## addEventListner('load',function(){}) ,addEventListner('DOMContentLoaded',function(){})
load ka use jab hame kise button ya class ka page ke pure load hone ke baad add karna hota hai iska use kare ke hame page loder bana sakte hai

or DOMContentLoaded ka use jab kiya tab kya jata hai jab hame kise button ka Html dom render hote hi add karn hota hai 

# when you want remaing time to your fyture time you use this code
```
 const t = futureTime-today;// t is remaing time in ms 
  // 1s = 1000ms 
  // im=60s
  // 1hr = 60min
  //1d=24hr
  const oneDay=24*60*60*1000;
  const oneHours=60*60*1000;
  const oneMinite=60*1000;
  // caslculate all values
  let Remday=Math.floor(t/oneDay);
  let Remhours = Math.floor((t % oneDay)/oneHours);
  let Remmin = Math.floor((t % oneHours)/oneMinite)
  let Remsec = Math.floor((t % oneMinite)/1000)

```
# how to make and set attribue in html using js
```
 const element = document.createElement('article');
        // add class
        element.classList.add('grocery-item');
        // add id
        const attr = document.createAttribute('data-id');
        attr.value = id ;
        element.setAttributeNode(attr);
```
# note
when we make a emlemnet using a createElement methode we can't accese those element outside this function but we can acces those element using outside of elements

#note 2 how to acces previous Element sibling 
 use.previousElementSibling to acces previous Element sibling like this 
```
editElement = e.currentTarget.parentElement.previousElementSibling

```
