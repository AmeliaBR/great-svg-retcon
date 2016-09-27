# The Great SVG RetCon

- **Cover Slide**
- **Title Page**
- Introduce myself
- **Cover Repeat**
- Define terms: Great, SVG, Con
- Broken continuity
- **A magic suit**
- **Retroactive**
- Why?
- Move the story forward
- **A spinoff TV show**
- **just one problem**

## RetCon-ing the Web
- Continuity even more important
- You can't reboot the web
- Different from other programming environments
- Different from JS frameworks & libraries
- **It's been tried (XML)**
- **or like this (XML part 2)**
- Standards makers have learned
- Old websites still supported
- New features allow fallbacks
- **picture element builds on img**
- **brings us to SVG 2**
- Candidate Recommendation
- Many new features
- Also many dropped features
- Today, focus on changes in concepts.

## Markup
- **SVG is XML**
- XML didn't take over the world
- Retcon'd story:
- **SVG is ... or XML** (_read!_)
- You probably already use it
- SVG 2 changes just tidying up
- **But .svg still XML**
- Same markup, different file name, different parser
- What if you need .svg?
- **Use the parser, Luke**
- Easy: MS Edge right-click
- Otherwise: Dev Tools
- What about reverse direction?
- Continuity good, except:
- **No weird prefixes**
- SVG software will use correct prefixes, but:
- **Avoid bloated files**
- HTML parser ignores it, but why have it?
- **Warning: namespaces & scripting**
- The proper way
- Use the parser, Luke
- (watch for innerHTML support)

## Links
- Next most basic part of the web
- The old story:
- **SVG uses XLink ...** (_read!_)
- XLink was a neat idea
- But went nowhere
- SVG only "simple" links
- HTML had same, without XLink
- So:
- **SVG uses href ...** (_read!_)
- What does this mean to you?
- **Not much, Sorry**
- Continuity with old browsers
- Fallback rules in spec don't help authors
- **Except for test cases**
- Browser test results
- It will get better... (when you can drop support for old browsers)

## Styles
- This is a CSS conference
- But CSS was still new
- **SVG styles ... or XML attr** (_read!_)
- CSS support was not required
- But CSS keeps getting bigger
- 3 problems:
  - Too many attributes
  - New features don't map to attributes
  - No fallback in attributes
- So:
- **SVG styles are defined ...** (_read!_)
- CSS required _for software_
- No new presentation attributes
- **CSS-in-SVG automatically upgrades**
- Use CSS fallback methods
- But where?
- Img must be same file
- Object / Inline can be external
- 2 dangers:
  - Style clash for inline
  - Lost URL refs
- But what does it mean to style an SVG?

## Geometry
- style vs content
- **Geometric structure...**
- Works for drawings
- **Cat vs Rabbit vs Crazy Cat**
- But not all SVGs are drawings
- geometry as stylistic choice
- repeated geometry for classes
- Presentation attributes = RetCon opportunity!
- New separation of style and structure
- **Document structure...**
- Document structure defined
- Benefits:
  - reduce duplication
  - media queries
  - pseudoclasses
  - CSS animations & transitions
- **But… attributes ≠ styles**
  - attribute always has element
  - style (should be) universal
- **rx & ry, rect vs ellipse**
- **rx & ry, defaults differ**
- Choice to break continuity; only breaking an error state
- Other cases not so easy, e.g. text
- The RetCon is incomplete
- **Geometry Properties Table**
- shapes vs graphical effects
- Polygon, polyline, line missing
- Didn't want to lock in bad decisions
- May need new CSS-friendly syntax,
similar to transform

## Transforms
- Other half of core SVG geometry
- Also originally attribute-only
- **SVG coordinate system ... attribute**
- **transform examples**
- manipulate shape/drawing as a whole, without changing geometry attributes
- CSS wanted it, too
- CSS Transforms module
- For SVG, same presentation attribute RetCon
- But style also applies to other elements
- Revised story:
- **Coordinates can be...**
- Wonderful.
- Not wonderful.
- Buggy transforms in SVG?
- Broken continuity!
- CSS Transforms spec designed for CSS layout needs.
- **SVG layout vs CSS**
- Firefox: continuity
- Blink/WebKit: consistency(-ish)
- Microsoft: Nothing (yet)
- Solution: transform-box!
- **view-box vs fill-box: setup**
- **view-box vs fill-box: figure**
- default will be backwards compatible
- change transform-box and transform-origin for same behavior as CSS
- no transform-box options for non-SVG yet
- Not in browsers. Coming soon(-ish).
- Final story:
- **Coordinates ... and transform-box ...**
- For now: fallbacks!
- Attribute works everywhere
- But other differences
- **Table of syntax comparisons**
- Biggest difference: units
- Other: new shorthands
- These were good retcons!
- Use legacy syntax for now.
- Can use CSS transforms, with careful fallback:
  - optional hover effects
  - alternate media query layouts
- **3D with 2D fallback**
- Beware many 3D bugs!
- **Fallback layout if no 3D**

## So much more
- Not enough time!

## About me

