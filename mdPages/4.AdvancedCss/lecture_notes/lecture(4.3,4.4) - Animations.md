<link href="../md_config/style.css" rel="stylesheet">

# Animations

- Transition & Transform works with states defined
- Animations work when you want transformation activation without activation on states(eg. hover)
- What can be added as property?
  - border-radius, border-color, opacity ... but not everything can be added
  - Use "Transform" properties mainly
- [Site for animation sets you can look](https://animista.net/)
- Syntax

  - Types:
    1. From... to
    2. 0% 50% 100%; percentage syntax  
       You can do more than 3 steps if you want
  - Example
    > @keyframes \<name of your animation>  
    > from {  
    >  transfrom:  
    > }  
    > to  
    > {  
    >  transform:  
    > }

  <br>

  > Note: Write where you want an animation-effect  
  > ... {  
  >  animation: \<name of your animation> \<time> \<method> \<method> ...  
  > }

## Animations

- Example 1

  - HTML
    ```HTML
      <article>
        <div>
          <a href="#">Go Home</a>
        </div>
        <div>
          <img src="img/hj_logo.png" />
        </div>
      </article>
    ```
  - CSS
    ```CSS
      section img {  // this will automatically apply
        margin: 5px;
        height: 100px;
        width: 100px;
        border: 3px solid grey;
        border-radius: 50%;
        animation: coinFlippersYay 5s ease-in-out;
        // You can also do this if you want infinite loop
        // animation: coinFlippersYay 5s ease-in-out infinite;
      }
      section img:hover {  // this when the state activation hover is True
        transform: rotateY(70deg) rotateX(20deg) scaleX(1.2) translateY(-20px);
      }
    ```

- Example 2

  - CSS

    ```CSS
      @keyframes coinFlippersYay {
        0% {
          transform: rotateX(0);
        }
        50% {
          transform: rotateY(180deg) translateY(-50px);
        }
        100% {
          transform: rotateY(360deg) rotateX(360);
        }
    ```

  - Result
    <img src="images/screencast%202021-08-17%2006-08-41.gif" />
