# svg-clock-class
PHP classes to dynamically generate and configure clocks for visual math problems

## Questions

1. What was the goal and what were the requirements? How does this work meet them?

We had numerous math problems featuring clocks. However, it was a lot of raw HTML/CSS that was mostly duplicated across the files and difficult to manage.

The goal was to update all instances of clocks with a new, class-based, SVG clock alternative. We also needed to preserve all the math logic, interactivity, and functionality of those respective math problems and thus had a list of minimum features to bake into the class(es).

Ultimately, this class allowed us to dramatically reduce the size of those respective files by having clean, minimal instantiations of our new clock class while preserving the logic and functionality of those math problems. This also allowed us to more easily maintain the math logic by making it easier to focus on simple parameters rather than updating numerous values across often bloated and messy raw HTML/CSS clocks. They also looked a lot better!

2. Who did you work on this with, and which parts were you responsible for?

I coded all of this entirely by myself but had several conversations with my team during pair programming sessions so I could ask for input or confirmation of design choices.

Originally, I set to work building a monolithic class file just for the clock objective alone. But, as we went along, it became increasingly obvious how easily we could share certain logic while upgrading several other of our raw HTML/CSS type visual assets to SVG.

The included files are actually plucked from a 'family' of SVG classes we ultimately built that feature not only clocks, but also box plots, shapes, scatterplots, and angles (to teach degrees).