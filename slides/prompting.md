## Prompting

Prompting is used to ask the user options for the generator.

```javascript
prompting: function () {
  var done = this.async();

  // Have Yeoman greet the user.
  this.log(yosay(
    'Welcome to the fine' + chalk.red('Test') + ' generator!'
  ));

  var prompts = [{
    type: 'confirm',
    name: 'someOption',
    message: 'Would you like to enable this option?',
    default: true
  }];

  this.prompt(prompts, function (props) {
    this.someOption = props.someOption;

    done();
  }.bind(this));
}
```
It uses [Inquirer.js](https://github.com/SBoudrias/Inquirer.js)
