# Slogan scanner

Training computer vision models to perform brand and slogan detection on photos and screenshots.

# TODO:
- [ ] annotated dataset
- [ ] data pre-processing to improve image quality
- [ ] text extraction from pictures
- [ ] implementation of an NLP model as a supervised classifier
- [ ] pattern recognition with a CNN model

## Frontend

### General

#### 🔋 Stack: TypeScript, React, Tailwind
#### 💅 Code formatter: prettier
#### 📚 Libraries
- [x] [Base Mui](https://mui.com/base-ui/)
- [x] [Mui Charts](https://mui.com/x/react-charts/getting-started/)
- [x] [Tailwind UI](https://tailwindui.com/)

Using vite template:
```
npm create vite@latest my-app -- --template react-ts
```

### Usage

💅 Format your files:
```
npm run format
```

💻 Dev mode:
```
npm run dev
```

In an other terminal run tailwind for CSS:
```
npx tailwindcss -i ./src/style/input.css -o ./src/style/output.css --watch
```

🏗️ Build mode:
```
npm run build
```

🐋 Dockerize:
```
docker build -t frontend:latest .
docker run -p 3000:3000 frontend
```

## Backend

### General

#### 🔋 Stack: Python, FastAPI, SQLite
<!-- #### 💅 Code formatter: ? -->
#### 📚 Libraries
- [x] [BeautifulSoup](https://pypi.org/project/beautifulsoup4/)
- [x] [Requests](https://pypi.org/project/requests/)
- [x] [Pydantic](https://docs.pydantic.dev/latest/)
- [x] [SQLAlchemy](https://www.sqlalchemy.org/)

### Usage

```
uvicorn main:app --reload
```

Dockerize:
```
docker build -t backend:latest .
docker run -p 8000:8000 backend
```