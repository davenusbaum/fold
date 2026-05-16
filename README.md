# Fold
Functional PHP Framework, no magic

Fold is a small PHP framework built around plain functions, immutable data, and pipelines. 
There is no service container. 
There are no facades. 
There is no autowiring, no model events, no global helpers pretending to be language features. 
When you read Fold code, what you see is what runs.
It is unopinionated about how you build your app, and opinionated about how it gets out of your way.

## Why
Modern PHP is a good language.
Typed properties, enums, readonly, first-class callable syntax, arrow functions, match expressions — the pieces for writing clean, 
functional-leaning code are all there. 
Most PHP frameworks ignore them and keep grafting features onto an OOP service-container worldview from 2011.
Fold treats those features as the point. 
Routes are functions. 
Middleware is functions. 
Handlers compose. 
State is explicit. 
The framework hands you primitives and gets out of the way.
If you’ve built and operated a real PHP application for more than a few years and found yourself slowly pulling logic out of your framework 
instead of leaning into it, Fold is for you. 
If you love Laravel, Fold is not for you, and that’s fine.

## What’s in the box
	•	Routing. Map HTTP methods and paths to handler functions.
	•	Request and response. Plain value objects. No statics, no globals.
	•	Middleware. A pipeline of functions wrapping your handler. Compose them however you like.
	•	Database. A thin layer over PDO (or MySQLi) for querying. No ORM. No magic columns. You write the SQL.
	•	That’s it. No CLI scaffolding, no auth provider, no queue abstraction, no cache facade. Use real libraries for those, or write the small amount of glue you need.
