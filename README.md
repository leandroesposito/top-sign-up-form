# Odin Sign-up Form

This is a front-end demonstration project of a responsive sign-up form with client-side validation and a visually appealing design. Features a split-panel layout with a scenic background image and a clean form interface.

Preview: [https://leandroesposito.github.io/top-sign-up-form/](https://leandroesposito.github.io/top-sign-up-form/)

## Features

- **Split-panel design** - Left panel with hero image and branding, right panel with form content
- **Responsive layout** - Adapts to different screen sizes using flexible units
- **Form validation** - Built-in password pattern validation (8-20 characters, requires uppercase, lowercase, and numbers)
- **Password confirmation** - Fields for password and confirm password
- **Modern styling** - Clean typography, subtle shadows, and focus states
- **Custom fonts** - Norse font for branding, system fonts for form content

## Technologies Used

- HTML5
- CSS3 (Custom properties, Flexbox)

## Screenshots

| Desktop View | Mobile View |
|--------------|--------------|
| <img src="https://github.com/leandroesposito/top-sign-up-form/blob/main/screenshots/desktop_view.png" height="700" alt="Desktop"> | <img src="https://github.com/leandroesposito/top-sign-up-form/blob/main/screenshots/movile_view.png" height="700" alt="Movile"> |

## Project Structure

```
sign-up-form/
├── index.html          # Main HTML document
├── style.css           # Styling and layout
├── fonts/              # Custom font files
│   ├── norse-bold-webfont.woff
│   └── norse-bold-webfont.woff2
└── imgs/               # Image assets
    ├── background.jpg  # Hero background image
    └── odin-lined.png  # Logo image
```

## Form Fields

The form includes the following fields:
- First Name (text)
- Last Name (text)
- Email (email format)
- Phone Number (tel format)
- Password (with pattern validation)
- Confirm Password

### Password Requirements
- Minimum 8 characters
- Maximum 20 characters
- At least one uppercase letter
- At least one lowercase letter
- At least one number

## Color Scheme

| Variable | Color | Usage |
|----------|-------|-------|
| `--color-white` | #F9FAFB | Right panel background |
| `--color-background-transparent` | rgba(0,0,0,0.5) | Overlay backgrounds |
| `--color-grey-font` | #1F2937 | Form text |
| `--color-light-border` | #E5E7EB | Input borders |
| `--color-focus` | rgb(29, 78, 216) | Input focus state |
| `--color-invalid` | rgb(189, 42, 42) | Invalid input state |
| `--color-image` | #7BA9CE | Button and link color |

## Customization

### Changing the Background Image
Replace `imgs/background.jpg` with your own image (recommended size: at least 1200x800px).

### Modifying Form Validation
Update the `pattern` attribute in the password input fields:
```html
pattern="(?=.*[a-z])(?=.*[A-Z])(?=.*\d).{8,20}"
```

### Adjusting Layout
Modify the CSS variables or Flexbox properties in `style.css`:
- `--title-heigth` - Controls logo and title size
- `.left-panel` flex basis - Controls left panel width

## Acknowledgments

- Background photo by [Rafael Hoyos Weht](https://unsplash.com/@rhweht) on [Unsplash](https://unsplash.com/)
- Odin logo from [The Odin Project](https://www.theodinproject.com)
- Norse Bold font by [Joël Carrouché](https://www.jcfonts.com/)

**Note:** This is not a real online service. Created as part of a front-end development exercise.
