# exo-react-2023

You are starting the checkpoint from scratch ! So you need to install everything.
You can either use :

- [create-react-app](https://create-react-app.dev/)


## :one: React

**In this step, you will create a web-app using React, that displays games from one of our API !**

_Please please, don't forget to make atomic commits with explicit messages_ :pray:

You can find the API documentation there :

- https://apis.wilders.dev/wild-games

### Starting point

- You can wipe all the boilerplate jsx code in `App.jsx`
- Then, create a `<Header />` component that displays a cool welcome message.
- Pass a `name` prop to this component, to display your website name (_react game_ if you don't have any idea)

_commit_ 

### Some list ?

- Your next mission is to display the full list of games.
- Start by creating two new components `<GameList />` and `<Game />`.
- In the `<GameList />` component, you will need to get the list from the API, and map it in your jsx. For each game you get from the API, display a `<Game />` component.
- Your `<Game />` component will need some props to display the game informations. There are plenty of informations you can use (_name, rating, images, ..._). Display them in the format of your choice !

_commit_ 

### Filtering

- Now that you are displaying all games, your next mission is to add a filter on this list.
- Add a `button` to the `<GameList />` component, when you click on it, it will display only the games whose rating is above `4.5`. When clicking again on this button, the list should display all the games again.

_again, don't forget to commit_ :wink:

### Details page

You are going to use `react-router-dom`

- Refactor your code to implement a router, with two routes :
  - `"/"` will display your `<GameList />`
  - `"/games/:id"` will display the next component you are going to create
- Create a `<GameDetails />` component, and use it in your `/games/:id` route.
- Then, you can add a navigation link (or button) to your `<Game />` component that will redirect to the details page of this game.
- The `<GameDetails />` component will need to fetch data from the API and display detailed information about the current game (what you choose to display is up to you !)

_you know what to do, right ?_ :wink:

- - -
### Congrats ! You did it ! :confetti_ball:


## Bonuses

If you have remaining time, here are some bonuses. As they are bonuses, they are **totally optional**, and you shouldn't do them if you haven't finished the previous steps.

### Removing a game

`<Game />` contains a `<button>` which allows you to remove a game from the list _(doesn't need to remove it in the API)_.

### Use a CSS framework

Integrate the CSS framework of your choice in your React App. 
If you don't know which one to choose, we can recommand Tailwind.

You can start by looking at the documentation about [how to install it](https://tailwindcss.com/docs/installation).

**Be careful !** :warning: If you choose to start using `create-react-app`, you will need to install CRACO, but every steps [are explained here](https://tailwindcss.com/docs/guides/create-react-app).
