# Topic: Knowledge check

# Link: https://www.theodinproject.com/lessons/foundations-intro-to-css#knowledge-check


- What is the syntax for class and ID selectors?

class="yourClass"

.yourClass{
    properties: value
}


id="yourId"

#yourId{
    properties: value
}


- How would you apply a single rule to two different selectors?

1- Adding a shared class to both selectors
2- grouping / chain / descendant-combinator


- Given an element that has an id of title and a class of primary, how would you use both attributes for a single rule?

could be using a chain selector

#title.primary{
    single rule
}

- What does the descendant combinator do?

it apply certain style to a nested element, in any deep of the nesting, but need to use with care.

- What are the names of the three ways to add CSS to HTML?

1- External CSS
2- Internal CSS
3- Inline CSS


- What are the main differences between the three ways of adding CSS to HTML?

External CSS is the preferred way of do things with styles, as using a separated file to hold all the styles keep the HTML file clean and light.

Having a External file gives the change to use this same file for multiple HTML documents so to keep organize the code.

Internal and Inline CSS are not that convenient, but they have some perks as to test something in site, plus giving the opportunity to make some changes that erase the code of the main style document.
