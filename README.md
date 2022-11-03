# Coding-Practices
This document lists out all the coding best practices we need to follow during our development
### Use only fucntional components
  Any new components we are writing should be functional components with hooks only, please avoid class components. 
### Avoid using multiple `state` variables, instead try using object if necessary
Try to avoid multiple state variables and try using objects instead for avoiding multiple re renders
```
const [username, setusername] = useState('')
const [password, setpassword] = useState('')
```
Insted of using this, try

```const [user, setuser] = useState({})```
### Organize Files Related to the Same Component in One Folder 
File structure is very important in react. Organise files in such a way that file can tracked down based on it's implementation.
For example files should be placed in folder structure similar to routes.
![image](https://user-images.githubusercontent.com/115486326/199731618-0084988c-c866-4b27-b958-95dd27fdb2c2.png)
https://levelup.gitconnected.com/2-simple-effective-react-file-naming-convention-tips-cce1022328a8
Refer this documentation
### Please follow URL and Variable naming conventions
![image](https://user-images.githubusercontent.com/115486326/199731963-c85be39e-255f-4333-87e8-c5152b877230.png)
Variables should be `pascalCase`
File name should be `CamelCase`
File name shoudl match class name
###  Opt for Fragments Instead of Divs Where Possible
Avoid using empty  `div` in component return statement
```
return <div><span>1</span><span>2</span></div>
```
Instead use `React Fragments <></>`
```
return <><span>1</span><span>2</span></>
```
### Reuse the code properly, don't repeat any code and maintin code consistency
Avoid repeating any code, instead re use existing code and maintain consistency
### Use linter in dev environment
TODO: Linter configuration should be shared across the team
