# Mostly Harmless Cafe

## Contributing recipes

Thanks for your interest in contributing recipes!

Any recipes are welcome but here's what we currently need most:
- Submissions
    - Drinks (alcoholic and non-*)
    - Baking
    - Desserts
    - Anything that isn't currently listed as a category
- Website
    - I'm still new to web design so if you see something you can't stand, make a PR or issue saying what you'd like us to try out.

### Via Issue Request

Click the `Issues` tab and select `New issue`. Add the title of your dish, all the ingredients, the steps for the recipe, and a picture of the end product. I'll manually create the post and add it to the recipe branch.

### Via Pull Request

Clone the repo:

`git clone https://github.com/deadbody/deadbody13.github.io`

Create your entry with `hugo new content/post/recipe-title.md` (if you don't have Hugo, install it, it should be in most mainstream repos).

Modify the frontmatter to include the following information (anything with a `< >`, remove the brackets)

```
deadbody13.github.io/content/posts/<recipe-title>.md
---
title: "<Recipe Title>"
date: 2023-06-17T16:39:03-04:00
draft: false
credits:
- <person-1>
- <person-2>
tags:
- <tag-1>
- <tag-2>
---
```

#### Formatting Your PR

##### Tags

Tags are used to categorize the food and drinks and sort them into their respective pages. All posts should generally include either a food or drink tag and any other tags that you think should apply.

The current tags are:
- food (include with all food posts)
    - burgers
    - chicken
    - pasta
    - sauce
- Drinks (include with all drinks)
    - alcoholic
    - non-alcoholic
 
If you don't see a tag here that you think should be included with your recipe, go ahead and list it in the front-matter like all the other tags. If I see enough food/drink items for a particular tag (like `baking`, `desserts`, etc.) I'll add it to the menu and it's better to include too many tags than not enough.

##### Organization

Entries should have at least an `## Ingredients` (unordered) and `## Instructions` (ordered) section. You can also include a section at the end `### Optional` (unordered).

##### Images
When submitting images, use Hugo's `figure` shortcode. This allows you to label and credit the images with captions. If you got the photo from someone else or you would like credit yourself, remember to credit the image in the caption.
```
{{< figure src="/images/food-images/image.jpg" caption="caption; image by anon001" alt="alt" >}}
```

##### Crediting Yourself or Others

Credits are... for giving credit. If you want to credit yourself or another person list them here (i.e. `- deadbody13`)

##### Previewing
The following command is used to host the website locally. It will then be accessible via `https://localhost:1313/` or something like that.

```
hugo server -D
```

## Furthermore

Try not to include stories, epiphanies on life, embarrassing moments from high school, that time you scraped your knee, or other stuff that people may feel the need to scroll past to get to the recipe itself.


## Contributing to the Website

Have something you think would make the website better (styling, layouts, etc.)? Submit a PR and we'll look into it.

## Credits for Website

[Spicy Forth](https://github.com/SpicyForthProgrammer) - graphics design, web hosting

[Fonts](https://indestructibletype.com/Home.html) are from Owen Earl from IndestructibleType*.
