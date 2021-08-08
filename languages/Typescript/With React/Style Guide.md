# TypeScript with React StyleGuide
Follow this style guide when using TypeScript to write React. Also consult the TypeScript Style Guide.

## Patterns 
- Leverage the [Context API](https://reactjs.org/docs/context.html) instead of higher order functions to solve most cases wherein state needs to be shared between components.
- Use the Component FTTemplate to generate folder structures for components.
- Avoid using classes. In cases where you need a class, consider whether you actually just need a factory function. If you think you need a member function, consider whether a functional pattern might suffice. Functional and immutable patterns are encouraged to reduce context switching and maintain simplicity.
```typescript
/**
* @description Discouraged class.
*/
class Tree{

  name : string;
  germDate : date;

  constructor(name : string, germDate: Date){

    this.name = name;
    this.germDate : Date;

  }

  changName(newName : string){

    this.name = newName;

  }

}
 
/**
* @description Encouraged factory.
* /
const Tree = (name : string, germDate : Date)=>{ // mkTree may be preferred in some contexts
  return {
    name : name,
    germDate : Date
  }
}
 
 /**
 * @description Discouraged factory for object with member function.
 * @ remarks
 * mkTree make be preferred in some circumstances.
 */
const Tree = (name : string, germDate : Date) : TreeI=>{
  return {
    name : name,
    germDate : Date
    updateName(newName : string){
      this.name = newName;
    }
  }
 }
 
 /**
 * @description Encouraged functional pattern.
 */
 const assignNewName = (tree : TreeI, newName : string) : TreeI=>{
  return {
    ...tree,
    name : newName
  }
 }

```
- Do not use inheritance. Good apps can be written without it. If you follow [Alan Kay](https://softwareengineering.stackexchange.com/questions/264697/alan-kay-the-big-idea-is-messaging), OO can is really about messaging. Maps and control flow are good tools for ensuring different responses to messages, and you can read them faster.

## Tests
Test React frontends with both [Jest](https://jestjs.io/) and [Cypress](https://www.cypress.io/). 
- Matching Jest unit tests must be written for all files contributed.
- Cypress can be used for unit, integration, and e2e testing as you please.

### Jest
Match Jest test files to their source by naming them `<filename>.test.{tsx,tsx}`.

### Cypress 
Use Cypress component testing. Match Cypress test files to their source by naming them `<filename>.cy.{tsx,tsx}`
