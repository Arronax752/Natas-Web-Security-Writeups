# Natas 0 — Writeup

## Objective

Find the password for **Natas 1**.

## What We Have

* Username: `natas0`
* URL : `http://natas0.natas.labs.overthewire.org`
* Password : `natas0`

## What We Need

The password for **Natas 1**.

## Initial Investigation

Open the Natas 0 webpage.

The page looks normal, but the password is not visible.

Right-click the page → **View Page Source**

Or press:

```text
Ctrl + U
```

## Why Do This?

The browser receives the webpage as HTML.

Something that isn't visible on the page can still be present inside the HTML source.

So, checking the source is a basic web reconnaissance step.

## Solution

Search through the HTML source.

The password is hidden inside an **HTML comment**. `scfWG6qNEIdzqVyfRwEGXyNUfFZkZeQ7`

Copy the password and use it to log in to **Natas 1**.

## Concepts

* HTML source code
* HTML comments
* Basic web reconnaissance
* Hidden information in webpage source

## Tools Used

```text
Browser
View Page Source
Ctrl + U
```

## Lesson

**Hidden from the webpage DOES NOT MEAN hidden from the browser.**

Always check the source code when investigating a webpage.
