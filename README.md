# CSS

## initialise
```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box; 
  // border+padding not added to width/height.
}

body {
  font-family: "Lato", sans-serif;
  font-weight: 400;
  font-size: 16px;
  line-height: 1.7;  // 70% higher than normal
  color: #777
}
```

## centering

```css
position: absolute;
top: 50%;
left: 50%;
transform: translate(-50%, -50%);
```
centre block in block element
```css
margin: 0 auto;
```

```css


```
## animation
```css

.class {
  animation-name: moveInLeft;
  animation-duration: 1s;
  animation-iteration-count: 2;
  animation-delay: 1s;
  // wait with dispalting animation
}

@keyframes moveInLeft {
  0% {
    opacity 0;
    transform: translateX(-100px);
  }

  80% {
    transform: translateX(20px);
  }

  100% {
    opacity 1;
    transform: translateX(0);
  }
}

```
## pseudo classes

```css
a:link,
a:visited,
a:hover,
a:active {

}

.class:not(:last-child){
  
}


```

## pseudo element
create a new element with css

```css
.class::afer {
  content: "";
  display: inline-block;
  height: 100%;
  width: 100%;
  position: absolute;
  top: 0;
  left: 0;
}


```

## transition

```scss
.heading-secondary {
    font-size: 3.5rem;
    text-transform: uppercase;
    font-weight: 700;
    display: inline-block;
    background-image: linear-gradient(to right, $color-primary-light, $color-primary-dark);
    -webkit-background-clip: text;
    color: transparent;
    letter-spacing: .2rem;
    transition: all .2s;

    &:hover {
        transform: skewY(2deg) skewX(15deg) scale(1.1);
        text-shadow: .5rem 1rem 2rem rgba($color-black, .2);
    }
}

```