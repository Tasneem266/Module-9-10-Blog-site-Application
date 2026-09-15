# Blog Application

A Django based blog application built and updated with a bit advanced features, under a single project.

## Features

### Module 9 Features
- User registration, login, and logout
- Create, read, update, and delete blog posts
- Ownership restrictions (only the author can edit or delete their own posts)
- User profile display
- Django template inheritance
- Django messages

### Module 10 Features
- Comment system on blog posts
- Nested comment replies
- Like and unlike posts
- Like and unlike comments
- Post rating system (1 to 5 stars)
- Average rating display
- Aggregation and annotation (Count, Avg) using Django ORM
- Popular posts based on likes and comments
- Search posts by title, content, or author
- Filter posts by category
- Profile statistics (posts, comments, likes given, ratings given)
- Django Admin for all models
- Query optimization with `select_related()` and `prefetch_related()`

## Tech Stack

- Python
- Django 6.1.1
- SQLite
- HTML5
- Custom CSS (no Bootstrap, no Tailwind)


## Installation
 Clone the repository

## Project Structure

See `project_structure.txt` for the complete folder layout.

## Usage

1. Register a new account.
2. Log in.
3. Create blog posts.
4. View, like, rate, and comment on posts.
5. Reply to comments.
6. Edit or delete your own posts and comments.
7. View your profile statistics.
8. Use search and category filters.

## Django ORM Usage

- `annotate(Count('likes', distinct=True))` for like counts
- `annotate(Count('comments', distinct=True))` for comment counts
- `annotate(Avg('ratings__rating'))` for average ratings
- `select_related('author', 'category')` for foreign key optimization
- `prefetch_related('replies')` for reverse foreign key optimization
- `Q()` objects for combined search lookups
- `update_or_create()` for preventing duplicate ratings


## License
This project is for educational purposes.
