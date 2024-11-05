# The Beluga's Magic Ocean Potion - Interactive Storybook

This project is an interactive digital storybook titled **"The Beluga's Magic Ocean Potion"** by **Elodie Harvey**, with illustrations generated using AI tools. The story was handwritten by Elodie and digitized using AI assistance. This README file explains the process of creating the book, including image generation, text digitization, and building the interactive web application.

---

## Table of Contents

- [The Beluga's Magic Ocean Potion - Interactive Storybook](#the-belugas-magic-ocean-potion---interactive-storybook)
  - [Table of Contents](#table-of-contents)
  - [This was the Original Story](#this-was-the-original-story)
  - [Link to the Book](#link-to-the-book)
  - [Overview](#overview)
  - [Project Structure](#project-structure)
  - [Process Overview](#process-overview)
    - [1. Image Generation](#1-image-generation)
    - [2. Text Digitization](#2-text-digitization)
    - [3. Building the Interactive Book](#3-building-the-interactive-book)
      - [**HTML Structure**](#html-structure)
      - [**CSS Styling**](#css-styling)
      - [**JavaScript Functionality**](#javascript-functionality)
  - [How to Run the Project](#how-to-run-the-project)
  - [Customization](#customization)
  - [Accessibility Considerations](#accessibility-considerations)
  - [Acknowledgments](#acknowledgments)

---

## This was the Original Story

![Handwritten Story](/Images/OriginalStory.jpg)

---

## Link to the Book

👉 **[Click here to view the interactive storybook online.](https://yourusername.github.io/BelugaMagicOceanPotion/)**

---

## Overview

"The Beluga's Magic Ocean Potion" is a children's story created by Elodie Harvey. This project transforms her handwritten story and illustrations into an interactive digital book that can be viewed in a web browser. The interactive book features:

- **Page-turning animations** that simulate a real book.
- **Responsive design** that adapts to various screen sizes, from desktops to mobile devices.
- **Accessibility features** for keyboard navigation and screen readers.

---

## Project Structure

- `index.html` - The main HTML file containing the structure of the interactive book.
- Inline `<style>` tags in `index.html` - Contains all CSS styles for the book.
- Inline `<script>` tags in `index.html` - Contains all JavaScript logic for interactivity.
- `Images/` - A directory containing all the images used in the book (e.g., cover, page illustrations).
- `README.md` - This README file explaining the project and its creation process.

---

## Process Overview

The creation of the interactive storybook involved several key steps:

### 1. Image Generation

The images for the book were created using AI image generation tools.

- **Conceptualization**: Identified key scenes and elements from the story that needed illustrations.
- **AI Generation**: Used an AI image generator (e.g., OpenAI's DALL·E) to create images based on descriptive prompts.
  - *Example Prompts*:
    - "A magical ocean scene with a beluga whale."
    - "A fish jumping out of the water."
- **Selection and Refinement**:
  - Generated multiple images per scene to choose the best fit.
  - Performed minimal editing if necessary (cropping, resizing) to ensure consistency.

### 2. Text Digitization

The handwritten text from Elodie's story was converted into digital format.

- **Scanning**: Scanned or photographed the handwritten pages to create clear images of the text.
- **AI Text Recognition**:
  - Used **Claude AI** to process the images and convert the handwritten text into digital text.
  - Ensured that the AI accurately captured the nuances of the handwriting.
- **Editing and Formatting**:
  - Reviewed the digitized text for any errors or misinterpretations.
  - Formatted the text for inclusion in the HTML structure.

### 3. Building the Interactive Book

The interactive book was built using standard web technologies: HTML, CSS, and JavaScript.

#### **HTML Structure**

- **Book Container**: A `<div>` with the class `book-container` serves as the main wrapper.
- **Pages**:
  - Each page is a `<div>` with the class `page`.
  - Pages are structured with front and back content (`.page-front`, `.page-back`).
- **Content**:
  - Text and images are placed within the appropriate page divs.
  - ARIA labels and roles are used to enhance accessibility.

#### **CSS Styling**

- **Reset and Base Styles**: Applied basic resets to remove default margins, padding, and set box-sizing.
- **Layout**:
  - Used flexbox to center the book on the page.
  - Set responsive dimensions using `vw` (viewport width) and `vh` (viewport height) units.
- **Page Styling**:
  - Styled pages to resemble real book pages with shadows and borders.
  - Implemented a spine for the book using CSS transformations.
- **Animations**:
  - Used CSS transitions and transforms for smooth page-turning animations.
  - Created media queries to adjust styles for different screen sizes.
- **Accessibility Styles**:
  - Included focus outlines and other visual cues for keyboard navigation.

#### **JavaScript Functionality**

- **Initialization**:
  - On document load, initialized the book by setting up page order and initial states.
- **Page Turning Logic**:
  - Managed the current page index and controlled the turning of pages forward and backward.
  - Added event listeners for click, touch, and keyboard events.
- **Event Handling**:
  - **Click Events**: Turned pages when users clicked on the turn areas.
  - **Touch Events**: Enabled swipe gestures for touch devices.
  - **Keyboard Events**: Allowed navigation using arrow keys, Page Up/Down, Home, and End keys.
- **Accessibility Features**:
  - Implemented ARIA live regions to announce page changes.
  - Ensured that interactive elements are focusable and have appropriate labels.

---

## How to Run the Project

To view and interact with the storybook:

1. **Download the Project**:
   - Clone the repository or download the project files to your local machine.

2. **Prepare the Images**:
   - Ensure that all image files are placed in the `Images/` directory.
   - Images should be named according to their references in `index.html` (e.g., `Cover.jpg`, `pageOne.jpg`, etc.).

3. **Open the HTML File**:
   - Navigate to the project directory.
   - Open `index.html` in a modern web browser (Chrome, Firefox, Safari, Edge).

4. **Interact with the Book**:
   - Click on the right side of the book to turn pages forward.
   - Click on the left side to turn pages backward.
   - On touch devices, swipe left or right to navigate.
   - Use keyboard arrows for navigation:
     - Right Arrow or Page Down to go forward.
     - Left Arrow or Page Up to go backward.
     - Home to go to the beginning.
     - End to go to the last page.

---

## Customization

You can customize the storybook to create your own interactive stories.

- **Update Content**:
  - **Text**: Modify the story text within the HTML structure.
  - **Images**: Replace image sources with your own images. Ensure they are correctly referenced in the HTML.

- **Style Adjustments**:
  - Modify the `<style>` section in `index.html` to change fonts, colors, sizes, and layouts.
  - Adjust media queries to fine-tune responsiveness for different devices.

- **Functional Changes**:
  - Update the JavaScript logic in the `<script>` section to alter interactivity.
  - Add new features such as audio narration, background music, or interactive elements within pages.

---

## Accessibility Considerations

This project includes several features to enhance accessibility:

- **Semantic HTML**: Used appropriate HTML elements and attributes for better screen reader support.
- **Keyboard Navigation**: Users can navigate the book using standard keyboard keys.
- **Focus Management**: Interactive elements are focusable and have appropriate labels.
- **ARIA Labels**: Added ARIA attributes to provide additional context to assistive technologies.
- **Live Regions**: Implemented ARIA live regions to announce page changes.

---

## Acknowledgments

- **Elodie Harvey**: For creating the original story "The Beluga's Magic Ocean Potion."
- **DALL·E AI**: For generating the images used in the book.
- **Claude AI**: For converting handwritten text into digital format.
- **OpenAI's ChatGPT**: For assisting with code generation and problem-solving.

---

*Thank you for exploring "The Beluga's Magic Ocean Potion" interactive storybook. We hope you enjoy reading it as much as we enjoyed creating it!*
