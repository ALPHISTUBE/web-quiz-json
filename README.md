# JSON Quiz Exam Application

## Description

This is a web-based JSON Quiz Exam Application. Upload or paste JSON quiz data,
convert various JSON formats into a unified quiz format, filter questions by 
category, and take timed or untimed exams. Supports review and retake features
for incorrect questions and provides syntax-highlighted JSON editing and 
conversion tools.

---

## Features

- Upload JSON quiz data by drag & drop or file selector.
- Support multiple JSON formats:
  - Array of question objects.
  - Object with categories as keys and arrays of questions.
- Filter questions by categories across tabs: All, Quiz, Review, Help & Convert.
- Timed and No-time exam modes with customizable question count and per-question time.
- Options to exclude recently asked questions or repeat only incorrect ones.
- Interactive exam interface with submit and skip.
- Review results with detailed stats.
- Syntax-highlighted JSON editor with error detection.
- Convert JSON with flexible key mapping for category, question, answer.
- Accessibility support for keyboard and screen readers.

---

## Supported JSON Formats

### Format A: Array of question objects

```json
[
  {
    "category": "Math",
    "question": "What is 2 + 2?",
    "answer": "4"
  },
  {
    "category": "Science",
    "question": "What is H2O?",
    "answer": "Water"
  }
]
```
### Format B: Object with categories as keys and question arrays as values
```json
[
  "Math": [
    {
      "question": "What is 2 + 2?",
      "answer": "4"
    }
  ],
  "Science": [
    {
      "question": "What is H2O?",
      "answer": "Water"
    }
  ]
]
```
Use the Help & Convert tab to map keys and convert formats correctly.

# How to Use
## Upload & Load Questions
Drag & drop or select a .json file in the upload section.

Or paste JSON in Help & Convert tab and click Convert & Load JSON.

JSON must follow one of the supported formats.

## Tabs Overview
- All: View and filter all questions.
- Quiz: Configure and take exams.
- Recent: Review past questions with filters.
- Help & Convert: Edit, highlight, and convert JSON.

## Taking an Exam
 1. Select categories in Quiz tab.
 2. Configure exam settings.
 3. Click Start Exam.
 4. Answer or skip questions.
 5. View results with score and timing.

## Accessibility
- Keyboard navigable tabs and controls.
- Screen reader friendly ARIA labels.
- Focus outlines and dynamic content updates.

## Technologies Used
- HTML5, CSS3 (Flexbox)
- Vanilla JavaScript
- LocalStorage for persistence
