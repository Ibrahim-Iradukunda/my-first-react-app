# react-dev-week-2-react-app

## Guided Learning Activity: Creating Your First React App with TypeScript and Vite

### Goal

Build a simple React app that displays a heading and paragraph using a custom component styled with CSS.

### Prerequisites

- Node.js version 16 or later and npm. Verify with `node -v` and `npm -v`.
- A code editor such as VS Code.
- Basic terminal, HTML, CSS, and JavaScript knowledge.

### Getting Started

1. Create a new public GitHub repository for this activity.
2. Clone the repository locally.
3. Add this `README.md` file to the repository root.
4. Create the Vite project:

   ```bash
   npm create vite@latest my-first-react-app -- --template react-ts
   cd my-first-react-app
   npm install
   npm run dev
   ```

5. Open the local URL shown by Vite, usually `http://localhost:5173/`.
6. Type the code yourself while following the steps. Do not copy and paste the provided code directly.
7. Commit and push meaningful progress incrementally.

### Project Structure

- `index.html`: The HTML entry point for the React app.
- `src/main.tsx`: Renders the root `App` component.
- `src/App.tsx`: The main application component.
- `src/App.css`: Styles for the app layout.
- `src/MyComponent.tsx`: The custom React component.
- `src/MyComponent.css`: Styles for the custom component.
- `package.json`: Project dependencies and scripts.
- `tsconfig.json`: TypeScript configuration.
- `vite.config.ts`: Vite configuration.

### Create `MyComponent`

Create `src/MyComponent.tsx`. Import React and `./MyComponent.css`, define a `MyComponent` functional component, and render:

- A `div` with `className="my-component"`.
- An `h1` containing `Hello from MyComponent!`.
- A paragraph containing `This is a paragraph of text within my component.`.

Export `MyComponent` as the default export.

### Use the Component in `App.tsx`

Import `MyComponent` from `./MyComponent` and `./App.css`. Render `<MyComponent />` inside a `div` with `className="App"`.

### Style the Component

Create `src/MyComponent.css` and style `.my-component` with a light-blue background, 20px padding, a 1px blue border, a 5px border radius, and centered text. Style the heading navy and the paragraph with a 16px font size.

Optionally style `.App` in `App.css` with flexbox so the component is centered and has a minimum height of `100vh`.

### Run and View

Run `npm run dev`, open the local Vite URL, and confirm that the styled heading and paragraph are displayed without errors.

### GitHub Expectations

- Make multiple meaningful commits during the activity.
- Push changes progressively rather than uploading everything at the end.
- Use clear commit messages describing the work completed.
- Keep the repository clean and do not commit `node_modules` or other generated files.
- Include all files needed to install and run the project.
- Push the latest completed work before submitting the repository URL on Canvas.

### Rubric Checklist

- **Functionality and component structure:** The app runs, `MyComponent` is separate, and `App.tsx` imports and renders it.
- **TypeScript and code quality:** Code is clear, formatted, organized, and uses appropriate React and TypeScript conventions.
- **Component design and styling:** Styles are separated into `MyComponent.css` and applied with `className`.
- **GitHub practices:** The repository shows incremental meaningful commits, descriptive messages, a clean structure, and no `node_modules`.

### Further Exploration

- Learn how to pass props into components.
- Explore React state.
- Learn about more complex styling approaches.
- Read the [Vite documentation](https://vitejs.dev/), [React documentation](https://react.dev/), and [TypeScript documentation](https://www.typescriptlang.org/).
