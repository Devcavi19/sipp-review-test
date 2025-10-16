# CS4116 SIPP Quiz Reviewer

A comprehensive interactive quiz application for **CS4116 - Social Issues and Professional Practice** covering all four modules.

## 📚 Modules Covered

- **Module 1**: Ethics & Business Ethics
- **Module 2**: Professional Codes & IT Ethics
- **Module 3**: Cybersecurity
- **Module 4**: Privacy & Freedom

## ✨ Features

- 🎯 **Module Selection**: Choose from 4 different modules
- 📊 **Customizable Quiz Length**: 10, 15, 20, 30, or 40 questions
- 🎭 **Question Type Filtering**: All questions, Multiple Choice only, or True/False only
- 🔄 **Adaptive Learning**: Follow-up questions on missed topics
- 📈 **Real-time Statistics**: Score, streak, accuracy tracking
- 🎯 **Weak Topic Analysis**: Identifies areas needing improvement
- ⌨️ **Keyboard Shortcuts**: Enter (submit), N (next), S (skip)
- 📱 **Responsive Design**: Works on desktop, tablet, and mobile

## 🚀 Deployment to GitHub Pages

### Method 1: Via GitHub Website (Easiest)

1. **Create a new repository** on GitHub
   - Go to [github.com](https://github.com)
   - Click "New repository"
   - Name it: `sipp-quiz-reviewer` (or any name you prefer)
   - Make it **Public**
   - Don't initialize with README (we already have one)

2. **Upload files**
   - Click "uploading an existing file"
   - Drag and drop all files:
     - `index.html`
     - `mcq1.json`
     - `mcq2.json`
     - `mcq3.json`
     - `mcq4.json`
     - `README.md`
   - Commit the files

3. **Enable GitHub Pages**
   - Go to repository Settings
   - Scroll to "Pages" section
   - Under "Source", select "Deploy from a branch"
   - Choose branch: `main` (or `master`)
   - Choose folder: `/ (root)`
   - Click Save

4. **Access your site**
   - Your quiz will be live at: `https://yourusername.github.io/sipp-quiz-reviewer/`
   - It may take 1-2 minutes to deploy

### Method 2: Using Git Command Line

```bash
# Navigate to this directory
cd "C:\Users\Asus\OneDrive - Camarines Sur Polytechnic Colleges\Documents\4thYear\SIPP\Reviewer\SIPP_revTest"

# Initialize git repository
git init

# Add all files
git add index.html mcq1.json mcq2.json mcq3.json mcq4.json README.md

# Commit
git commit -m "Initial commit: SIPP Quiz Reviewer"

# Add remote (replace YOUR_USERNAME and REPO_NAME)
git remote add origin https://github.com/YOUR_USERNAME/REPO_NAME.git

# Push to GitHub
git branch -M main
git push -u origin main
```

Then enable GitHub Pages in repository settings as described in Method 1, step 3.

## 📖 How to Use

1. **Select a Module**: Choose from the dropdown (Module 1-4)
2. **Configure Quiz**:
   - Select question type filter (All/MC only/TF only)
   - Choose number of questions (10-40)
3. **Start Quiz**: Click "Start Quiz" button
4. **Answer Questions**:
   - Select your answer
   - Click "Submit" to check
   - Read the explanation
   - Click "Next" for the next question
5. **Review Performance**: Check weak topics in the sidebar

## 🎮 Keyboard Shortcuts

- **Enter**: Submit answer
- **N**: Next question
- **S**: Skip question

## 📁 File Structure

```
SIPP_revTest/
├── index.html          # Main quiz application
├── mcq1.json          # Module 1 questions
├── mcq2.json          # Module 2 questions
├── mcq3.json          # Module 3 questions
├── mcq4.json          # Module 4 questions
└── README.md          # This file
```

## 🔧 Technical Details

- **Pure HTML/CSS/JavaScript**: No dependencies, no build process
- **Static Site**: Runs entirely in the browser
- **JSON-based**: Easy to add/edit questions
- **Mobile-responsive**: Adapts to all screen sizes

## 📝 Adding New Questions

Edit the respective `mcqX.json` file with this format:

```json
{
  "id": 1,
  "question": "Your question text here?",
  "choices": ["Option A", "Option B", "Option C", "Option D"],
  "answer": "Option B",
  "explanation": "Explanation of the correct answer.",
  "topic": "Topic Name"
}
```

For True/False questions:
```json
{
  "id": 2,
  "type": "TF",
  "question": "Statement to evaluate?",
  "answer": true,
  "explanation": "Explanation here.",
  "topic": "Topic Name"
}
```

## 🎨 Customization

Edit the CSS variables in `index.html` to customize colors:

```css
:root {
  --bg: #0b132b;        /* Background */
  --panel: #1c2541;     /* Panel background */
  --card: #3a506b;      /* Card background */
  --acc: #5bc0be;       /* Accent color */
  --text: #eaeaea;      /* Text color */
  --warn: #ffb703;      /* Warning color */
  --bad: #ef476f;       /* Error color */
  --good: #06d6a0;      /* Success color */
}
```

## 📄 License

This project is for educational purposes for CS4116 students.

## 👨‍💻 Support

For issues or questions, please open an issue on GitHub.

---

**Made with ❤️ for CSPC CS4116 Students**
