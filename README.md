# PurgeCSS removes essential Tailwind CSS styles

This repository demonstrates an uncommon bug where PurgeCSS, used with Tailwind CSS, removes essential styles despite seemingly correct configuration.  The issue focuses on the loss of styles specifically related to responsive design variations or dynamically added classes.  The `bug.js` file shows the problematic code, and `bugSolution.js` provides a potential solution.

## Problem

The problem lies in how PurgeCSS interacts with certain classes or responsive modifiers that might not be directly referenced in the initial HTML but are generated dynamically or depend on responsive breakpoints.  Despite having the correct PurgeCSS configuration and Tailwind directives, these styles are being purged.

## Solution

The solution often involves carefully reviewing the PurgeCSS configuration to ensure it correctly handles dynamic class generation and responsive utilities.  It might involve adding more explicit patterns or using a different approach to handle the responsive variations.

## Setup

This repo requires Node.js and npm (or yarn) to be installed. You can run `npm install` or `yarn` to install the dependencies.
