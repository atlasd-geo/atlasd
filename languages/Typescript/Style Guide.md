# Typescript Style Guide
Read the below before contributing Typescript source.

## Syntax
- Use `const` and `()=>{}` instead of function. This helps order your logic. If you run into issues with this syntax, re-examine your design pattern before abandoning.
```typescript
/**
* @description Discouraged method with function.
* ...
*/
function logName (name : string)=>{
  console.log(name);
}

/**
* @description Encouraged method with const.
* ...
*/
const logName = (name : string)=>{
  console.log(name);
}
```

## Patterns
- Use OOP and Functional patterns freely. (Different recommendations may apply for certain frameworks and technologies.)
- Keep method length short. 20 lines is generally a good rule, unless you absolutely need to wrap a method in context.
```typescript
/**
* @description Discouraged longer method.
* ...
*/
const hideYoSpouseAndKids = (you : Person, spouse : Spouse, kids : Kid[])=>{

  you.yellTo(spouse);
  you.find(spouse);
  you.hug(spouse);
  you.hide(spouse, "in closet");

  kids.forEach((kid)=>{

    you.yellTo(kid);
    you.find(kid);
    you.getAttention(kid);
    you.getAttentionAgain(kid);
    you.encourgaeWithCandy(kid);
    you.hide(kid, "under bed");

  })

}

/**
* @description Encouraged shorted method.
* ...
*/
const hideYoSpouseAndKids = (you : Person, spouse : Spouse, kids : Kid[])=>{

  you.hideSpouse(spouse); // hideSpouse implemented elsewhere

  kids.forEach((kid)=>{

    you.hideKid(kid); // hideKid implemented elsewhere

  })

}
```
- Write code that describes itself.

## Comments
- Use [Typedoc](https://typedoc.org/) conventions with the addition of the following:
  - @dev: for remarks on refactoring and other development pattern suggestions
- Always use @description when describing what a variable or function is or does.
- Try to write code that doesn't require too many comments to understand.

## Variables
- Use variables freely. (Different recommendations may apply for certain frameworks and technologies.)

## Types and Interfaces 
- Use types unless you need an interface.
