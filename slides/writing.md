## Writing
Most common use cases are copying files, templating files, creating directories...

```javascript
writing: {
  config: function () {
    ...
  },
  app: function () {
    this.fs.copy(
      this.templatePath('_package.json'),
      this.destinationPath('package.json')
    );
    this.fs.copy(
      this.templatePath('_bower.json'),
      this.destinationPath('bower.json')
    );
  }
}
```
