# Pancake Recipe

## About the Project

This is a simple recipe website for making pancakes, created as a practice project to learn and improve my HTML and CSS skills.

## Technologies Used

- HTML5
- CSS3
- ex testing 
- pillow

```bash
python -c "from PIL import Image; print('Pillow is ready')"
python -c "from pathlib import Path; from PIL import Image, ImageOps; p=Path('images'); sizes={'hero-food':1600,'pancakes':900,'waffles':900,'pasta':900,'salad':900,'risotto':900,'brownies':900}; [(lambda src,limit: (lambda im: (im.thumbnail((limit,limit),Image.Resampling.LANCZOS), im.convert('RGB').save(src.with_suffix('.webp'), 'WEBP', quality=82, method=6)))(ImageOps.exif_transpose(Image.open(src)) ))(p/f'{name}.jpeg',limit) for name,limit in sizes.items() if (p/f'{name}.jpeg').exists()]; print('Conversion finished.')" 
python -c "from pathlib import Path; from PIL import Image; [(lambda im: print(f'{p.name}: {im.width}x{im.height}'))(Image.open(p)) for p in sorted(Path('images').glob('*.webp'))]"
```

## Structure

```text
Recipe/
├── index.html
├── page-2.html
├── page-3.html
├── style.css
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
│   └── waffles.html
└── categories/
    ├── breakfast.html
    ├── lunch-dinner.html
    ├── healthy.html
    └── desserts.html
```

## Features

- Pancake ingredients list
- Step-by-step cooking instructions
- Simple and clean layout
- CSS styling

## What I Learned

- Structuring a webpage with semantic HTML
- Styling elements with CSS
- Organizing content in a clear and readable way

## Getting Started

1. Clone or download this repository.
2. Open `index.html` in your web browser.
3. Explore the pancake recipe.

## Future Improvements

- Improve the responsive design for mobile devices.
- Add more recipes.

---

This project was created for learning purposes.
