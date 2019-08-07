![ga_cog_large_red_rgb]

# Project 2 - REACT APP

### Technical Requirements and Project Overview
The second project is to **build a React application** that consumes a **public API**.
The completed project can be viewed at https://iamshola.github.io/Project-2/#/
​
Your app must:
​
* **Consume a public API** – this could be anything but it must make sense for your project.
* **Have several components** - At least one classical and one functional.
* **The app should include a router** - with several "pages".
* **Include wireframes** - that you designed before building the app.
* Have **semantically clean HTML** - you make sure you write HTML that makes structural sense rather than thinking about how it might look, which is the job of CSS.
* **Be deployed online** and accessible to the public.


## Project Reflection

### Technologies used
  - REACT
  - CSS
  - HTML
  - Javascript
  - Lodash
  - Bulma

### Approach taken - Thought process & methods of producing it
  - Basic MVP including couple searches from a public API

#### Wireframes
![IMG_20190802_084348](https://user-images.githubusercontent.com/43203736/62653578-b9ad1e80-b955-11e9-8ee5-b37f6ab0aa11.jpg)

![IMG_20190802_084315](https://user-images.githubusercontent.com/43203736/62653654-e3664580-b955-11e9-9693-7aed03f7f966.jpg)

![IMG_20190802_084332](https://user-images.githubusercontent.com/43203736/62653660-e7926300-b955-11e9-8271-d9dcf66a0a09.jpg)

<img width="985" alt="Screenshot 2019-08-07 at 20 51 04" src="https://user-images.githubusercontent.com/43203736/62653333-43a8b780-b955-11e9-9b02-16e93e092d10.png">


###  Snippets of your code and screenshots of your project and wireframes

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

### Wins and Blockers
Wins:
I like the final look of the project. I believe its clean, well designed

Blockers:
We should have understood our API better to decide which features we'd like to include in our App.

### Future features
   More filters such as filter by ingredients such as 'does their drink contain sprite, vodka and lemon'.


### What you have learned (tech & soft skills)

#### Tech skills:
This project was a good opportunity to solidify my knowledge around react.

#### Soft skills:
Communication between myself and my team mate.
Organisation
Detailed planning and plan of execution

​
