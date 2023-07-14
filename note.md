### Steps

step1: install vite

```jsx
npm create vite@latest ./

Select a framework: › React
Select a variant: › JavaScript

npm install
npm run dev
```

step2: install [tailwindcss](https://tailwindcss.tw/docs/guides/vite)

```jsx
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p

npm run dev
```

step3: install file-saver, react-router-dom

```jsx
npm install file-saver react-router-dom
```

step4: add client logic

step5: build server

```jsx
npm init -y

// add start script in package.json
"scripts": {
    "start": "nodemon index"
  },

npm install cloudinary cors dotenv express mongoose nodemon openai

// add type in package.json
"type": "module",
```

step6: get DB url from mongoDB

step7: build `Post` schema

```jsx
./mongo/models/Post.js

import mongoose from "mongoose";

const Post = new mongoose.Schema({
    name: { type: String, required: true},
    prompt: { type: String, required: true},
    photo: { type: String, required: true},
})

const PostSchema = mongoose.model("Post", Post)

export default PostSchema
```

step8: go OpenAI web and choose API and get API key