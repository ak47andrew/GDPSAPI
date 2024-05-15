# Your First Code Contribution

To set up your environment for contributing to GDPS API, follow these steps:

## 1. Fork the repository

Before you can contribute to GDPS API, you need to fork the repository to your own GitHub account. This will create a copy of the repository that you can clone to your local machine and make changes to. Here's how you can fork the repository:

1. Go to the [GDPS API repository page](https://github.com/ak47andrew/GDPSAPI) on GitHub.
2. Click on the "Fork" button in the top-right corner of the page.
3. You will now have a copy of the repository in your own GitHub account.

## 2. Clone the forked repository

After forking the repository, you need to clone it to your local machine. Here's how you can do that:

1. Open your terminal or command prompt.
2. Run the following command to clone the forked repository to your local machine:

```bash
git clone git@github.com:<your-github-username>/GDPSAPI.git
```

Replace `<your-github-username>` with your actual GitHub username. This will create a copy of the repository in your local machine's directory structure.

## 3. Create a virtual environment

We recommend using a virtual environment to isolate the project dependencies from your system's dependencies. To create a virtual environment, use the following command:

```bash
python3 -m venv venv
```

## 4. Activate the virtual environment

After creating the virtual environment, you need to activate it. The process for activating the virtual environment depends on your operating system:

- **Windows**: Open the `venv\Scripts\` folder and run `activate.bat`.
- **Linux/macOS**: Open the `venv/` folder and run `source activate`.

## 5. Install dependencies

Once the virtual environment is activated, you can install the project dependencies by running the following command:

```bash
pip install -r requirements.txt
```

## 6. Format the code and perform static type checking

GDPS API follows the [Autopep8](https://github.com/chrisatmachine/autopep8) code formatter and [Pylint](https://www.pylint.org/) for static type checking. To format the code and perform static type checking, run the following commands in your terminal:

```bash
# Format the code
autopep8 --in-place --aggressive --agree-with-message --recursive src

# Perform static type checking with Pylint
pylint --rcfile=.pylintrc .
```

## 7. Start the project

To start the project, run the following command:

```bash
uvicorn main:app --reload
```

Now you should be able to see the GDPS API running on your local machine. You can access the API by visiting `http://localhost:8000/docs` in your web browser.

## 8. Create a pull request

After making changes to the forked repository and testing them, you can create a pull request to merge your changes into the main repository. Here's how you can create a pull request:

1. Open your forked repository on GitHub.
2. Click on the "Pull requests" tab in the top-right corner of the page.
3. Click on the "New pull request" button.
4. In the "Compare" dropdown, select "base: main" and "head: <your-branch-name>". Replace `<your-branch-name>` with the name of the branch where you made your changes.
5. Write a clear and concise title for your pull request, describing the changes you made.
6. In the "Write a comment..." text area, provide a detailed description of the changes you made, including any relevant context, motivation, and any potential issues or limitations.
7. Click on the "Create pull request" button to submit your pull request.

Your pull request will now be reviewed by the maintainers of the GDPS API repository. They may ask for additional changes or provide feedback on your contribution. Once your pull request is merged, your changes will be included in the main repository, and you can celebrate your successful contribution to the GDPS API project!

Remember to follow the [contribution guidelines](https://github.com/ak47andrew/GDPSAPI/blob/master/CONTRIBUTING.md) when making changes to the codebase. Happy contributing!
