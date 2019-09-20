![ga_cog_large_red_rgb](https://cloud.githubusercontent.com/assets/40461/8183776/469f976e-1432-11e5-8199-6ac91363302b.png) x <img width="220" alt="Screenshot 2019-09-16 at 19 37 39" src="https://user-images.githubusercontent.com/43203736/64984044-d6743480-d8b9-11e9-83ad-59a729cb64ee.png">

# Project 2: CocktailBored
###### View Site [Here](https://iamshola.github.io/Project-2/#/)

### Installation

* Clone or download the repo
* Run `yarn init` in the CLI
* Run `yarn serve` in the CLI

## Overview
Cocktailbored is a platform where users can search, filter and sort different alcoholic drinks all from an external API. Launch on [gh-pages](https://iamshola.github.io/Project-2/#/). Check out the [GitHub](https://github.com/Iamshola/Project-2). Many thanks to [TheCocktailDB](https://www.thecocktaildb.com/) for this API.

## Project Brief

### The brief requirements were:

* **Consume a public API** – this could be anything but it must make sense for your project.
* **Have several components** - At least one classical and one functional.
* **The app should include a router** - with several "pages".
* **Include wireframes** - that you designed before building the app.
* Have **semantically clean HTML** - you make sure you write HTML that makes structural sense rather than thinking about how it might look, which is the job of CSS.
* **Be deployed online** and accessible to the public.

### Process
As a team, we agreed on out basic MVP and gave ourselves just under half of the total time frame to complete. This would give us enough contingency time for any bugs or additional features we'd like to implement.

Our basic MVP included;
- An index page
- A filter which allows the user to enter am ingredient of their choice
- A navbar which is fully routed.

We built our wireframes based on this MVP.

#### Wireframes:
<img width="985" alt="Screenshot 2019-08-07 at 20 51 04" src="https://user-images.githubusercontent.com/43203736/62653898-88811e00-b956-11e9-81c1-5d3b39084366.png">

#### Languages and Technologies Used:
  - REACT
  - CSS
  - HTML
  - Javascript
  - Lodash
  - Bulma

#### Timeframe:
  2 days

#### Preview of site

![ezgif com-video-to-gif (3)](https://user-images.githubusercontent.com/43203736/65348901-1d279e80-dbda-11e9-9c4c-5109c345c45b.gif)


### Features

> **All Features:**

  - Sort through cocktails
  - Search through cocktails
  - Filter through Cocktails
  - View show pages of the cocktail
  - Navigate through different pages using react router
  - Read the About us sections


## Wins and Blockers

### Wins:

#### Sort
This is the function that allowed the users to sort through the cocktails alphabetically.

```Javascript
    <label> Alphabetical Order:  </label>
    <select onChange={this.handleChange}>
      <option value="strDrink|asc">A-Z </option>
      <option value="strDrink|desc">Z-A </option>
    </select>
    <br />
    <br />
```
#### Search
This is the function that allowed case sensitive searches in our input bar.

``` Javascript
filterCocktails(){
  const re = new RegExp(this.state.searchTerm, 'i')

  const filterCocktails = _.filter(this.state.cocktails, cocktail => {
    return re.test(cocktail.strDrink)
  })

  return filterCocktails
}
```

#### Soft skills:
This was my first time pair programming and I believe the communication between myself and my team mate was very good and this made the process enjoyable. We were organised and had a detailed plan and plan of execution and an understanding of how important time was in the execution of a project.

### Blockers:
One  downfall we had as a group, was not understanding our API fully and the features we could implement. As a result, we lost time trying to access data we couldn't thus not being able to add more complex features as seen on most websites.  

### Future features
I would love to add more filters such as filter by ingredients which allows the user to ask the following style of question 'Does the drink contain sprite, vodka and lemon?'. This can be achieved by selecting multiple radio buttons and manipulating the GET request to the API.


## Course Curriculum
  Details of my training and links to more projects whilst at General Assembly -  12 Week Immersive.

> **Week 1-3 | Module One - Fundamentals**

  - HTML5
  - CSS3
  - Sass
  - JavaScript


> **Week 4**

  Project 1 : Frogger  | [GitHub](https://github.com/Iamshola/project-01) | [gh-pages](https://iamshola.github.io/project-01/)

>**Week 5 | Module Two - React**

  - React.js
  - Routing
  - RESTFUL API
  - Third-party APIs

>**Week 6**

  Project 2 : CocktailBored  | [GitHub](https://github.com/Iamshola/Project3) | [gh-pages](https://iamshola.github.io/Project-2/#/)

>**Week 7-8 | Module Three - Node and Express**

  - RESTFUL Routing
  - Node.js
  - Express
  - Token Authentication & Session Authentication
  - API Creation
  - Mocha and Chai

>**Week 9**

  Project 3 : Date-a-base | [GitHub](https://github.com/Iamshola/Project3) | [Herouku](https://datingexp.herokuapp.com/#/)

>**Week 10-11 | Module Four - Python and Django**

  - Python
  - SQL
  - Django
  - Token Authentication

>**Week 12**

  Project 4 : Space | [GitHub](https://github.com/Iamshola/project-04) | [Herouku](https://date-a-base-aos.herokuapp.com/#/)


  ### Contact
  Adesola Oni-Shogbonyo\
  Email : s.oni-shogbonyo@hotmail.co.uk\
  [Portfolio](https://iamshola.github.io/) | [Linkedin](https://www.linkedin.com/in/adesola-oni-shogbonyo/) | [GitHub](https://github.com/Iamshola)
​
