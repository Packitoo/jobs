
# React-Redux Developer challenge:

## Instructions

The goal of this challenge is to see how comfortable you are using React, Redux and to learn how to use our front-end stack.

For this challenge the stack is composed of the following libraries :

- Typescript https://create-react-app.dev/docs/adding-typescript
- ReactJs https://reactjs.org/
- Material-ui https://material-ui.com/
- Redux https://redux.js.org/
- React-redux https://github.com/reduxjs/react-redux / https://react-redux.js.org/introduction/quick-start
- Redux-Persist https://github.com/rt2zz/redux-persist
- Redux-dev-tools https://github.com/zalmoxisus/redux-devtools-extension
- Redux-saga https://redux-saga.js.org/ (or Redux-Thunk)
- Formik https://formik.org/
- Reselect (Export logic from view into selector) https://github.com/reduxjs/reselect
 https://redux.js.org/recipes/computingderiveddata

The folder structure should be feature-based. You can find an example here https://github.com/ryanlanciaux/react_feature_folder_example

All these libraries must be installed using **yarn**

**Important**

In order for us to verify your progress, you'll need to have at least one commit for each level. You can host your repository publicly on your Github/Gitlab profile, or send us a copy of the entire folder (including the .git folder).

## Let's go!

We are going to build one page with two components.

One component for the creation of a brief/summary of a packaging to build and one for list all these summaries.

These 2 components should be independant in the page. And at the end your main App.js should look like this :

```javascript
  return (
    <div>
      <BriefForm />
      <BriefList />
    </div>
  );
```

---

### Level #0 - Boilerplate

Since this is the first level, let's go easy.

First create the project structure. For this you should use create-react-app (https://github.com/facebook/create-react-app).

Next you will have to install all other necessary tools : Redux / React-redux / Redux-Saga (You can install Redux-dev-tools for debugging)

You will also have to install a fake REST Api (https://github.com/typicode/json-server).

A db.json file is already present in this folder and you must use it.

To do all your request you can use whatever you want (fetch/axios...)

> **Level #0 - Checklist**
>
> - [ ] Prepare the project structure using create-react-app
> - [ ] Install libraries Redux / React-redux / Redux-Saga / json-server

---

### Level #1 - Setup Redux / React-redux

Now that you have installed all libraries, we need to setup them.

Setup redux, react-redux and redux-saga.

For this setup you should create store / reducers / actions / actions type.

This architecture is called flux and works like this :

# <img height="150" src="https://facebook.github.io/flux/img/flux-simple-f8-diagram-with-client-action-1300w.png" alt="flux-architecture" />

If you have any doubt on what's a store or a reducer or flux, you should read redux docs or find your answer on the internet.

> - [ ] Setup Redux / React-redux / Redux-saga (create store / reducer / actions creator / actions type)

---

### Level #2 - Start brief creation form

Everything is setup, now we can start coding our first component of the page : the brief creation form.

The brief form will have 3 fields :
 - Title (String)
 - Comment (Text)
 - ProductId (Relation Id)

Title and Comment are simple text input and the value of these inputs are stocked in the state of the component

For the product id, what you need to do is to fetch products data from json-server fake api and stock them in the store.

For this you should :
- Create an action who is responsible of fetching products data, this action will be called in ComponentDidMount lifecycle method of the BriefForm component (https://reactjs.org/docs/react-component.html) and your component should be connected to redux by connect method from react-redux to work.
- The action will dispatch a type of action with product data in the payload to the reducer and the reducer will stock it in store
- The component will be connected by connect method from react-redux and products data would be available in props (Use mapStateToProps to do this)
- Get products data from props and create a Select input to select a product for the brief creation
- Selected product will be store in the state of the component like text and comment

At the end of this level you should have a form with 2 text inputs and 1 select input. All the data of these inputs should store their values in the component state.

> **Level #2 - Checklist**
>
> - [ ] Create BriefForm.js
> - [ ] Fetch products from json-server fake api and stock fetched products in the store (use connect of react-redux)
> - [ ] Get products data from props (use connect of react-redux)
> - [ ] Create a form div with 3 inputs inside (title, comment and products)
> - [ ] Store title, comment and product id value in state of the component (https://reactjs.org/docs/forms.html)
> - [ ] Add a submit button to create the brief

---

### Level #3 - Create a brief

Now that we have a beautiful form who collect data, the last step is to send this data to the server for create a brief.

To do this, like previous step we will use an action. The action will send data to the fake json rest api. (POST request)
On the response, the server will return the brief created, the action should dispatch this data and store it in briefs data of the store.

> **Level #3 - Checklist**
>
> - [ ] Create an action to create a brief
> - [ ] Launch this action on onClick of submit button
> - [ ] Store brief created from server's response to store

---

### Level #4 - ListBrief Component

Now we have our BriefForm Component, it's time to create the second component.

The goal of this component is to fetch briefs data and display them in a list. To do this use what you learned on previous level.

The data displayed should be :
  - title
  - comment
  - product name

When a brief is created from the form bellow, it must be automatically displayed in the list.

> **Level #4 - Checklist**
>
> - [ ] Fetch Briefs data
> - [ ] Display Them
> - [ ] Implement the routes

---

### Level #5 - Filter brief in BriefList by product

The goal is to add a select input in BriefList where you can select a product and then it will filter brief by the selected product. The best way to do this is to use reselect library.

> **Level #5 - Checklist**
>
> - [ ] Filter Briefs

---

### Requirements


#### Requirement #1. Use Reselect in BriefList

In BriefList we are directly manipulating data from the store in the view to access product name of brief for example.

A good practice is to use a "selector" to manipulate data of the store and set the results in props of the component. With this practice the view is just in charge of displaying the data and nothing more.

You can implement this functionality using Reselect https://github.com/reduxjs/reselect

### Requirement #2. Use Typescript

We use typescript in our projects.

---

### Bonus level 💪

All right! You didn't have enough, well we've got more! If you want to show off your skills, now is the time.

Here are a few things that you can do. You are not required to do all of them, but be sure to have at least one commit for every task.

#### Bonus #1. Inform user of requests with Loader

At the moment when briefs data are fetching or when you are waiting for the server's response the user doesn't know that it's loading.

Fix this and add a loader on every request to inform user of what's happening.

#### Bonus #2. Style our App

We didn't talk about the style of the app because it's not the main goal of this challenge.

But if you want to, you can design your app using Material-UI library. https://material-ui.com/

#### Bonus 3. Cypress tests

An very important part of what we do is testing, we use cypress.io to make tests, you can add a test with this
