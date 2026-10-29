# Recipe Website

## About the Project

This is a simple, responsive recipe website created as a practice project to learn and improve my HTML5 and CSS3 skills.

The website features a collection of recipes, organized into categories, with individual pages containing ingredients and step-by-step cooking instructions.

## Technologies Used

- HTML5
- CSS3
- Python 3
- Pillow for image optimization
- Git and GitHub

## Features

- Homepage featuring selected recipes
- Six individual recipe pages
- Four recipe categories:
  - Breakfast
  - Lunch & Dinner
  - Healthy
  - Desserts
- Ingredient lists and step-by-step instructions
- Shared CSS stylesheet for consistent styling
- Responsive layout for different screen sizes
- Optimized WebP images
- Semantic HTML structure and descriptive image alt text
- Navigation between the homepage, categories, and individual recipes

## Project Structure

```text
Recipe/
├── index.html
├── page-2.html
├── page-3.html
├── style.css
├── README.md
├── images/
│   ├── hero-food.webp
│   ├── pancakes.webp
│   ├── waffles.webp
│   ├── pasta.webp
│   ├── risotto.webp
│   ├── salad.webp
│   └── brownies.webp
├── recipes/
│   ├── pancakes.html
│   ├── waffles.html
│   ├── pasta.html
│   ├── risotto.html
│   ├── salad.html
│   └── brownies.html
└── categories/
    ├── breakfast.html
    ├── lunch-dinner.html
    ├── healthy.html
    └── desserts.html
```

## Image Optimization

Images were converted to WebP format and resized using Python and Pillow to reduce file sizes and improve loading performance.

To verify that Pillow is installed, run:

```bash
python -c "from PIL import Image; print('Pillow is ready')"
```

To inspect the dimensions of the WebP images, run:

```bash
python -c "from pathlib import Path; from PIL import Image; [(lambda im: print(f'{p.name}: {im.width}x{im.height}'))(Image.open(p)) for p in sorted(Path('images').glob('*.webp'))]"
```

The image conversion script was used during development to create optimized versions from the original JPEG files.

## Getting Started

1. Clone or download this repository.
2. Open the project folder.
3. Open `index.html` in your web browser.
4. Explore the recipes and browse the different categories.

No additional installation is required to view the website.

## What I Learned

- Structuring webpages with semantic HTML elements.
- Styling and organizing layouts with CSS.
- Reusing a shared stylesheet across multiple pages.
- Creating navigation between related pages.
- Organizing recipes into categories.
- Improving image loading performance with WebP.
- Using Python and Pillow for image processing.
- Checking accessibility and performance with browser developer tools.

## Future Improvements

- Add more recipes and categories.
- Continue improving accessibility and responsive design.
- Explore additional ways to optimize website performance.

---

This project was created for learning purposes as part of my ongoing web development practice.
