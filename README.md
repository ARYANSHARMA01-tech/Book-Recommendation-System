
# 📚 Book Recommendation System

This is a **Content-Based Recommendation System** for books, built using **Python**, **Flask**, and **Machine Learning**. It suggests books to users based on the content similarity of books (titles, authors, etc.). The application uses preprocessed and pickled data models for fast recommendations.

---

### 🌐 Live Demo

🔗 **[Click here to try it live](https://book-recommendation-system-9vxu.onrender.com/)**

---

![App Screenshot 1](https://drive.google.com/uc?id=1fl4fwFPdn67uYcN8PVA_CRkFzu60CKi_)
![App Screenshot 2](https://drive.google.com/uc?id=1qtClo--il_pl8Fohqa-1SWL-pqlqJnsN)
![App Screenshot 3](https://drive.google.com/uc?id=19RqqIg4r8ydybc1BXjptQn-VqqwoL5LA)

---

## 🚀 Features

- Homepage showing popular books with average rating, votes, and book cover.
- Recommendation page where user can input a book title and get similar recommendations.
- Content-based filtering using cosine similarity on book features.

---

## 🔧 Tech Stack

- **Frontend**: HTML, CSS, Jinja2 (via Flask Templates)
- **Backend**: Python, Flask
- **ML Model**: Content-Based Filtering using Cosine Similarity
- **Libraries Used**: `numpy`, `pandas`, `pickle`, `flask`

---

## 📁 Files Included

```
├── app.py                  # Flask application  
├── templates/  
│   ├── index.html          # Homepage  
│   └── recommend.html      # Recommendation UI  
├── static/                 # CSS / JS (if any)  
├── popular.pkl             # Pickled DataFrame for popular books  
├── pt.pkl                  # Pickled Pivot Table for content filtering  
├── books.pkl               # Pickled books metadata  
├── similarity_scores.pkl   # Cosine similarity scores  
```

---

## 💡 How It Works

1. **Homepage** loads the most popular books from `popular.pkl`.
2. **Recommendation System** takes user input, searches the pivot table (`pt.pkl`) and finds the index.
3. Cosine similarity is used to compute similarity scores from `similarity_scores.pkl`.
4. The top similar books are fetched from `books.pkl` and displayed.

---

## 🛠️ Installation & Run Locally

### 1. Clone the Repo

```bash
git clone https://github.com/your-username/book-recommendation-system.git
cd book-recommendation-system
```

### 2. Create Virtual Environment

```bash
python -m venv venv
```

### 3. Activate the Virtual Environment

- For Windows:
```bash
venv\Scripts\activate
```

- For macOS/Linux:
```bash
source venv/bin/activate
```

### 4. Install Requirements

```bash
pip install flask numpy pickle-mixin
```

### 5. Run the App

```bash
python app.py
```

Then open `http://127.0.0.1:5000` in your browser.

---

## 📬 Contact

For any feedback or suggestions:

- **Aryan Sharma**  
- [LinkedIn: aryan-sharma-671817322](https://www.linkedin.com/in/aryan-sharma-671817322)
