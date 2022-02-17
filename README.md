# react-material-tree-checkbox
An improvised JS version of Typescript data-driven TreeView https://codesandbox.io/s/edeyu?file=/src/App.tsx

![alt text](https://www.dropbox.com/s/x9dgpjgbbtbd5gs/react-material-tree-checkbox.png?raw=1)

## Impprovisation

When data array has children property set but it is in form of an array and is empty. Hence:

Replaces

    if (!nodes.children) {
      return null;
    }
    
with

    if (!nodes.children || nodes.children.length <=0 ) {
      return null;
    }
