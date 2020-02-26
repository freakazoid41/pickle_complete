

# Pickle Complate

> Pickle complate is a autocomplate component written as completely pure javascript. Just send json object or request information have fun again ! :-D 

> Pickle complate does't need anything except you !

**Badges Falan**

- Simple javascript ability
- Simple css ability for some style editing for your project




## Initiation And Using Example 

> Initiate like this (not serverside) :

```javascript


const pc = new PickleComplate({
      data:[{
        value:'Turkey',
        text:'Türkiye'
      },{
        value:'Russia',
        text:'Rusya'
      },{
        value:'Germany',
        text:'Almanya'
      },{
        value:'Italia',
        text:'İtalya'
      },{
        value:'France',
        text:'Fransa'
      }],
      config: {
        type:'local',
        target: '.picomplete',
        clickCallback:(target,node)=>{
          target.value = node.value;
        }
      }
    });
```
> Initiate this for serverside :
```javascript


const pc = new PickleComplate({
      request:{
        url:'https://yourapiaddress.com',
        type:'POST',
        value:'name',
        text:'name'
      },
      config: {
        type:'server',
        target: '.picomplete',
        clickCallback:(target,node)=>{
          target.value = node.value;
        }
      }
    });
```



---

> You can use 'POST' or 'GET' for serverside.



---

## Installation

- Just include js and css file to your project then you can use it

### Clone

- Clone this repo to your local machine using `https://github.com/freakazoid41/pickle_complete.git`

