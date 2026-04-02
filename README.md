# Homepage Feature Cards Coding Exercise

This project demonstrates how to build a simple set of **homepage feature cards** using HTML and CSS.

Feature cards are small content blocks often placed on a homepage to preview important parts of a website. They help organize information into smaller sections that are easier to scan and understand.

This example also includes a **call-to-action section** below the cards. A call-to-action section is a highlighted area designed to draw attention and encourage the visitor to take the next step.

## Learning goals

The goal of this exercise is to help you practice:

- building a practical layout with CSS Grid
- using repeated content structures
- aligning content with Flexbox
- creating visual hierarchy with cards and a call-to-action section
- designing homepage content that is easier to scan and understand

<br>

## What this example includes

This page includes:

- a header with a site title and navigation links
- an introduction section explaining feature cards
- a three-column set of feature cards
- icons placed next to card headings
- a highlighted call-to-action section
- a styled button
- a media query for smaller screens

<br>

## Files in this project

- `index.html` – the HTML structure for the page
- `reset.css` – a reset stylesheet to remove browser default spacing and styling
- `cards.css` – the CSS styles for the page

<br>

## What are feature cards?

Feature cards are useful because they:

- break content into smaller pieces
- help visitors scan the page more quickly
- highlight important sections of a site
- create a more organized and polished homepage layout

Cards are often used for things like:

- services
- portfolio categories
- featured projects
- important site sections
- quick previews of content
- helpful information or tips

<br>

## HTML structure used in this example

Each card is built with a repeated structure:

- a card container
- a title row
- an icon
- a heading
- a paragraph

Here is the general pattern:
```html
    <article class="card">
      <div class="card-title">
        <span class="card-icon">🎨</span>
        <h3>Creative Work</h3>
      </div>

      <p>
        Use a card like this to highlight an important part of your site.
      </p>
    </article>
```
This repeated structure is helpful because once you build one card, you can reuse the same pattern for the others.

<br>

## How the cards are arranged

The cards are placed inside a parent container called `.card-grid`.

That container uses **CSS Grid** to arrange the cards into columns.

Example:

```css
  .card-grid {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    gap: 1.5rem;
  }
```
### What this means

- `display: grid;` turns the container into a grid layout
- `grid-template-columns: 1fr 1fr 1fr;` creates 3 equal-width columns
- `gap: 1.5rem;` adds space between the cards

This is one of the most important parts of the exercise because it shows how Grid can be used for a practical real-world layout.

<br>

## Why there is also Flexbox in this project

The main layout method in this exercise is **Grid**, but there is also a small use of **Flexbox** inside each card title.

The card title row uses Flexbox to place the icon and heading on the same line.

Example:
```css
  .card-title {
    display: flex;
    align-items: center;
    gap: 0.75rem;
  }
```
### What this means

- `display: flex;` places the icon and heading in a row
- `align-items: center;` lines them up vertically
- `gap: 0.75rem;` adds space between them

So in this project:

- **Grid** controls the larger card layout
- **Flexbox** helps line up smaller content inside each card

<br>

## Call-to-action section

Below the cards is a **call-to-action section**.

This section is used to visually stand out from the rest of the page and encourage the visitor to do something next, such as:

- learn more
- contact the site owner
- explore another page
- view a gallery
- start a project

This call-to-action section includes:

- a heading
- a short paragraph
- a link styled to look like a button

<br>

## Button styling

The call-to-action link is styled to look like a button using CSS.

Example:
```css
  .cta-button {
    display: inline-block;
    background-color: #457b9d;
    color: #ffffff;
    text-decoration: none;
    font-weight: bold;
    padding: 0.9rem 1.4rem;
    border-radius: 0.75rem;
  }
```
This helps the link look more noticeable and clickable.

<br>

## Responsive design

This page also includes a media query for small screens.

At smaller screen sizes, the card layout changes from multiple columns to a single column.

Example:
```css
  @media (max-width: 480px) {
    .card-grid {
      grid-template-columns: 1fr;
    }
  }
```
This helps keep the cards readable on phones and smaller devices.

<br>

## Customizing this example

After following along with the coding exercise, your version should not remain an exact copy of the starter.

You should customize your page by changing things such as:

- the card headings
- the card paragraphs
- the emoji icons
- the button text
- colors
- spacing
- border radius
- background colors
- hover effects

You may also choose to replace the emoji with **Font Awesome icons** if you want a different visual style.

<br>

## Using this in your final project

You are welcome to reuse this code in your final project if it fits your site well. However, you should customize it enough that the final result clearly feels like your own work and not just an exact copy of the example.

Feature cards can be useful on many kinds of websites, including:

- portfolio sites
- hobby or fan sites
- business sites
- informational sites
- event sites

<br>

## Key idea to remember

A homepage does not have to be one long block of text.

Feature cards help organize content, guide the visitor, and make important parts of the site easier to notice.
