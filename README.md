# Notes of a lifetime ☝️ 🕋

**All the following stuff are preserved for personal use as the key things are very crucial**

-   [Tailwind CSS](#tailwind-css) 🟣
-   [React Fundamentals](#react-fundamentals) 🔵

---

## 👉 Tailwind CSS 🟣

**Extensions / Plugins**

-   [Twin.macro](#twin.macro)
-   [Headwind](#headwind)
-   [Tailwind Docs](#tailwind-docs)
-   [TailwindCSS Debug Screens](#tailwindcss-debug-screens)

**UI library**

-   [TailBlocks](#tailblocks)
-   [Tailwind Toolbox](#tailwind-toolbox)

---

#### 🟣Twin.macro

[url](https://github.com/ben-rogerson/twin.macro) | [extension](https://marketplace.visualstudio.com/items?itemName=lightyen.tailwindcss-intellisense-twin)

**use-case :**

-   make code look cleaner
-   organized [css at pne portion + using those predefined elements in the next part]

---

#### 🟣Headwind

[extension](https://marketplace.visualstudio.com/items?itemName=heybourn.headwind)

**use-case :** the classes are sorted as they should be

---

#### 🟣Tailwind Docs

[extension](https://marketplace.visualstudio.com/items?itemName=austenc.tailwind-docs)

**use-case :** can direct to the website of the specific searched topic form vs code

---

#### 🟣TailwindCSS Debug Screens

[url](https://github.com/jorenvanhee/tailwindcss-debug-screens)

**use-case :** can show on what screen size we are in during development

---

#### 🟣TailBlocks

[url](https://tailblocks.cc/)

**use-case :** UI component library

---

#### 🟣Tailwind Toolbox

[url](https://www.tailwindtoolbox.com/)

**use-case :** UI component library

---

---

## 👉 React Fundamentals 🔵

**Topics**

-   [Conditional Rendering vs Ternary Op.](#conditional-rendering-vs-ternary-op)

---

#### 🔵 Conditional Rendering vs Ternary Op

**Issue :**

-   Conditional Rendering only works on boolean values
-   If the passed props is not boolean then JS may see it otherwise

<br/>

🔴

    render() {
        let isLoggedIn = true; // will work fine

        // let isLoggedIn -> 0 or hello etc
        // will not work

        return (
        <div className="App">
            <h1>
            This is a Demo showing several ways to implement Conditional Rendering in React.
            </h1>
            {isLoggedIn && <button>Logout</button>}
        </div>
        );
    }

**Solution :** use ternary operator

🟢

    render() {
        let isLoggedIn = true; // will work fine

        // let isLoggedIn -> 0 or hello etc
        // will work

        return (
        <div className="App">
            <h1>
            This is a Demo showing several ways to implement Conditional Rendering in React.
            </h1>
            {isLoggedIn ? <button>Logout</button> : <button>Login</button>}
        </div>
        );
    }
