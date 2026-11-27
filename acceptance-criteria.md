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

# Acceptance Criteria

### Feature: Featured Books Showcase
US1:
- AC1.1: Given the user opens the Homepage (index.html), when the page finishes loading, then a "Featured Books" section displays recommended books with each book's cover image, title, and category.
- AC1.2: Given the user is viewing the Featured Books section, when the user selects any featured book, then that book's details view opens with its information.
- AC1.3: Given the user is on the Homepage, when the user selects a navigation link ("Home", "Book Library", or "My Bookshelf"), then the corresponding page opens.
- AC1.4: Given the user views the Homepage on a desktop screen or a 375px-wide mobile screen, when the page loads and is scrolled, then all text, images, and navigation links fit within the screen width without horizontal scrolling.



### Feature: Book Library
US2:
- AC2.1: Given the user opens the Book Library (app.html), when the page finishes loading, then all available books display with each book's cover image, title, and category.
- AC2.2: Given the user is on the Book Library page, when the user selects a category filter ("Fiction", "Fantasy", "Romance", "Mystery", "Horror", "Education", "Technology", or "Self-Development"), then only books in that category remain visible.
- AC2.3: Given the user enters text into the search bar on the Book Library page, when the search runs, then only books whose titles contain the search text (ignoring uppercase/lowercase differences) remain visible.
- AC2.4: Given the user selects both a category filter and a search term, when both filters are active, then only books matching both the selected category and the search term remain visible.


### Feature: View Book Details and Quick Summaries
US3:
- AC3.1: Given the user selects a book from the Featured Books section or the Book Library, when the details view opens, then it displays the book's cover image, title, author, category, publication year, and summary.
- AC3.2: Given the book details view is open, when the user selects the "Close" control, then the details view closes and returns to the previous book list.
- AC3.3: Given a selected book has no summary text, when its details view opens, then "No summary available for this title" displays in place of the summary.

### Feature: "My Bookshelf"
US4:
- AC4.1: Given a book's details view is open, when the user selects "Want to Read", "Currently Reading", or "Finished", then the book is added to that reading status on My Bookshelf (bookshelf.html) and a confirmation message appears.
- AC4.2: Given a book is already saved on My Bookshelf, when the user selects a different reading status for that book, then the book moves to the newly selected status and is removed from its previous status without creating duplicates.
- AC4.3: Given the user opens My Bookshelf (bookshelf.html), when the user selects "Want to Read", "Currently Reading", or "Finished", then only books assigned to that status display.
- AC4.4: Given no books are saved under the selected reading status (or the bookshelf is empty), when My Bookshelf displays that section, then "Your bookshelf is currently empty" appears alongside a link to the Book Library (app.html).



(Temporary)
### Feature: Featured Books 
US1: As a reader, I want to explore featured books on the website, so that I can conveniently discover books recommended by popularity. 
- AC1.1: Featured Books section displays selected popular books in the interface in every category. 
- AC1.2: Each featured book displays the book cover, title and author. 
- AC1.3: Featured Books layout and interactive buttons remain accessible and responsive across different screen sizes. 

US2:

US3:

### Feature: Book Library 
US2: As a reader, I want to browse books by category, so that I can easily find books matching my interests in one place without visiting multiple websites. 
- AC2.1: Filter must show categories such as romance, fantasy, mystery, technology, education, personal growth, fiction, and self-development. 
- AC2.2: Selecting a category displays matching books from that category, and search or selection is not case sensitive.
- AC2.3: Book covers and titles must be displayed for each book in the selected category

US2:

US3:

### Feature: View Book Details and Quick Summaries
US3: As a reader, I want to view detailed information about a selected book so that I can understand its content and learn more about the book before deciding to read it.
- AC3.1: Clicking a book shows the details such as cover, title, author, description, and published date.
- AC3.2: The book details shows ongoing and finished status.
- AC3.3: A short summary of the book of what is the book all about.

US2:

US3:

### Feature: My Bookshelf 
US4: As a reader, I want to organize books into different reading status sections, so that I can keep my book exploration organized in a single platform. 
- AC4.1: My Bookshelf displays separate sections for All, Continue Reading, What to Read, and Finished.
- AC4.2: Clicking a reading status control filters or displays books under that status. 
- AC4.3: Empty reading status sections display a clear empty state that no books have been added.

US2:

US3:
