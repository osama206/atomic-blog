# The Atomic Blog

The Atomic Blog is a simple blogging platform built with React. It demonstrates various React concepts and techniques, including state management, context API, memoization, and performance optimization.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Components](#components)
- [Context Management](#context-management)
- [Utility Functions](#utility-functions)
- [Performance Considerations](#performance-considerations)
- [Credits](#credits)

## Features

- Create and display blog posts
- Search for posts by title and body
- Toggle dark mode
- Archive and restore posts
- Clear all posts

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/osama206/atomic-blog.git
   cd atomic-blog
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm start
   ```

## Usage

1. Use the form at the top of the page to add a new post by entering a title and body.
2. Use the search bar to filter posts based on the title and body content.
3. Toggle dark mode using the moon/sun button.
4. View archived posts by clicking "Show archive posts" and add them back to the main list.
5. Clear all posts by clicking the "Clear posts" button.

## Components

### App

The main component that sets up the application's structure and provides context to its child components.

### Header

Contains the title, search input, post count, and a button to clear posts.

### Main

Contains the form to add new posts and displays the list of posts.

### Archive

Displays a list of archived posts and allows adding them to the main list.

### Footer

Displays the footer of the application.

### FormAddPost

Form to add new posts with inputs for the title and body.

### List

Displays a list of posts.

### SearchPosts

Input field to search posts by title and body.

### Results

Displays the count of posts found based on the search query.

## Context Management

### PostContext

Context created using React's `createContext` to manage and share state across the application.

### PostProvider

Wraps the application components and provides context values like posts, search query, and handlers for adding and clearing posts.

### usePosts

Custom hook to access context values in child components.

## Utility Functions

### createRandomPost

Generates random posts using the `faker` library.

## Performance Considerations

### useMemo and memo

- `useMemo` is used in `PostProvider` to memoize the context value to avoid unnecessary recalculations.
- `memo` is used in the `Main` component to prevent unnecessary re-renders when the props do not change.

### SlowComponent and Counter

Demonstrates how performance issues can arise with slow components and how to manage them using memoization and optimization techniques.

## Credits

- [React](https://react.dev/)
- [Faker.js](https://github.com/faker-js/faker) for generating random post content

---
