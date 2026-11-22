# Space quiz

- The entire application is in `index.html`: markup, styles, question data, and quiz logic. Open the file directly in a browser; no server or dependencies are required.
- `questions` holds each question's answers, correct answer index, and feedback fact. The script tracks the current question, score, and whether it has been answered. `renderQuestion`, `selectAnswer`, and `updateProgress` coordinate the quiz UI; the Next and Play again handlers manage results and reset.
- Answer buttons are generated from the question data. Selecting an answer disables all choices, reveals the correct answer and explanatory feedback, updates the score and progress, and enables navigation to the next question.
- Preserve keyboard focus management, semantic buttons, the live feedback status, and progress-bar ARIA values when changing the flow. Styles support light and dark color schemes and reduced motion.
- If changing the number of questions, keep the static score denominator and progress bar's `aria-valuemax` consistent with the question data.
