# Project setup

Create an .env file with the following text:
```
ROBOFLOW_API_KEY="YOUR KEY HERE"
```

Next, setup python libraries:
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

Then running the script depends on IDE. If you want to run it in terminal you can use:
```bash
pip install nbconvert
jupyter nbconvert --to notebook --execute Main.ipynb --output Main_Run.ipynb
```

# Project description

This is a machine learning project that classifies photos of junk into six categories: glass, metal, plastic, cardboard, paper and trash. Trash is everything not recognized as the other categories.

The project can be ran either with a backbone or without it. With backbone it achieves ~86 average f1 score and without it ~64.
