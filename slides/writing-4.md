## Copying files with variables

```javascript
this.fs.copyTpl(
  this.templatePath('config/Provision/playbook.yml'),
  this.destinationPath('Provision/playbook.yml'),
  {
    'app_name': this.projectName
  }
);
```

This will replace
```bash
<%= app_name %>
```
in
```bash
templates/config/Provision/playbook.yml
```
with the content in
```javascript
this.projectName
```
and copy the result to
```bash
Provision/playbook.yml
```
