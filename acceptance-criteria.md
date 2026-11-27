# Acceptance Criteria — BookVerse

## Feature: Featured Books Showcase

### US1.1: View Featured Books on Homepage
- AC1.1.1: Given the user opens the Homepage, when the page finishes loading, then a "Featured Books" section shows recommended books, with each book's cover, title, and category.
- AC1.1.2: Given no books are marked as featured, when the Homepage finishes loading, then a message shows in place of the featured book cards.

### US1.2: Select a Featured Book
- AC1.2.1: Given the user is looking at the Featured Books section on the Homepage, when the user clicks any featured book card, then the book details view opens for that book.

### US1.3: Responsive Navigation Across Pages
- AC1.3.1: Given the user is on the Homepage, when the user clicks a navigation link ("Home", "Book Library", or "My Bookshelf"), then the matching page opens.
- AC1.3.2: Given the user views the Homepage on a computer screen or a 375px-wide phone screen, when the page loads and scrolls up and down, then all text, cover images, and navigation links fit inside the screen width without sideways scrolling.

---

## Feature: Book Library

### US2.1: Browse Complete Book Catalog
- AC2.1.1: Given the user opens the Book Library page, when the page finishes loading, then all available books show in a grid, with each book's cover, title, and category.

### US2.2: Filter Books by Category
- AC2.2.1: Given the user is on the Book Library page, when the user picks a category filter ("Fiction", "Fantasy", "Romance", "Mystery", "Horror", "Education", "Technology", or "Self-Development"), then only books in that category stay visible.
- AC2.2.2: Given a category filter is active on the Book Library page, when the user sets the filter back to "All", then all available books show again.

### US2.3: Search Books by Title
- AC2.3.1: Given the user types words into the title search bar on the Book Library page, when the search runs, then only books whose titles have those words (ignoring uppercase and lowercase letters) stay visible.
- AC2.3.2: Given both a category filter and a title search are active on the Book Library page, when the filters run, then only books that match both the chosen category and the searched words stay visible.
- AC2.3.3: Given a title search or category filter matches zero books, when the search runs, then a "No matching books found" message shows instead of an empty grid.

---

## Feature: Book Details

### US3.1: View Book Metadata and Summary
- AC3.1.1: Given the book details view opens for a selected book, when the view loads, then it shows the book's cover, title, author, category, publication year, and summary.
- AC3.1.2: Given a selected book has no summary text, when its details view opens, then `"No summary available for this title"` shows in place of the summary.

### US3.2: Close Book Details View
- AC3.2.1: Given the book details view is open, when the user clicks the "Close" button, then the details view closes and returns the user to the book list.

---

## Feature: My Bookshelf

### US4.1: Save a Book to a Reading Status
- AC4.1.1: Given a book's details view is open, when the user clicks "Want to Read", "Currently Reading", or "Finished", then the book is saved to My Bookshelf under that status and a confirmation message shows.

### US4.2: View Saved Books by Reading Status
- AC4.2.1: Given the user opens My Bookshelf, when the user clicks "Want to Read", "Currently Reading", or "Finished", then only books saved under that reading status show.
- AC4.2.2: Given zero books are saved under the chosen reading status (or the bookshelf is empty), when My Bookshelf shows that section, then `"Your bookshelf is currently empty"` shows along with a clickable link to the Book Library.

### US4.3: Update a Saved Book's Reading Status
- AC4.3.1: Given a book is already saved on My Bookshelf, when the user picks a different reading status for that book, then the book moves to the new status and is removed from its old status without making duplicates.

### US4.4: Remove a Book from My Bookshelf
- AC4.4.1: Given a book is shown on My Bookshelf, when the user clicks the "Remove" button for that book, then the book is deleted from My Bookshelf and disappears from the list right away.