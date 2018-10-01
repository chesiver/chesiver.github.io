---
title: "Determining the dimensions of elements"
categories: 
  - html/css
---

## How much room does it use up

If you need to know the total amount of space an element occupies, including the width of the visible content, scrollbars (if any), padding, and border, you want to use the HTMLElement.offsetWidth and HTMLElement.offsetHeight properties. Most of the time these are the same as width and height of Element.getBoundingClientRect(), when there aren't any transforms applied to the element. 

## What's the size of the displayed content?
If you need to know how much space the actual displayed content takes up, including padding but not including the border, margins, or scrollbars, you want to use the Element.clientWidth and Element.clientHeight properties:

## How big is the content?
If you need to know the actual size of the content, regardless of how much of it is currently visible, you need to use the Element.scrollWidth and Element.scrollHeight properties. These return the width and height of the entire content of an element, even if only part of it is presently visible due to the use of scroll bars.