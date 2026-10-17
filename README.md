# 📚 Book Finder — Python GUI Application

A colorful and interactive desktop application built with **Python, PyQt5, and the APILayer API** that helps users discover books by title, topic, or author. Users can view book covers, explore search results, find places to purchase books, and search for online reading previews.

## ✨ Features

- 🔍 **Book Search:** Search for books by title, topic, or author.
- 🎨 **Modern GUI:** Beautiful purple, blue, and pink gradient background.
- 📖 **Book Covers:** Display available book cover images.
- 🗂️ **Book Cards:** View book titles and book IDs in organized cards.
- 🛍️ **Purchase Links:** Find online shopping results for books.
- 📚 **Reading Previews:** Search for online previews and ebook reading options.
- ⚡ **Background Searching:** Uses PyQt5 threads to keep the interface responsive while searching.
- ⚠️ **Error Handling:** Displays messages for API authentication problems, connection failures, timeouts, and usage limits.
- 🖥️ **Scrollable Results:** Browse multiple books in a scrollable grid layout.

## 🛠️ Technologies Used

- **Python** — Main programming language.
- **PyQt5** — Desktop graphical user interface.
- **Requests** — Makes HTTP requests to the book search API.
- **APILayer / APILieague API** — Retrieves book search results.
- **OS** — Reads the API key from an environment variable.
- **Webbrowser** — Opens book purchasing and reading search links.
- **urllib.parse** — Encodes book titles for URLs.

## 📋 Requirements

Before running the application, make sure you have:

- Python 3 installed.
- An API key for the book search API.
- An internet connection.

## 🚀 Installation

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

Replace `YOUR_GITHUB_REPOSITORY_URL` with your actual GitHub repository URL.

### 2. Navigate to the project folder

```bash
cd YOUR_PROJECT_FOLDER
```

### 3. Install the required libraries

```bash
pip install PyQt5 requests
```

### 4. Configure your API key

The application reads its API key from the `BOOK_API_KEY` environment variable. Configure it before running the program.

**Windows Command Prompt:**

```cmd
set BOOK_API_KEY=YOUR_API_KEY
```

**Windows PowerShell:**

```powershell
$env:BOOK_API_KEY="YOUR_API_KEY"
```

Replace `YOUR_API_KEY` with your actual API key.

Keep your API key private. Do not publish it in your GitHub repository.

### 5. Run the application

```bash
python book_finder.py
```

Replace `book_finder.py` with the actual name of your Python file if it is different.

## 🖱️ How to Use

1. Open the Book Finder application.
2. Enter a book title, author, or topic in the search box.
3. Click **Search Books** or press Enter.
4. Browse the displayed book cards.
5. Click **Buy This Book** to search for purchasing options.
6. Click **Read / Preview** to search for online reading previews and ebook options.

## 🎨 Design

The application uses a modern color scheme featuring:

- Deep purple: `#4937B8`
- Purple: `#6D5AE6`
- Blue: `#4388F5`
- Pink: `#E879C6`

Rounded buttons, book cards, cover images, and a gradient background give the application a colorful desktop experience.

## ⚙️ API Information

The application sends requests to the book search endpoint:

```text
https://api.apileague.com/search-books
```

It uses the `x-api-key` request header and sends search parameters to retrieve books.

API availability, authentication, and request limits depend on your API provider and subscription plan.

## ⚠️ Important Notes

- Book results depend on the API response and availability.
- Some books may not have cover images.
- The Buy and Read / Preview buttons open Google search results. They do not guarantee that a book is available for purchase or that its full text is available to read.
- The application does not download or display entire books. Reading links may provide previews, excerpts, or other available information.
- Never commit your API key to a public repository.

## 🔮 Future Improvements

Possible upgrades include:

- Add filters for authors, genres, and publication dates.
- Add a favorites list.
- Save search history.
- Add pagination for larger result sets.
- Display book descriptions, ratings, and publication dates.
- Integrate direct links to legitimate ebook previews and libraries.
- Improve the layout for different window sizes.

## 👨‍💻 Project Purpose

This project is designed to practice Python GUI development, API integration, HTTP requests, multithreading, error handling, and opening web links from a desktop application.

## 📄 License

You may add an open-source license, such as the MIT License, if you want other developers to reuse and modify your project.

---

**Built with Python and PyQt5. 📚💜**
