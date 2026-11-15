# Natas 2 — Writeup

## Objective

Find the password for **Natas 3**.

## What We Have

* Username: `natas2`
* Natas 2 webpage
* Password for `natas2`

## What We Need

The password for **natas 3**.

## Initial Investigation

Open the Natas 2 webpage.

The page looks almost empty.

Check the page source:

```text
Ctrl + U
```

Look through the HTML for anything interesting.

A line contains:

```html
<img src="files/pixel.png">
```

This shows that the website has a `/files/` directory.

## Why Do This?

The HTML source tells where the webpage gets its files from.

If the page loads something from:

```text
/files/
```

there may be other files or directories stored there.

So, try opening the directory directly:

```text
/files/
```

## Solution

Open:

```text
http://natas2.natas.labs.overthewire.org/files/
```

The directory listing shows another file:

```text
users.txt
```

Open:

```text
/files/users.txt
```

The file contains usernames and passwords.

Find the entry for:

```text
natas3
```

Copy the password and use it to log in to **Natas 3**.

## Concept Learned

* HTML source inspection
* Directory discovery
* Directory listing
* Exposed files
* Basic web reconnaissance

## Tools Used

```text
Browser
View Page Source
```

## Lesson

**Don't only inspect what the webpage displays.**

Check the source code and investigate files/directories referenced by the page.
