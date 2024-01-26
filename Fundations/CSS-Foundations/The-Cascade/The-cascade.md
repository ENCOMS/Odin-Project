# Topic: The Cascade

## link: https://www.theodinproject.com/lessons/foundations-the-cascade

## What the cascade does.

### What is Cascade of CSS

The cascade is what determines which rules actually get applied to our HTML. There are different factors that the cascade uses to determine this. We will examine three of these factors, which will hopefully help you avoid those frustrating “I hate CSS” moments.

## Specificity and combining CSS selectors.

### Specificity

A Css declaration that is more specific will take precedence over less specific ones.

ex: inline styles, have highest specificity compared to selectors

- ID selectors (most specific selector)
- One or More Class selector (descendant selectors, grouping[only after])
- Type selectors
- Universal selector (Don't have a specificity value)

Specificity will only be taken into account when an element has multiple, conflicting declarations targeting it, sort of like a tie-breaker. An ID selector will always beat any number of class selectors, a class selector will always beat any number of type selectors, and a type selector will always beat any number of less specific selectors. When there is no declaration with a selector of higher specificity, a rule with a greater number of selectors of the same type will take precedence over another rule with fewer selectors of the same type.

- Class selector

```
<!-- index.html -->

<div class="main">
  <div class="list subsection">Red text</div>
</div>
/* rule 1 */
.subsection {
  color: blue;
}

/* rule 2 */
.main .list {
  color: red;
}
```

Note: 
- It wont matter if before of after the single selector, if rule 2 use descendant selector specify
- for chaining won't work
- for grouping only work after.

- Using ID selector specify
```
<!-- index.html -->

<div class="main">
  <div class="list" id="subsection">Blue text</div>
</div>
/* rule 1 */
#subsection {
  color: blue;
}

/* rule 2 */
.main .list {
  color: red;
}
```

In this case Id selector takes precedence 

ID > Class > Type selectors

if two rules have ID
    Wins the one with more classes

if they have the same quantity of class selectors

## How inheritance affects certain properties.

### Inheritance
Inheritance refers to certain CSS properties that, when applied to an element, are inherited by that element’s descendants, even if we don’t explicitly write a rule for those descendants.
Typography-based properties (color, font-size, font-family, etc.) are usually inherited, while most other properties aren’t

The exception to this is when directly targeting an element, as this always beats inheritance

parent
    child (if are targeting this one it will win the changes, but still receive the parent properties and values that are not affected)

### Rule order
The final factor, the end of the line, the tie-breaker of the tie-breakers. Let’s say that after every other factor has been taken into account, there are still multiple conflicting rules targeting an element. How does the cascade determine which rule to apply?

- Whichever rule was the last defined is the winner.




