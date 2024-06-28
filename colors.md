## How to use colors
You can use colors in chat by typing a `&` preceded by a **hex code** or **color codes**.

## Hex
- `&#ff0000hello` - Makes the text "hello" the color `#ff0000` which is as red as it gets.
- `&#2f4870hi` - Makes the text "hi" the color `#2f4870hi` which is a nice blue.

## Color Codes
Color codes are basically shortcuts to a hex code. Instead of typing `&#00AAAA` you can just type `&3` instead.
Color codes are just palette colors

## Palettes
Palettes are a collection of color codes.
Instead of having to write out the hex code each time for a color, just reference them by their **code**.
See a list of palettes by typing `/palettes`. Click on a palette to see their color codes.
Hover over the square with the color that you want to see the color code, and click on it to copy it to your clipboard.
Paste the code after a typing a `&` i.e. `&bf1`.

## Gradients
You can combine multiple colors to form a gradient! 
- **Manual Gradient** - Combining multiple color codes turns the preceding text into a gradient i.e. `&a&b&cHELLO`
- **Palette Gradient** - Type a palette's name after the `&` and then add a special character after it to grab that palette as a gradient!
  - `&palette>` - Creates a gradient from the all the palette colors (left to right)
  - `&palette<` - Creates a gradient from the all the palette colors (right to left)
  - `&palette*` - Creates a gradient from all the palette colors (left to right to left)
  - `&palette^` - Creates a gradient from all the palette colors (right to left to right)
  - `&palette#` - Creates a gradient from all the palette colors (shuffled)

## Functions
- **Random Color** - `&x[0-200]` where you enter a number **between 0 and 200** after `&x`
- **Invert Color** - `&(...)!` where you put a **!** at the end of your color code(s) to invert them
- **Random Color from a palette** - `&palette?`

### Note...
- Don't get mad if you can't type `&` and nothing shows up, simply use a double `&&` in its place.
- Do not attempt `&rgb(r,g,b)`, you would be a fool to do so.
- Don't forget your `#` before your hex code or else you will cry!
- Also, minecraft doesn't support opacity so your hex code better be exactly **6** characters long!
- All the special characters that apply to **palette gradients** (`><^*#?`) do not apply to **manual gradients** (i.e. `&a&b&c<Hey`)
