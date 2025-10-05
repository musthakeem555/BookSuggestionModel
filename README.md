# 📚 Kindle Book Recommender System

## 📘 Overview
This project implements a **Kindle Book Recommender System** that provides personalized book suggestions to users based on their reading preferences and past ratings.

The system uses:  
- **Exploratory Data Analysis (EDA):** Understand user demographics, book trends, and rating patterns  
- **Content-Based Filtering:** Recommends books similar to those a user has liked, based on book metadata  
- **Collaborative Filtering (Item-Based):** Recommends books based on **book-to-book similarity**, using ratings from users with similar preferences  

_This hybrid approach allows for accurate and personalized recommendations for Kindle users._

---

## 📂 Dataset
The dataset consists of three tables: **Users**, **Books**, and **Ratings**

### **Users Table**
| **Column** | **Description** |
|------------|----------------|
| `User-ID`  | Unique identifier for each user |
| `Location` | User's location (`city, state/province, country`) |
| `Age`      | User's age (if available) |

### **Books Table**
| **Column** | **Description** |
|------------|----------------|
| `ISBN`          | Unique identifier for each book |
| `Book-Title`    | Title of the book |
| `Book-Author` _optional_ | Name of the author |
| `Year-Of-Publication` _optional_ | Year of publication |
| `Publisher` _optional_ | Name of the publisher |

### **Ratings Table**
| **Column** | **Description** |
|------------|----------------|
| `User-ID`     | ID of the user giving the rating |
| `ISBN`        | ID of the book being rated |
| `Book-Rating` | Rating given by the user (numeric scale, e.g., 0–10) |

_Notes:_  
- All tables are linked using `User-ID` and `ISBN`  
- Item-based collaborative filtering uses **book-to-book similarity**  
- Ratings of `0` may indicate _not rated_ or _neutral_  

---

## 🛠️ Tools & Technologies
- **Python:** pandas, numpy, scikit-learn  
- **Jupyter Notebook** for EDA and modeling  
- **Visualization:** matplotlib, seaborn  

---
