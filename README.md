# List

## JavaScript
- [source map](http://blog.teamtreehouse.com/introduction-source-maps)

### React.js
- Component
    - Naming convention: start with capital
- All React components do not attempt to change their inputs.
- Using setters, React may batch ultiple setState() calls into a single update for performance
````
// will not re-render a component
this.state.comment = "hi"
// Correct
this.setState({comment: "hi"});
````
- setState() will do shallow merge.
- stateless component vs statefull component
- React events are named using camelCase
- prevent default behavior
````
// plain HTML
<a href="#" onclick="console.log('hi'); return false>
    click me
</a>
// In React
function ActionLink(){
    function handleClick(e) {
        e.preventDefault();
        ocnsole.log('hi');
    }
    return (
        <a href="#" onClick={handleClick}>
        Click me
        </a>
    );
}
````
- In JavaScript, class methods are not bound by default (https://facebook.github.io/react/docs/handling-events.html). ``this.handleClick = this.handleClick.bind(this)`` or React property initializer syntax``handleClick = () => {}``


