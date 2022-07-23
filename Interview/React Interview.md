## 1. The differnece between React.Fragment and div
- The main difference between React.Fragment vs div is that using a React.Fragment will not add any additional elements into the DOM tree, whereas, using a div will add a div to the DOM tree.

```jsx
export default function App() {
  return (
    <div>
      <p>Hello</p>
      <p>World</p>
    </div>
  );
}
```
### Result
```html
<div>
  <p>Hello</p>
  <p>World</p>
</div>
```


```jsx
export default function App() {
  return (
    <React.Fragment>
      <p>Hello</p>
      <p>World</p>
    </React.Fragment>
  );
}
```
### Result
```html
<p>Hello</p>
<p>World</p>
```