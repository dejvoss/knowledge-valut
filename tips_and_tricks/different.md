# Tips and Tricks for everything not in Python.

## How to clone and push repository to GitHub with Token instead a username and password.

1. Generate a token in GitHub. Go to Settings -> Developer settings -> Personal access tokens -> Generate new token. Select the scopes you need and generate the token. Copy the token to the clipboard.
2. Clone the repository to your local machine. Open the terminal and type the following command:
```bash
git remote set-url origin https://<TOKEN>@github.com/<USERNAME>/<REPOSITORY>.git
```
3. Once you clone the repo that way you can push and pull the changes without the need to enter the username and password.

## Excel keyboard shortcuts
- `Ctrl + Shift + L` - Apply filter
- `Ctrl + Shift + 1` - Format as number
- `Ctr + d` - Copy the value from the cell above
- `F4` - pressed during typing formula will lock the cell reference (will add sign of $ before the column and row), pressing again will lock only the column, pressing again will lock only the row, pressing again will unlock the cell reference.
- `Ctrl + ~` - Show formulas in the cells

## Excel functions
- `=round(number, number_of_decimal_places)` - round the number to the specified number of decimal places, what is interesting that it round also to the negative numbers of decimal places, for example, `=round(123.456, -1)` will round the number to the nearest ten, so the output will be `120`.
- `sum.ifs(range1, criteria1, [range2], [criteria2], ...)` - sum the values that meet the criteria. The function can have multiple ranges and criteria. In you want to sum all values that are greater than 10 you can place sign ">" before the number, for example `=sum.ifs(A1:A10, ">10")`. Other signs are works too.
