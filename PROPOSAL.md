
# RecipeHub – Recipe Discovery and Sharing Platform

## 1. Project Overview

**Project Name:** RecipeHub

**Project Type:** Full-Stack Web Application

### Project Pitch

RecipeHub is a web application where users can discover, explore, and share recipes. The platform allows users to browse different recipes, search for cooking ideas, and filter recipes by category.

Each recipe provides detailed information, including ingredients, preparation instructions, cooking time, difficulty level, and category.

Users can also contribute to the platform by submitting their own recipes, editing or deleting recipes, and sharing their opinions through ratings and reviews.

The main goal of RecipeHub is to create a simple and accessible platform that brings recipe discovery and sharing together in one place.

**Target Users:**
- People who enjoy cooking.
- Beginners looking for simple recipes.
- People who want to discover new dishes.
- People who want to share their own recipes.

The application will not require user authentication. Users can submit recipes and reviews by providing basic information such as their name.

## 2. Main Features

The application will provide the following features:

- Browse all available recipes.
- Search recipes by name.
- Filter recipes by category.
- View detailed recipe information.
- Add new recipes.
- Edit existing recipes.
- Delete recipes.
- Submit ratings and reviews.
- View reviews submitted by other users.

## 3. Pages and Routes

| Route | Description | Rendering Strategy |
|---|---|---|
| `/` | Homepage displaying featured recipes and an introduction to RecipeHub. | Static |
| `/recipes` | Displays all available recipes with search and category filters. | Dynamic |
| `/recipes/[id]` | Displays the details of a specific recipe, including ingredients, instructions and reviews. | Dynamic |
| `/recipes/new` | Form for submitting a new recipe. | Dynamic |
| `/categories/[id]` | Displays recipes belonging to a selected category. | Dynamic |
| `/recipes/[id]/reviews` | Displays reviews and provides a form to submit a new review. | Dynamic |

### Rendering Strategy Explanation

- **Static rendering:** The homepage contains general information and can be generated in advance.
- **Dynamic rendering:** Recipe listings, recipe details and category pages depend on database content that can change when users add, edit or delete recipes.
- Dynamic routes such as `/recipes/[id]` allow the application to display different recipes using their unique IDs.

Public recipe pages will be designed to support search engine optimization (SEO).

## 4. Database Entities

The application will use three main entities.

### Recipe

| Field | Type |
|---|---|
| id | Integer |
| title | String |
| description | String |
| ingredients | Text |
| instructions | Text |
| cookingTime | Integer |
| difficulty | String |
| imageUrl | String |
| categoryId | Integer |

### Category

| Field | Type |
|---|---|
| id | Integer |
| name | String |
| description | String |

### Review

| Field | Type |
|---|---|
| id | Integer |
| recipeId | Integer |
| reviewerName | String |
| rating | Integer |
| comment | String |
| createdAt | DateTime |

## 5. Entity Relationships

The application will have the following relationships:

- One Category can contain multiple Recipes.
- Each Recipe belongs to one Category.
- One Recipe can have multiple Reviews.
- Each Review belongs to one Recipe.

These relationships will be implemented using Prisma and a relational database.

## 6. Write Actions

The application will support the following operations:

### Recipe Management
- Create a new recipe.
- Read and display recipes.
- Update existing recipe information.
- Delete a recipe.

### Review Management
- Submit a review for a recipe.
- Read and display reviews.
- Delete a review.

### Category Management
- Organize recipes into categories.
- Filter recipes by category.

These operations will demonstrate Create, Read, Update and Delete (CRUD) functionality.

## 7. Technical Implementation

The project will use the following technologies:

| Technology | Purpose |
|---|---|
| Next.js | Application framework and routing |
| React | User interface and interactive components |
| TypeScript | Type safety |
| Tailwind CSS | Styling and responsive design |
| Next.js API Routes | Backend API endpoints |
| Prisma | Database access and ORM |
| PostgreSQL | Relational database |
| Git and GitHub | Version control and project collaboration |
| Vercel | Application deployment |

## 8. Project Scope and Limitations

The project will focus on recipe discovery, recipe management and user reviews.

The following features are outside the initial project scope:

- User registration and authentication.
- Social networking and messaging.
- Online payments.
- Advanced recommendation systems.

The application will be developed incrementally, starting with the Next.js frontend and routing, followed by API development, database integration and deployment.

## 9. Expected Outcome

The expected outcome is a functional full-stack web application where users can discover recipes, manage recipe content and submit reviews.

The project will demonstrate the practical application of Next.js, server-side rendering, dynamic routing, API development, database relationships, Prisma and CRUD operations.

## 10. GitHub Repository

**GitHub Repository:** To be added after creating the repository.
