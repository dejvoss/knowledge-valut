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

### Comparing two lists in python
To compare two lists, the best would be to get the unique elements from both lists. To do that we can convert list to set:
```python
list1 = [1, 2, 2, 3, 4, 5]
set(list1)
```
The output will be:
```python
{1, 2, 3, 4, 5}
```
Now we can compare two sets:
```python
list1 = [1, 2, 2, 3, 4, 5]
list2 = [1, 2, 3, 4, 5]
set(list1) == set(list2)
```
The output will be:
```python
True
```
Sometimes, except to compare we want also to know the common elements of two lists. To do that we can use the following code:
```python
list1 = [1, 2, 2, 3, 4, 5]
list2 = [1, 2, 3, 4, 5]
set(list1).intersection(set(list2))
```
The output will be:
```python
{1, 2, 3, 4, 5}
```
One more example:
```python
list1 = [1, 2, 2, 3, 4, 5]
list2 = [5, 6, 7, 8, 9, 10]
set(list1).intersection(set(list2))
```
The output will be:
```python
{5}
```
