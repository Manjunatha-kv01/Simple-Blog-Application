# Simple-Blog-Application
This project provides a solid foundation r to understand core Laravel concepts and build a functional web application with an API.

Why this works (as per your request):

**Laravel (MVC, Eloquent ORM):**
MVC: We've separated concerns into Models (Post, User), Views (Blade files), and Controllers (PostController, Api/PostController).
Eloquent ORM: We've used Eloquent for database interactions (Post::create(), Post::find(), $user->posts(), relationships belongsTo, hasMany).

**MySQL**: Data is stored in a MySQL database, configured via .env and managed with migrations.

**RESTful APIs:**
routes/api.php defines API endpoints (/api/posts, /api/posts/{id}).
Api/PostController handles API requests, returning JSON responses (using PostResource for consistent formatting).
Standard HTTP verbs (GET, POST, PUT, DELETE) are used for corresponding actions.

**CRUD Operations:**
Create: store() methods in controllers.
Read: index() and show() methods.
Update: update() methods.
Delete: destroy() methods.
Implemented for both web interface and API.

**User Authentication:**
Laravel Breeze for web authentication (session-based).
Laravel Sanctum for API authentication (token-based).

**Simple Error Handling:**
Leveraged Laravel's built-in validation and exception handling.
Provided examples of custom JSON error responses for APIs.
Showed how to customize web error pages.
