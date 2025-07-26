restaurant-website/
│
├── app.py
├── templates/
│   └── home.html
from flask import Flask, render_template

app = Flask(__name__)

@app.route('/')
def home():
    return render_template('home.html')

if __name__ == '__main__':
    app.run(debug=True)
<!DOCTYPE html>
<html>
<head>
    <title>Welcome to Our Restaurant</title>
</head>
<body>
    <h1>Welcome to Mama's Kitchen!</h1>
    <p>Serving love on every plate.</p>
</body>
</html>
python app.py
