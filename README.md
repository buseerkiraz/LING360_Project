# Mom, What's For Dinner?

## Overview

**"Mom, What's For Dinner?"** is a computational linguistics project designed to recommend recipes based on user input.  
The system interacts with the user by asking two specific questions, encodes the responses using a Hugging Face sentence transformer model, and then recommends the most suitable recipe.

### Interaction Flow

1. **What are you craving?:**  
   The user describes what they feel like eating.

2. **What do you have in your fridge?:**  
   The user lists the available ingredients.

Based on these inputs, the program finds the best matching recipe and displays the following:

- 📝 **Recipe name**  
- 🧂 **List of missing ingredients** (based on what's not already in the fridge)  
- ⏱️ **Preparation time**  
- 👩‍🍳 **Step-by-step instructions**

After showing the recipe, the program asks:

> **Did you like this recipe? Yay or Nay?:**

- If the answer is **"Yay"**, it prints: Amazing! Bon appetit!

- If the answer is **"Nay"**, it presents the **second-best recipe** based on the initial input.

---

## Dataset

The recipe data is sourced from the **[Food.com Recipes and Interactions](https://doi.org/10.34740/KAGGLE/DSV/783630)** dataset on Kaggle, which contains over **180,000 recipes** from Food.com (formerly GeniusKitchen).

> **Citation**:  
> Shuyang Li. (2019). *Food.com Recipes and Interactions* [Data set]. Kaggle. https://doi.org/10.34740/KAGGLE/DSV/783630

---

## How to Use

1. Download and unzip the project files.
2. Open the included **Google Colab** notebook file.
3. Run the notebook.
4. Enter your input when prompted:
 - What are you craving?
 - What do you have in your fridge?
5. Get your personalized recipe recommendation.
6. Respond to the "Yay or Nay" prompt to get either a confirmation or a second-best suggestion.

---

## Technologies Used

- Python
- Hugging Face Sentence Transformers
- Pandas, NumPy
- Food.com Recipes Dataset
