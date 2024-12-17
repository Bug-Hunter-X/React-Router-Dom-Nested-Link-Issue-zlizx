# React Router Dom Nested Link Issue

This repository demonstrates a common, yet easily missed, issue when using nested links within React Router Dom.  The problem arises when a link is placed inside a component which is already routed, and the path is not properly specified.  The example shows a relative path causing unexpected behavior.

## Problem

The core issue is that in a nested route, a relative path (e.g., `to="/home"`) may not work as expected.  A misunderstanding of how relative paths are resolved in the context of nested routes often leads to the bug.

## Solution

Ensure that you use absolute paths (`to="/home"`) for all links in your application, especially in nested routes.  This avoids issues related to relative path resolution within React Router Dom.