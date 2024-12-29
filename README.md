# React Router v6 Nested Route Bug

This repository demonstrates a bug encountered when using nested routes with parameters in React Router v6.  The issue specifically arises when attempting to render a component based on a wildcard path segment ('*').

## Problem

The provided `App.js` demonstrates the scenario. The `Contact` component is only rendered when navigating directly to `/contact`, it does not render when attempting to navigate to a path like `/contact/something`.  The expected behavior is for `Contact` to render regardless of the path after `/contact`.

## Solution

The solution is provided in `bugSolution.js`. This fixes the bug by ensuring the wildcard route handles all paths that begin with '/contact' correctly.

## Setup

1. Clone this repository.
2. Navigate to the directory.
3. Run `npm install` to install the dependencies.
4. Run `npm start` to start the development server.