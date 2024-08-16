# Movie Listing API

This FastAPI Movie Listing API allows users to list, view, rate, and comment on movies. It uses JWT for secure access, ensuring only the original user can modify or delete their listings. The application is deployed on a cloud platform for public access.

# Features

## User Authentication:
### User Registration: 
- Users can register by providing a username and password.
### User Login: 
- Registered users can log in to receive a JWT token.
- JWT Token Generation: After logging in, users receive a JWT token for authentication.
### Movie Listing:
- View a Movie: Anyone can view details of a listed movie.
### Add a Movie: 
- Authenticated users can add new movies.
### View All Movies: 
- Anyone can view the list of all movies.
### Edit a Movie: 
- Only the user who listed the movie can edit its details.
### Delete a Movie: 
- Only the user who listed the movie can delete it.
## Movie Rating:
### Rate a Movie: 
- Authenticated users can rate movies.
### Get Ratings for a Movie: 
- Anyone can view ratings for a movie.
## Comments:
### Add a Comment: 
- Authenticated users can add comments to movies.
### View Comments: 
- Anyone can view comments for a movie.
### Add Nested Comments: 
- Authenticated users can reply to existing comments, creating nested comments.


### Deployment: 
- Render 

## Technologies Used
### Language & Framework: 
- Python with FastAPI
### Database: 
- SQLAlchemy ORM with support for SQL databases
### Authentication: 
- JWT for securing endpoints
### Testing: 
- Unit tests for API endpoints using pytest
### Documentation: 
- OpenAPI/Swagger for API documentation
### Logging: 
- Integrated logging for important application details using PaperTrail logging



## Setup and Installation
#### Prerequisites
- Python 3.7+
- An SQL database (PostgreSQL, MySQL, SQLite, etc.)
- Git (for version control)

## Security
- JWT tokens secure the endpoints.
- Only authenticated users can add, edit, or delete movies and comments.
- In production, use a strong, unique SECRET_KEY.

## Installation Process
1. Clone the Repository:
``` bash
git clone https://github.com/yourusername/movie_listing_api.git
```

``` bash
cd movie_listing_api
```
2. Create and Activate a Virtual Environment:
``` bash
python -m venv environment_name
source environment_name/bin/activate 
```
3. Install Dependencies:
``` bash
pip install -r requirements.txt
```
4. Set Up Database:
``` bash
alembic upgrade head
```
5. Run the Application:
``` bash
uvicorn app.main:app --reload
```
6. Access the API Documentation:
- Visit `http://127.0.0.1:8000/docs` to explore the API with Swagger UI.

### Running Tests
To run unit tests, use the following command:
```bash
pytest
```
### Contribution
If you'd like to contribute to this project, please fork the repository and use a feature branch. Pull requests are welcome.

### Support
For any inquiries or support, reach me on ejirosamuelolori@gmail.com
