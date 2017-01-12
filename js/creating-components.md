## Create a Component

At the top of `index.js`, create a `Hello` component using the following code:

```jsx
const Hello = () => <div>Hi there!</div>
```

## Use the Hello Component in Your Main Component

Replace `it's working` with an instance of your component:

```jsx
export default () => <div><Hello/></div>
```


Your entire `index.js` file should now look like the following:
```jsx
const Hello = () => <div>Hi there!</div>

export default () => <div><Hello/></div>
```

## Say Hello to Yourself

Components receive `props` that you display inside the Component.

The `name="John"` below:
```
<Hello name="John"/>
```

Is passed into the `Hello` component as `props`.
Then you display the name using `{props.name}`:
```
const Hello = props => <div>Hi {props.name}!</div>
```

`index.js` should now look like the following:

```
const Hello = props => <div>Hi {props.name}!</div>

export default () => <div><Hello name="John"/></div>
```

Your webpage at [http://localhost:3000](http://localhost:3000) should
now display: 

```Hi John!```