# Word Space ✦

A small, single-file web app for learning English vocabulary with Arabic translations. You see an English word, try to remember its Arabic meaning, and reveal hints step by step.

## Quick Start

1. Save the page as `index.html`.
2. Double-click the file to open it in any modern browser (Chrome, Firefox, Edge, Safari).
3. That's it. No installation, build step, or server is needed.

> An internet connection is only needed to load the hint images (they come from Unsplash by default).

## How to Use

### Play

1. On the home screen, click **START ✦**.
2. A random English word is shown. Try to recall its Arabic meaning.
3. Click the hint button:
   - **💡 Hint 1** shows an image related to the word.
   - **🌐 Hint 2** reveals the Arabic translation.
4. Click **Next Word →** for another random word (the same word never appears twice in a row).
5. Click **Home** to go back to the main screen.

### Add Your Own Words

1. On the home screen, click **+ Add Word**.
2. Fill in the form:
   - **English word** (required)
   - **Arabic translation** (required)
   - **Image URL** (optional): a direct link to an image, used as Hint 1
3. Click **Save Word**. A confirmation message appears when it is saved.
4. Click **Cancel** to return home. Your new word will appear in the game and in the floating background.

Notes:
- Duplicate English words are rejected ("This word already exists!").
- If no image URL is given, Hint 1 shows "No image available" and you can move on to Hint 2.
- If an image link is broken, the app tells you the image is unavailable.

## Features

- Random word practice with no immediate repeats
- Two-step hint system (image, then translation)
- Add custom words with optional images
- Words saved automatically in your browser
- Word counter in the header
- Animated floating-words space background
- Responsive layout for desktop and mobile

## Where Your Words Are Stored

Custom words are saved in your browser's `localStorage` under the key `wordSpaceWords`.

- They stay after closing or refreshing the page.
- They are tied to **one browser on one device**. Another browser or device will not see them.
- Clearing your browser data, or using private/incognito mode, will remove them.

## Customizing

To change the built-in words, edit the `defaultWords` array in the `<script>` section:

```js
{
  word: "Apple",
  translation: "تفاحة",
  image: "https://example.com/apple.jpg"
}
```

To change the look, edit the CSS at the top of the file (colors, fonts, card size, etc.).

## Project Structure

```
index.html   # HTML, CSS, and JavaScript all in one file
README.md    # This file
```

## Tech Stack

- HTML5
- CSS3 (gradients, animations, glassmorphism card)
- Vanilla JavaScript (no frameworks or dependencies)

## Troubleshooting

| Problem | Solution |
|---|---|
| Images don't show | Check your internet connection, or verify the image URL is a direct link to an image |
| Added words disappear | Browser storage may be disabled or cleared (private mode, cleanup tools) |
| "Please add some words first" | The word list is empty; add at least one word |

Enjoy exploring the universe of words! 🚀
