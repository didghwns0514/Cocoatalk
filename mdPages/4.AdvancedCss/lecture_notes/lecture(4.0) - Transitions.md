<link href="../md_config/style.css" rel="stylesheet">

# Transition

- Requires some state
- Switching States is the very definitino of Transition of CSS.

## 1) State

- Example

  - HTML
    ```HTML
      <section>
        <article>
          <div>
            <a href="#">Go Home</a>
          </div>
        </article>
      </section>
      <aside></aside>
    ```
  - CSS
    ```CSS
      section a {
        color: white;
        background-color: tomato;
        text-decoration: none;
        padding: 3px 5px;
        border-radius: 5px;
      }
      section a:hover {
        color: tomato;
        background-color: white;
      }
    ```

## 2) Transition

- To add a state, you must add the property to a CSS where it does not have a State(eg: :hover)
- You need this because everything changes so quickly! -> you want some smooth effects
- This works because I added a State in the element(and the element has changed property in CSS)
  1. Something (a property) needs tobe changed in the state heading to
  2. Transition property knows this and does the animation work for you.

<br>

- Syntax
  > **`transition : <What to change> <how long> ease-in-out`**
  > ease-in-out :
- Example

  - CSS : before

    ```CSS
      section {
        margin: 5px;
        height: 30vh;
        max-height: 60vh;
        background-color: wheat;
        padding: 8px;
      }

      section a { // you should add state here
        color: white;
        background-color: tomato;
        text-decoration: none;
        padding: 3px 5px;
        border-radius: 5px;
        font-size: 30px;
      }
      section a:hover {
        color: tomato;
        background-color: white;
      }
    ```

  - CSS : after

    - CSS

      ```CSS
        section a {
          color: white;
          background-color: tomato;
          text-decoration: none;
          padding: 3px 5px;
          border-radius: 5px;
          font-size: 30px;
          transition: background-color 10s ease-in-out, color 5s ease-in-out;

          /* We can also do this */
          transition: all 5s ease-in-out;
        }
        section a:hover {
          color: tomato;
          background-color: white;
        }
      ```
