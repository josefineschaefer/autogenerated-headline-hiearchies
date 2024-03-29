# Autogenerated headline hierarchy example using SvelteKit and Storyblok

When using a Content Management System, there are different ways to make sure headline hierarchies are used in a meaningful way. In order to provide context for screen reader users, we want to make sure there is only one `<h1>`, that we stick to a meaningful order of headlines and are not using `<div>` or `<span>` elements excessively to just visually present those different headlines. 

## Autogenerated Headline Hierarchies

In this example, we are using Storyblok, SvelteKit and TailwindCSS to illustrate how you could use a helper function to check whether an element is the first on the page by using the index; If it is the first, the `<h1>` element is automatically assigned to the headline. If it isn't the first, `<h2>` is used. This way, you only have one `<h1>`. 

### Limitations of this Example

Of course, in the "real world" we usually have more than two headlines and having one `<h1>` and many `<h2>` elements would not fulfill the purpose of making our headline hierarchies meaningful or accessible. Therefore, it's only applicable in this very small tutorial. In larger scale projects with more complex headline hierarchies, the logic would have to be extended, or in case of working with a (headless) CMS like Storyblok, restrictions could be set in place, for example which component can be used where or nested within each other, for example. 

### Resources

Are you curious about making your (headless) project more accessible? You can read about our suggestions in our article series on [accessible web development with Storyblok](https://www.storyblok.com/tp/accessible-web-development-with-storyblok), about [headline hierarchies](https://www.storyblok.com/tp/accessible-headline-hierarchies) more specifically in the corresponding article. 
