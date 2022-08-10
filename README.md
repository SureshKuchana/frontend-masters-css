# Frontend Masters CSS Animations Workshop

Welcome to the [Frontend Masters CSS Animations Workshop](https://frontendmasters.com/courses/css-animations/)! In this workshop, you will:

- Learn how to design meaningful animations that improve the user experience in websites and web apps
- Become proficient in creating animations with CSS and JavaScript
- Craft consistent motion design with CSS variables
- Create choreographed, synchronized animation sequences
- Make CSS animations reactive and dynamic with JavaScript
- Orchestrate animated transitions easily with state machines
- Get inspired and experience many animation demos

## Getting started

1. Clone this repo
2. Install npm dependencies:

```bash
npm install # or yarn
```

3. Run the project in dev mode:

```bash
npm run dev # or yarn dev
```

4. Go to [localhost:3000](https://localhost:3000) to see the running app.

You should now be able to access each of the sections:

<ul>
  <li><a href="/00-fundamentals/">Lesson 00: Fundamentals</a></li>
  <li><a href="/01-transitions/">Lesson 01: Transitions</a></li>
  <li><a href="/02-keyframes/">Lesson 02: Keyframe Animations</a></li>
  <li><a href="/03-choreography/">Lesson 03: Choreography</a></li>
  <li><a href="/04-states/">Lesson 04: States</a></li>
  <li><a href="/05-layout/">Lesson 05: Layout Animations</a></li>
  <li><a href="/06-reactive/">Lesson 06: Reactive Animations</a></li>
  <li><a href="/examples/inflight/">Inflight Example</a></li>
</ul>

#### CSS allows animation of HTML elements without using JavaScript or Flash!

- @keyframes
- animation-name
- animation-duration
- animation-delay
- animation-iteration-count
- animation-direction
- animation-timing-function
- animation-fill-mode
- animation

above properties are the animation property.

```
// sample example
h1 {
  animation: slide-right 1s linear infinite;
}

@keyframes slide-right {
  from {
    transform: translateX(ease 1s);
  }
  to {
    transform: translateX(50vw);
  }
}
```

#### CSS Variables

you can actually define custom css variables inside any selector's html, body.
To use the custom css varible `color : var(--primary-color)`
you can override the variable value `--primary-color : "red"`

### CSS Transitions

`transition-property: background, transform`
`transition-timing-function: linear, ease-in-out`
`transition-duration: 1s, 2s`

or

`transition: all 2s 0.5s ease-in-out`

```
// sample example
transition-property: background, transform;
transition-timing-function: linear, ease-in-out;
transition-duration: 1s 0.5s;

// transition-duration: 0;
// NOTE : you cannot do transition-duration: 0, it might cause animation break

&:hover {
  transition-duration: 1s 0.5s;
  background: blue;
  transform: scale(2);
}

<!-- when i hove over on the ball it is immediatley
  transition to blue
 -->
```
