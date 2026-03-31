# Next Books CRUD

A small CRUD app built with Next.js App Router to practice connecting API routes to a UI.

## What it does

- Lists books on the `/books` page
- Adds a new book through a client form
- Updates and deletes existing books
- Fetches the book list in a Server Component
- Handles form actions and mutations in Client Components

## Tech Stack

- Next.js 14+ App Router
- TypeScript
- Tailwind CSS
- Route Handlers (`app/api/...`)

## Project Structure

```bash
├── app
│   ├── api
│   │   └── books
│   │       ├── route.ts         # GET all books, POST new book
│   │       └── [id]
│   │           └── route.ts     # PUT/PATCH and DELETE by id
│   └── books
│       └── page.tsx             # Server Component for fetching and rendering books
├── components
│   ├── BookForm.tsx             # Client form for create/update
│   └── BookItem.tsx             # Client component for each book row and actions
```

## Running Locally

```
npm install
npm run dev
```

## Why this project

This project was built to understand:

- Server vs Client Components
- Route Handlers in Next.js
- Basic CRUD flow in the App Router
- Connecting UI actions to API endpoints
