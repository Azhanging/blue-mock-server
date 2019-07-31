# blue-mock-server
mock server in your cli tool

## Example

vue.config.js(vue-cli 3.x) 
```javascript
const mockServer = require(`blue-mock-server`);

module.exports = {
  devServer:{
    before(app){
      mockServer({
        app,          //express instance
        mockDir: ``,  //mock api dir,some file change,update new router in this server(resolute path)
        apiFilePath: ``   //mock api entry,(resolute path,this file in mockDir)
      });
    }
  }
};
```

## Go Example
- [blue-vue-program](https://github.com/Azhanging/blue-vue-program/blob/master/apps/blue-vue-tmpl/vue.config.js) 

