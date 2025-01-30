# React Router Dom v6 Catch All Route Not Working
This repository demonstrates a common issue encountered when using catch-all routes (*) in React Router Dom v6.  The catch-all route, intended to handle any unmatched URL, fails to function correctly, resulting in unexpected behavior.

## Problem Description
The provided example uses the standard structure for a catch-all route (`/*`). Despite this, URLs not explicitly defined still result in a routing failure.

## Solution
The solution involves ensuring that the catch-all route is placed *last* within the `Routes` component.  This ensures that it only matches if no other routes are matched.