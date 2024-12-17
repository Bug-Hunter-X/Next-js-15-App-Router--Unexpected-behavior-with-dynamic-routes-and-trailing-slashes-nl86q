# Next.js 15 App Router: Unexpected behavior with dynamic routes and trailing slashes

This repository demonstrates an unexpected behavior in the Next.js 15 App Router when dealing with dynamic routes and trailing slashes.  The issue arises when navigating to a route with a trailing slash that doesn't have a corresponding page file.  Instead of returning a 404, it sometimes displays the content of a different page.

## Steps to Reproduce

1. Clone the repository.
2. Install dependencies: `npm install`
3. Run the development server: `npm run dev`
4. Navigate to `/blog` (should correctly show blog page)
5. Navigate to `/blog/` (unexpected behavior: should return 404, but may show blog page instead)

## Expected Behavior

A 404 error should be returned when accessing a route with a trailing slash that doesn't have a corresponding file.