# LOTW Lesson #A1-17: Prepositions & God's Laws

An interactive web-based English lesson focusing on prepositions of place and the biblical story of Moses receiving God's laws.

## Features

- **Interactive Bible Lesson**: Teaches the story of Moses and the Ten Commandments
- **Grammar Practice**: Focuses on prepositions of place (in, on, at, above, below, etc.)
- **Pronunciation Exercises**: Practice /L/ and /H/ sounds
- **Interactive Activities**:
  - Drag and drop preposition exercises
  - Multiple-choice quizzes
  - Vocabulary listening exercises
- **Editable Content**: Teachers can modify lesson content directly in the interface
- **Responsive Design**: Works on desktop and mobile devices

## Lesson Structure

1. **Pray, Review, and Preview**
2. **Bible Reading**: Moses Gives God's Laws
3. **Pronunciation and Grammar**
4. **Interactive Practice**: Where Is It?
5. **Drag and Drop Activity**
6. **Vocabulary Review and Conclusion**

## Technologies Used

- HTML5
- CSS3 (with CSS Variables for theming)
- JavaScript (Vanilla JS)
- Font Awesome for icons
- Responsive design with media queries

## How to Use

1. Clone this repository or download the HTML file
2. Open `index.html` in any modern web browser
3. Navigate through the 6-page lesson using the Next/Previous buttons
4. Complete interactive exercises
5. (For teachers) Use the Edit buttons to modify lesson content

## Teacher Features

- Edit any text content directly in the interface
- Upload custom images for lesson illustrations
- Replace audio files for pronunciation exercises
- Save all changes (currently logs to console - implement backend as needed)

## Code Example

The lesson uses a simple page navigation system:

```javascript
function navigateTo(pageNumber) {
    if (pageNumber < 1 || pageNumber > totalPages) return;
    const currentPageElement = document.getElementById(`page${currentPage}`);
    const nextPageElement = document.getElementById(`page${pageNumber}`);
    if (currentPageElement) currentPageElement.classList.remove('active');
    if (nextPageElement) nextPageElement.classList.add('active');
    currentPage = pageNumber;
    window.scrollTo(0, 0);
}
