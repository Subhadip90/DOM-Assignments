# Dom Manipulation Assignment

1. Webiste Name: [Dev To](https://dev.to/)

### Topics

    - Query Selector, Inner HTML

### Sample Image

![Sample One](./Images/Pic1.png)

### Tasks

        Target the Top description div and change the DEV Community to <Your_Name> and description to your passion

### Output Code

```
document.querySelector(".crayons-layout .sidebar-wrapper .side-bar .crayons-card .crayons-subtitle-2").innerHTML = "iNeuron";

document.querySelector(".crayons-layout .sidebar-wrapper .side-bar .crayons-card .color-base-70").innerHTML = "I Write Code";
```

### Output Image

![Assignment_1_Output](./Images/Pic2.png)

---

2. Website Name: [Apple](https://support.apple.com/en-in)

### Task

![Store](./Images//Picture_3.png)

### Fetch all the product name and store in an array

### Output

['iPhone', 'Mac', 'iPad', 'Watch', 'AirPods', 'Music', 'TV']

### Output Code

```
let arr = [];
document.querySelectorAll(".as-imagegrid-item").forEach((e) => {
  arr.push(e.innerText.replace("\nSupport", " "));
})
console.log(arr);
```

### Output Image

## ![Output Image](../Assignment%20Output%20Images/2.JPG)

3. Webiste Name: [Youtube Support](https://support.google.com/youtube/)

### Topics

    - Get Element By Id, Create Element, Create Text Node, Append Child

### Sample Image

![Sample One](./Images//Pic4.png)

### Tasks

     Add another FAQ 'My New FAQ' to the list

### Output code

```
const hcfe_content = document.getElementById("hcfe-content");
const dropdown = document.querySelector(".primary-container .page-width-container .main-content .article .accordion-homepage");
const item = document.createElement("section");
item.className = "parent";
const text = item.innerHTML = "<h3>My New Faq </h3>";
dropdown.append(item);
```

### Expected Output

![Output](./Images//Pic5.png)

### My Output image

## ![Output Image](../Assignment%20Output%20Images/3.JPG)

4. Webiste Name: [OnePlus](https://www.oneplus.in/support)

### Topics

     Query Selector, InnerText

### Sample Image

![Sample One](./Images/Pic6.png)

### Tasks

      Change the contact number

### Output code

```
document.querySelector(".customer-support .service-number").innerText = "+91 6366256689";
```

### Expected Output

![Output](./Images/Pic7.png)

### My Output Image

![Output Image](../Assignment%20Output%20Images/4.JPG)

---

5. Webiste Name: [Samsung](https://www.samsung.com/in/offer/online/samsung-fest/)

### Topics

       getElementById, createElement, InnerText, append, setAttribute

### Sample Image

![Sample One](./Images/Pic8.png)

### Tasks

     Target the main div of card and change the Button text to Check out

### Expected Output

![Output](./Images/Pic9.png)

### Output code

```
document.querySelector(".feature-column-carousel__button .cta").innerText = "Check Out";
```

### My Output Image

![My Output Image](../Assignment%20Output%20Images/5.JPG)

---

6. Webiste Name: [Adidas](https://www.adidas.co.in/)

### Topics

    -   Query Selector, Event listeners, Changing Styles

### Sample Image

![Sample One](./Images/Pic10.png)

### Tasks

     Target the search box and on hover change thebackground color to red.

### Expected Output

![Output](./Images/Pic11.png)

### Output code

```
document.querySelector(".searchinput-wrapper___18TsX .searchinput___zXLAR").addEventListener('mouseover', function () {
  document.querySelector(".searchinput___zXLAR").style.backgroundColor = "Red";
});
```

### My Output Image

![My Output Image](../Assignment%20Output%20Images/6.JPG)

---

7. Webiste Name: [MDN Web Docs](https://developer.mozilla.org/en-US/)

### Topics

       Form, Value, Submit

### Sample Image

![Sample One](./Images/Pic12.png)

### Tasks

     To Search a topic in the MDN Search bar.
     First add a text to search in the search bar and then hit the submit search button to search the docs using DOM

### Expected Output

![Output](./Images/Pic13.png)

### Output code

```
function search(Text) {
  let input = document.querySelector("#hp-search-input");
  input.value = Text;
  let form = document.querySelector("#hp-search-form");
  form.submit();
}
search("CSS Selector");
```

### My Output Image

![My Output Image](../Assignment%20Output%20Images/7.JPG)

---

8. Webiste Name: [Google](https://www.google.com/)

### Topics

       Remove Elements

### Sample Image

![Sample One](./Images/Pic14.png)

### Tasks

     Remove alternate languages from the home page languages listed

### Expected Output

![Output](./Images/Pic15.png)

### Output Code

```
const elements = document.querySelectorAll("#SIvCob a");
for (i = 0; i < elements.length; i++) {
  if(i % 2 == 0) {
    elements[i].remove();
  }
}
console.log(elements);
```

### My Output Image

![My Output Image](../Assignment%20Output%20Images/8.JPG)

---

9. Webiste Name: [Code Wars](https://www.codewars.com/)

### Topics

       Change Font Family, Color of Text.

### Sample Image

![Sample One](./Images/Pic16.png)

### Tasks

    Change the font family of the text to monospace and text color to the logo’s background color.

### Expected Output

![Output](./Images/Pic17.png)

### Output Code

```
document.querySelector(".display-heading-1").style.fontFamily = "Monospace";
document.querySelector(".display-heading-1").style.color = "Red";
```

### My Output Image

![My Output Image](../Assignment%20Output%20Images/9.JPG)

---

10. Webiste Name: [Freecodecamp](https://www.freecodecamp.org/)

### Topics

       querySelector, mouseover, click eventListener,  callback function, style,

### Sample Image

![Sample One](./Images/Pic18.png)

### Tasks

    Target the button and change background colour on mouseover

### Expected Output

![Output](./Images/Pic19.png)

### Output Code

```
document.addEventListener('mouseover', function () {
  document.querySelector(".login-btn-text").style.backgroundColor = "red";
});
```

### My Output Image

![My Output Image](../Assignment%20Output%20Images/10.JPG)

---

11. Webiste Name: [realme](https://www.realme.com/in/)

### Topics

       querySelector,style,background-image

### Sample Image

![Sample One](./Images/Pic20.png)

### Tasks

    change the realme logo to ineuron logo

### Expected Output

![Output](./Images/Pic21.png)

### Output Code

```
document.querySelector(".logo .icon").style.backgroundImage = "url('https://ineuron.ai/images/ineuron-logo.png')";
```

### My Output Image

![My Output Image](../Assignment%20Output%20Images/11.JPG)

---

12. Webiste Name: [Github](https://github.com/)

### Topics

       querySelector,style,background-Color

### Sample Image

![Sample One](./Images/Pic22.png)

### Tasks

     change the background colour of the button to blue.

### Expected Output

![Output](./Images/Pic23.png)

### Output Code

```
document.querySelector(".btn-primary").style.backgroundColor = "blue";
document.querySelector(".btn-primary").style.color = "white";
```

### My Output Image

![My Output Image](../Assignment%20Output%20Images/12.JPG)

---

13. Webiste Name: [Hackerrank](https://www.hackerrank.com/)

### Topics

       querySelector,innerHtml

### Sample Image

![Sample One](./Images/Pic24.png)

### Tasks

Target the top description and change “Matching developers with great companies” to ‘JSBOOTCAMP“.

### Expected Output

![Output](./Images/Pic25.png)

### Output Code

```
document.querySelector(".fl-heading-text").innerText = "JSBOOTCAMP";
```

### My Output Image

![My Output Image](../Assignment%20Output%20Images/13.JPG)

---

14. Website Name: [Asus](https://www.asus.com/in/)

### Topics

      querySelector,style,font-size

### Sample Image

![Sample One](./Images/Pic26.png)

### Tasks

       change the fontsize of “Hot Deals” to 80px

### Expected Output

![Output](./Images/Pic27.png)

### Output Code

```
document.querySelector(".HotDealsAll__Heading__2fIbe").style.fontSize = "80px";
```

### My Output Image

![My Output Image](../Assignment%20Output%20Images/14.JPG)

---

15. Webiste Name: [Dell](https://www.dell.com/en-in/shop/deals/laptop-deals?gacd=10415953-9016-5761040-285981356-0&dgc=ST&gclid=Cj0KCQjwguGYBhDRARIsAHgRm4-XUDMhhVNyHXb3s1gY4ZBzORr_d9Se-buhJwy7asyUe7YdqEA11eEaAt6UEALw_wcB&gclsrc=aw.ds&nclid=BxjBlpBQsX6pjSHh-L8YYSU77EpfXRkG1AGMB5Wbeu386ykspfrPDnfx_DdFau20)

### Topics

      querySelector,style.textAlign

### Sample Image

![Sample One](./Images/Pic28.png)

### Tasks

       Convert the text “G15 Gaming Laptop” from left to right

### Output

![Output](./Images/Pic29.png)

### Expected Output

```
document.querySelector(".ps-top .ps-title").style.textAlign = "right";

```

### My Output Image

![My Output Image](../Assignment%20Output%20Images/15.JPG)

---

16. Webiste Name: [Vercel](https://vercel.com/)

### Topics

     querySelector,innerHTMl

### Sample Image

![Sample One](./Images/Pic30.png)

### Tasks

      change the heading “Start with the developer” to “Start with Scratch”

### Expected Output

![Output](./Images/Pic31.png)

### Output Code

```
document.querySelector(".section-title_title__VEDfK").innerText = "Start With Scratch";

```

### My Output Image

## ![My Output Image](../Assignment%20Output%20Images/16.JPG)

---

17. Webiste Name: [Sony](https://www.sony.co.in/)

### Topics

    querySelector,innerHTML

### Sample Image

![Sample One](./Images/Pic33.png)

### Tasks

     change the button text To current Date.

### Expected Output

![Output](./Images/Pic32.png)

### Output Code

```
document.querySelector(".btn-container .btn").innerHTML = new Date();
```

### My Output Image

![My Output Image](../Assignment%20Output%20Images/17.JPG)

---

18. Webiste Name: [Philips](https://www.philips.co.in/)

### Topics

     querySelector,style,backgroundcolor

### Sample Image

![Sample One](./Images/Pic34.png)

### Tasks

    change the background colour blue to orange

### Expected Output

![Output](./Images/Pic35.png)

### Output Code

```
document.querySelector(".p-f03-footer-container").style.background = "orange";
```

### My Output Image

![My Output Image](../Assignment%20Output%20Images/18.JPG)

---

19. Webiste Name: [Canon](https://in.canon/)

### Topics

          querySelector,src

### Sample Image

![Sample One](./Images/Pic36.png)

### Tasks

    extract the canon logo

### Expected Output

![Output](./Images/Pic37.png)

### Output Code

```
document.querySelector(".navbar-brand .logo").innerText = "https://in.canon/assets/brand/logo-300-002e45a4aec98fd92899838da9d5560f.png"
```

### My Output Image

![My Output Image](../Assignment%20Output%20Images/19.JPG)

---

20. Webiste Name: [Oppo](https://www.oppo.com/in/)

### Topics

          querySelector,style,color

### Sample Image

![Sample One](./Images/Pic38.png)

### Tasks

      Change the description colour black to orange

### Expected Output

![Output](./Images/Pic39.png)

### Output Code

```
document.querySelector(".desc").style.color = "orange"
```

### My Output Image

![My Output Image](../Assignment%20Output%20Images/20.JPG)
