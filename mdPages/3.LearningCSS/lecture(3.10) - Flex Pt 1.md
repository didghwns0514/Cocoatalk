<link href="../md_config/style.css" rel="stylesheet">

# Flex

## 1) Why it came out

- Developers wanted more easier ways to deal with boxes.
- Boxes were able to manipulated not regarding with the size of the monitor.

## 2) Additional height/width param

- **`Viewport height : it will change accordingly with the screensize.`**
- Example

  ```CSS
    content {
      display: flex;
      justify-content: space-between;
      align-items: center;
      height: 100vh;
    }
  ```

## 3) Rule

1. Rule 1

   - If you want to move elements, you must **`set flex property to the parent`**.
   - This makes the parent, a flex-container, which has main axis + cross-axis.
   - Example

     - You set flex to content-tag if you want to move div tags.
       ```HTML
           <main>
             <article>
               <content>
                 <div></div>
                 <div></div>
                 <div></div>
               </content>
             </article>
           </main>
       ```
       ```CSS
         content {
           display: flex;
         }
         div {
           width: 170px;
           height: 150px;
           background-color: teal;
         }
       ```
     - Result

       <img src="images/2021-08-03-16-41-50.png"/>

2. Rule 2

   - By Setting Flex property, **`You unlock other properties you can use`**
   - Example
     - properties
       1. Flex-end : Align to the end
       2. Flex-start : Defalut, align from the start
       3. Space-evenly : Display everything evenly
       4. Space-between : Display everything evenly and widely
       5. Center : Align to the center
       6. Stretch : Stretches the block / needs no fixed height or width
     - Center
       ```CSS
          content {
            display: flex;
            justify-content: center;
          }
       ```
     - Result
       <img src="images/2021-08-03-16-45-12.png"/>

3. Rule 3

- Flex also can effect vertically
- CSS vertical / horizontal axis
- [Link - MDN](https://developer.mozilla.org/ko/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox)
- Terms
  1. Main axis : control with **`Justify-content`**
  2. Cross axis : Control with **`Align-items`**
- Example  
  <img src="images/2021-08-03-22-19-34.png"/>
- <span style="color:red; font-weight:bold;">This Main(horizontal) / Cross axis(vertical) mapping can be changed later if you want to!</span>
