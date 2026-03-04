# Goodreads Choice Awards 2025 — Web Scraping & Analysis

This project scrapes the [Goodreads Choice Awards 2025](https://www.goodreads.com/choiceawards/best-books-2025) to collect all nominated books across 15 genres and performs exploratory data analysis to uncover patterns in ratings, popularity, and book characteristics.

### Data Source
Source: Goodreads Choice Awards 2025
Data collected: November–December 2025 award cycle
Genres scraped (15):
Fiction, Historical Fiction, Mystery & Thriller, Romance, Romantasy, Fantasy, Science Fiction, Horror, Debut Novel, Audiobooks, YA Fantasy & Sci-Fi, YA Fiction, Nonfiction, Memoir, History & Biography

### Analysis
The analysis explores three interrelated questions:

#### 1. Which genre has the highest rated nominees on average?
Looks at the average Goodreads rating of all nominees across genres to identify which genres produce the most critically acclaimed books.

#### 2. Within the highest rated genres, do books with more ratings also have higher scores?
Examines the correlation between popularity (number of ratings) and quality (rating score) within the top 5 genres. Finds that some genres (romantasy) show a positive correlation while others (history/bio) show a negative one.

#### 3. Among books that are both highly rated and widely read, what do they have in common?
Defines "elite" books as those in the top 25% of both rating and number of ratings, and examines what these books share in terms of genre, page count, and format.

### Key Findings
- Audiobooks, memoirs, and history/biography nominees tend to have the highest average ratings
- In history/biography, more popular books tend to be rated lower — popularity does not reflect quality in this genre
- In romantasy, the opposite is true — popular books also tend to be highly rated
- Elite books (high rating + widely read) tend to come from audiobook and romantasy genres
- Elite books average more pages than non-elite books

### Libraries Used

| Library | Purpose |
|---------|---------|
| `playwright` | Headless browser scraping of JavaScript-rendered pages |
| `beautifulsoup4` | Parsing saved HTML files |
| `pandas` | Data manipulation and analysis |
| `numpy` | Numerical operations |
| `matplotlib` / `seaborn` | Data visualization |
| `requests` | HTTP requests |

## AI Use Statement

This project was built with the assistance of an AI coding assistant (Claude by Anthropic). The AI was used to help debug scraping issues (particularly async Playwright on Windows), suggest CSS selectors, write helper functions, and provide guidance on analysis approaches. All analysis decisions, interpretations, and written content were reviewed and directed by the student.

## Citations

- Goodreads. (2025). *Goodreads Choice Awards 2025*. https://www.goodreads.com/choiceawards/best-books-2025
- Playwright for Python. https://playwright.dev/python/
- Beautiful Soup Documentation. https://www.crummy.com/software/BeautifulSoup/bs4/doc/
- pandas Documentation. https://pandas.pydata.org/docs/
