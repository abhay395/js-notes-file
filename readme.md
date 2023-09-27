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
