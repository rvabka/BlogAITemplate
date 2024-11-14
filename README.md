# HTML Article Generator Application

This tool allows you to generate structured HTML code based on the content of an article and a prompt passed to the OpenAI API. The application also enables the addition of `<img>` tags with appropriate attributes indicating places for images.

---

## Prerequisites

- **OpenAI API Key** – make sure you have your API key.
- **Text file with the article** – paste the content of the article into the `tekstArtykulu.txt` file.

---

## Running Instructions

### 1. Cloning the repository

Copy the code below and run it in the terminal:

```bash
git clone https://github.com/rvabka/zadanieOxido
cd zadanieOxido
```

### 2. Installing dependencies

Run the following command to install the necessary Node.js modules:

```bash
npm install
```

### 3. Entering the OpenAI API key

In the `main.js` file, find the place marked for entering the key and input your OpenAI API key:

```javascript
const API_KEY = new OpenAI({
  apiKey: "YOUR_API_KEY"
});
```

### 4. Preparing the article content

In the `tekstArtykulu.txt` file, paste the content of the article you want to send to the API.

### 5. Running the application

In the terminal, run the following command to generate the HTML file:

```bash
node main.js
```

### Result

The generated `artykul.html` file will be saved in the working directory. You will find the article content in HTML format with placeholders for images and appropriate HTML tags.

---

## File Structure

- `main.js` – the main application file, connecting to the OpenAI API, sending data, and saving the resulting HTML (`podglad.html`, `artykul.html`).
- `tekstArtykulu.txt` – txt file with the article content.
- `artykul.html` – the generated HTML file with the article.
- `szablon.html` – an optional template file for previewing the article.
- `podglad.html` – an optional full preview of the article.

---

## Example Invocation

To generate HTML from an article, follow these steps:

1. Place the article content in the `tekstArtykulu.txt` file.
2. Enter the API key in the `main.js` file.
3. Run `node main.js`.

The ready HTML file can be found under the name `artykul.html` in the working directory.

---

## Notes

If you want to customize the formatting, you can modify the `szablon.html` file to adjust the style and preview of the generated article.
