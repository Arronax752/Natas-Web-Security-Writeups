# Natas 1 — Writeup

## Objective

Find the password for **Natas 2**.

## What We Have

* Username: `natas1`
* Natas 1 webpage
* Password for `natas1`

## What We Need

The password for **natas2**.

## Initial Investigation

Open the Natas 1 webpage.

A message says that the password is **not visible**, but the page source may contain something interesting.

Try:

```text
Ctrl + U
```

But this time, right-clicking is disabled.

## Why Do This?

The website tries to prevent access to the page source through the right-click menu.

But disabling right-click doesn't actually protect the HTML source.

The browser still receives the HTML from the server.

So, open the source directly with:

```text
Ctrl + U
```

## Solution

Search through the HTML source.

The password for **natas2** is present in the source code.

Copy the password and use it to log in to **Natas 2**.

## Concept Learned

* HTML source inspection
* Client-side restrictions
* Right-click protection
* Browser developer features

## Tools Used

```text
Browser
Ctrl + U
View Page Source
```

## Lesson

**Client-side restrictions are not real security.**

Disabling right-click can make something less convenient to access, but it doesn't prevent the browser from receiving the source code.
