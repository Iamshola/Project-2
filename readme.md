![ga_cog_large_red_rgb](https://cloud.githubusercontent.com/assets/40461/8183776/469f976e-1432-11e5-8199-6ac91363302b.png) x <img width="220" alt="Screenshot 2019-09-16 at 19 37 39" src="https://user-images.githubusercontent.com/43203736/64984044-d6743480-d8b9-11e9-83ad-59a729cb64ee.png">


# Project 2: CocktailBored


### Installation

* Clone or download the repo
* Run `yarn init` in the CLI
* Run `yarn serve` in the CLI


## Overview
The completed project can be viewed [here](https://iamshola.github.io/Project-2/#/).

## Project Brief

### The brief requirements were:

* **Consume a public API** – this could be anything but it must make sense for your project.
* **Have several components** - At least one classical and one functional.
* **The app should include a router** - with several "pages".
* **Include wireframes** - that you designed before building the app.
* Have **semantically clean HTML** - you make sure you write HTML that makes structural sense rather than thinking about how it might look, which is the job of CSS.
* **Be deployed online** and accessible to the public.


### Project Reflection

### Technologies used
  - REACT
  - CSS
  - HTML
  - Javascript
  - Lodash
  - Bulma

### Timeframe:
  2 days


### Approach taken
As a team, we agreed on out basic MVP and gave ourselves just under half of the total time frame to complete. This would give us enough contingency time for any bugs or additional features we'd like to implement.

Our basic MVP included;
- An index page
- A filter which allows the user to enter am ingredient of their choice
- A navbar which is fully routed.

Once we had completed this, we decided to think more about the design and colour themes. We both agreed as this was a predominately alcohol based website, we wanted colours that screamed maturity and class yet quite fresh.

Lastly, we used some of our existing functions to build on more filters and sorters as seen on our index page.

#### Wireframes
![IMG_20190802_084348](https://user-images.githubusercontent.com/43203736/62653578-b9ad1e80-b955-11e9-8ee5-b37f6ab0aa11.jpg)


![IMG_20190802_084315](https://user-images.githubusercontent.com/43203736/62653654-e3664580-b955-11e9-9693-7aed03f7f966.jpg)


![IMG_20190802_084332](https://user-images.githubusercontent.com/43203736/62653660-e7926300-b955-11e9-8271-d9dcf66a0a09.jpg)



<img width="985" alt="Screenshot 2019-08-07 at 20 51 04" src="https://user-images.githubusercontent.com/43203736/62653898-88811e00-b956-11e9-81c1-5d3b39084366.png">

###  Snippets of code

##### Sort function
```Javascript
<section className="section">
  <div className="container">
    <div className="field">
      <input placeholder="Search your favourite drink" className="input" onKeyUp={this.handleKeyUp}/>
    </div>

    <label> Alphabetical Order:  </label>
    <select onChange={this.handleChange}>
      <option value="strDrink|asc">A-Z </option>
      <option value="strDrink|desc">Z-A </option>
    </select>
    <br />
    <br />

    <div className="columns is-multiline">
      {this.filterCocktails().map(cocktail =>
        <div className="column is-half-tablet is-one-quarter-desktop"
          key={cocktail.idDrink}
        >
          <Link to={`/cocktails/${cocktail.idDrink}`}>
            <Card name={cocktail.strDrink} image={cocktail.strDrinkThumb}/>
          </Link>
        </div>
      )}
    </div>
  </div>
</section>
```

##### Search function to make entries case insensitive
``` Javascript
filterCocktails(){
  const re = new RegExp(this.state.searchTerm, 'i')

  const filterCocktails = _.filter(this.state.cocktails, cocktail => {
    return re.test(cocktail.strDrink)
  })

  return filterCocktails
}
```


### Preview of site













### Wins and Blockers

#### Wins:

I like the final appearance of the project particularly how tidy and easy to navigate it is. Additionally, for my first group project I believe Alexis and I got on very well and helped each other patch up some of our grey areas from the teaching aspect of the module.

#### Blockers:
One  downfall we had as a group, was not understanding our API fully and the features we could implement. As a result, we lost time trying to access data we couldn't thus not being able to add more complex features as seen on most websites.  

### Future features
I would love to add more filters such as filter by ingredients which allows the user to ask the following style of question 'Does the drink contain sprite, vodka and lemon?'. This can be achieved by selecting multiple radio buttons and manipulating the GET request to the API.


### What you have learned (tech & soft skills)

#### Tech skills:
This project was a good opportunity to solidify my knowledge around react and using APIs. In addition to this, I believe this has highlighted good and bad features of APIs which will prove useful in my next project.

#### Soft skills:
Communication between myself and my team mate.
Organisation
Detailed planning and plan of execution
understanding how important time is in the execution of a project.


### Course Curriculum
  Details of my training and links to more projects whilst at General Assembly -  12 Week Immersive.

> **Week 1-3 | Module One - Fundamentals**

  - HTML5
  - CSS3
  - Sass
  - JavaScript


> **Week 4**

  Project 1 : Frogger  | [GitHub](https://github.com/Iamshola/project-01) | [GH-Pages](https://iamshola.github.io/project-01/)

>**Week 5 | Module Two - React**

  - React.js
  - Routing
  - RESTFUL API
  - Third-party APIs

>**Week 6**

  Project 2 : CocktailBored  | [GitHub](https://github.com/Iamshola/Project3) | [GH-Pages](https://iamshola.github.io/Project-2/#/)

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
