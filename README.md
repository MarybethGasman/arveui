
# Arveui
Yet another component library with Vue3.


# Quick start
You need [Vue.js](https://vuejs.org) version 3.2+

## 1. Install via npm
```
npm install arveui
```

## 2. Import

You can import the library depending on the project needs. Import all components globaly, import single components globaly or import individual component where it's used.

- Declare all components globaly.

    **main.ts**

    ```
    import VueLibraryLoader from 'arveui';

    const app = createApp(App);
    app.use(VueLibraryLoader);
    ```

- Declare global components (Treeshaking).

    **main.ts**

    ```
    import { HelloWorld } from 'arveui';

    const app = createApp(App);
    app.component('HelloWorld', HelloWorld);
    ```

- Declare components localy.
    
    **\*.vue**

    ```
    <script setup lang="ts">
    import { HelloWorld } from 'arveui';
    </script>
    ```


## 3. Use components

Implement each component normally on the template section **\*.vue**
    
```
<template>
<HelloWorld msg="Message test" color="green" />
</template>
```
# Acknowledgement
