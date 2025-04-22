# React-Vite deployment using GitHub Pages

> Reference : [Click here](https://youtu.be/hn1IkJk24ow?si=mqOZyurEs1KvL7Ke)

### Step 1: Add `base` URL in `vite.config.js`

```javascript
 base: "/repositoryName",
```

Commit: [Refer Here](https://github.com/SudirKrishnaaRS/react-vite-deployment-template/commit/f55ac5033d7b56ccd64ff0bd2dbcbd3e8017a516)


![image](https://github.com/user-attachments/assets/53a4c06c-ec31-45de-ab30-6febbdc7878f)

### Step 2: Add `homepage` key in package.json

```javascript
  "homepage": "https://sudirkrishnaars.github.io/repositoryName/",
```

Commit: [Refer Here](https://github.com/SudirKrishnaaRS/react-vite-deployment-template/commit/1a3bd7facccd57b939efa3b7f5faa3dac4f052ec)


![image](https://github.com/user-attachments/assets/5f9fb3ec-795c-437d-8d9f-0a1448f15b5f)

### Step 3: Install `gh-pages` npm package

```
 npm install gh-pages
```

### Step 4: Add scripts for predeploy and deploy in package.json

```javascript
  "predeploy": "npm run build",
  "deploy": "gh-pages -d dist" 
```

Commit: [Refer Here](https://github.com/SudirKrishnaaRS/react-vite-deployment-template/commit/04393aa6b8ac1188cc84a64761e123c3f741c3e4)


![image](https://github.com/user-attachments/assets/19369638-d672-4958-b6d9-32aee6893076)

### Step 5: Run the below command(in VS Code) to start the deployment

```
 npm run deploy
```

### Step 6: Congratulations ✨, your site would be live now 🚀

> NOTE: The above steps are not automated, hence you'll need to run `npm run deploy` to trigger a re-deployment

---

## React + Vite 

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh
