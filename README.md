# React Router v6 Catch-all Route Issue

This repository demonstrates a problem with the catch-all route ('/*') in React Router v6.  Other routes are working correctly, but the catch-all route fails to render when an unmatched route is accessed.

## Problem Description

The issue arises when using a catch-all route in conjunction with other, more specific routes. While the other routes function as intended, the catch-all route does not handle unmatched paths.  This causes unexpected behavior and prevents the display of a 'Not Found' page or similar error handling component.

## Solution

The solution involves ensuring the catch-all route is placed at the end of the route definitions within the `Routes` component. This ensures that React Router correctly evaluates the paths and uses the catch-all route only when no other matches are found.