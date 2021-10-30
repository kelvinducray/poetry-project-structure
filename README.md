# Poetry Project Structure
1. **Create a new repository on Github & initialise with a README.**
    *Optional*:
    - Use the Python ```.gitignore``` github provides
      - If you are using Mac, add ```.DS_Store``` to your ```.gitignore``` before
        you commit any code
    - License - MIT is very popular and highly permissive if you want to share
      your code for re-use  

2. **Clone the repository**
    Example:
    ```
    gh repo clone kelvinducray/poetry-project-structure
    cd poetry-project-structure
    code .
    ```  

3. **Initialise with Poetry**
    ```
    poetry init
    poetry shell
    ```  

4. **Create a project slug and starting scripts**
    Your project slug will be your project name with underscores
    instead of dashes, then create an ```__init__.py``` and a ```__main__.py.```
    The ```__main__.py``` is what will execute when you run:
    ```python -m <your_project_name>```
    From the base directory of the project.  

    *Note*: When import scripts within your project ensure you add a full-stop
    before the script name, e.g.:
    ```from .script import ...```