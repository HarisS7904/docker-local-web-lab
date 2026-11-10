# What's include in it and why?
```text
- .git	         # Git history isn't needed inside Docker image
- .gitignore	 # Git configuration isn't needed by the application
- .env	         # May contain passwords, API keys or other sensitive values
- .env.*	 # Excludes environment-specific files such as .env.local
- !.env.example	 # Allows a safe example configuration file to remain available.
- __pycache__/	 # Excludes Python's generated cache files
- *.pyc	         # Excludes compiled Python bytecode
- .venv/	 # Excludes Python local virtual environment
- .vscode/	 # Excludes VS Code workspace settings
```


