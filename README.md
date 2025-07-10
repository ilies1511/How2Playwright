# create venv
python3 -m venv venv

# go to venv
source venv/bin/activate

# install lib
pip install playwright

# install browser

playwright install chromium

# generate code automatically
playwright codegen \
 --browser=chromium \
 --target=python \
 --output=recorded_script.py http://localhost:5173/
