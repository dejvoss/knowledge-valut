## Useful tips about programming in python, Jupyter notebooks, data science, machine learning, etc.

### Sharing jupyter notebooks
There are few ways of quick sharing your work done in jupyter notebooks:
- [nbviewer](https://nbviewer.jupyter.org/): Paste the link to your notebook and share it with others.
- [Google Colab](https://colab.research.google.com/): Google collab allow you to run jupyter notebooks in the Google cloud environment. The notebooks you craete in google collab are stored in your Google Drive and can be shared with others just like any other Google Drive file.
- [Binder](https://mybinder.org/): Binder allows you to create a docker image of your jupyter notebook and share it with others. The notebooks are stored in the GitHub repository and can be shared with others by pasting the link to the repository.

### How to clone and push repository to GitHub with Token instead a username and password.

1. Generate a token in GitHub. Go to Settings -> Developer settings -> Personal access tokens -> Generate new token. Select the scopes you need and generate the token. Copy the token to the clipboard.
2. Clone the repository to your local machine. Open the terminal and type the following command:
```bash
git remote set-url origin https://<TOKEN>@github.com/<USERNAME>/<REPOSITORY>.git
```
3. Once you clone the repo that way you can push and pull the changes without the need to enter the username and password.

### Programming principles
- [DRY - Don't Repeat Yourself](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself): The DRY principle is a software development principle, which states that duplication in logic should be eliminated via abstraction; duplication in process should be eliminated via automation.
- [KISS - Keep It Simple, Stupid](https://en.wikipedia.org/wiki/KISS_principle): The KISS principle states that most systems work best if they are kept simple rather than made complicated; therefore, simplicity should be a key goal in design, and unnecessary complexity should be avoided.
- [YAGNI - You Aren't Gonna Need It](https://en.wikipedia.org/wiki/You_aren%27t_gonna_need_it): The YAGNI principle states that a programmer should not add functionality until deemed necessary.
- [SOLID](https://en.wikipedia.org/wiki/SOLID): SOLID is an acronym for five design principles intended to make software designs more understandable, flexible, and maintainable.
- [Single Responsibility Principle](https://en.wikipedia.org/wiki/Single-responsibility_principle): A class should have only a single responsibility.
- [Open/Closed Principle](https://en.wikipedia.org/wiki/Open%E2%80%93closed_principle): Software entities should be open for extension but closed for modification.
