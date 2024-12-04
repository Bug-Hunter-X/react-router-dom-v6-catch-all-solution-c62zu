# React Router Dom v6 Catch All Route Issue

This repository demonstrates a common issue encountered when using the catch-all route (`/*`) in React Router Dom v6. The catch-all route is intended to handle any unmatched routes, but in certain situations it may not function as expected, leading to unexpected behavior or errors.

## Issue Description

The problem lies in the order of routes. When a catch all route (`/*`) is placed before more specific routes, it will always match first, preventing other routes from being evaluated. This means that even if a route matches a specific path, the catch-all route will always take precedence.

## Solution

To resolve this issue, always place the catch-all route at the end of your route definitions. This ensures that all more specific routes are checked before the catch-all route is considered.  Additionally, ensure that your paths are correctly defined and avoid conflicts.

## Setup

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` to install the dependencies.
4. Run `npm start` to start the development server.
