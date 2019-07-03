# React Assessments

Try your best to answer each question on your own before looking up the answer online. Once you're done writing your first answer, you can google the question and write the best answer you find.

#### 1. Here is a list of pros and cons to using the React library to build your application -- but some of them are false. Remove the false statements from the list:

- React was created to be simple, so that even people with minimal code experience could use it and create Single Page Applications (SPAs)
- React is a modern, efficient answer to complex UI applications
false - React is a full stack framework for modern web applications
- React is a flexible library that plays the role of V in an MVC framework


 #### 2. What are "smart"(logic) and "dumb"(display) components? Explain the difference and also add why we bother to make the distinction between them.

Smart component is a component with a state defined in a constructor. Smart components contain callback functions that are used to update the state and get passed down to their chid components as props.
Dumb component is a component without a state, their only job is to present to the DOM.



#### 3. When we use "yarn add ..." in the terminal - what is yarn doing?
#### And what file will always be automatically updated after we add a package with yarn?

A package is simply a folder with code and a package.json file that describes the contents. When you want to use another package, you first need to add it to your dependencies. This means running yarn add [package-name] to install it into your project.
This will update your package.json and your yarn.lock so other developers working on th project will get the same dependencies as you when they run yarn or yarn install

#### 5. There are three mistakes in this code that would cause it to break our application. Find the mistakes and fix them:

import React, { Component } from 'react'

class Recipes extends Component{
  constructor(props){
    super(props)
    this.state = {
      recipes : [
          {name: 'Meatballs'},
          {name: 'Mac & Cheese'}]
    }
  }
  render() {
      let recipes = this.state.recipes.map(function(recipe){
        return(
          <li key={recipe.name}>{recipe.name}</li>
        )
      })
      return (
        <ul>{recipes}</ul>
      )
  }
}

export default Recipes

#### 6. Name three html input types. (NOTE: text is the default type - so it doesn't count in this case)

 //Your Answer
 <password>
 <file>
 <checkbox>

 //Googled Answer
 <password>
 <file>
 <checkbox>

 #### 7. How would you explain state to a friend who doesn't know code?
Its how something/anything/certain thing behaves in a certain situation and time.


 #### 8. What is the difference between component state and props? Your answer should include a short explanation of both.

In React Component data flows in one direction, from parent to a child.
Props are variables passed by parent component to a child component.
State is directly initialized and managed by the component.
State is an object that determines how the component renders and behaves. State allows you to create components that are dynamic and interactive.


#### 9. Write a paragraph or so about your experience with building tic-tac-toe. Some topics to start with might be: things you learned about yourself, concepts from React that stood out to you, something about pair programming (if you paired), or the experience of building something in code from scratch.
