# House Price Predictor
Final project for the Building AI course project by Reaktor and University of Helsinki

## Summary
This project uses a simple feedforward neural network to predict house prices from structured input features like square footage, number of rooms, and location data. It demonstrates how AI can model real-world patterns in housing markets. Building AI course project

![image of an online cat](https://tinyurl.com/elementsofaicat)

## Background
Real estate pricing can be inconsistent and difficult to assess due to the many variables involved. Manually estimating fair prices often leads to bias or missed value.

This project aims to address:

Inconsistent housing market pricing

Biases in manual valuation

Difficulty in forecasting home prices

I chose this topic because I’m passionate about using AI for practical, high-impact applications. Property decisions are major life choices—accurate predictions help make them fairer.

How is it used?
The model takes numeric input features such as:

Square meters

Bedrooms

Bathrooms

Age of property

Lot size

It outputs a predicted market price.

Users include:

Buyers estimating a home’s worth before making offers

Real estate professionals automating their valuation process

Data analysts researching market trends

<img src="https://upload.wikimedia.org/wikipedia/commons/a/ae/House_diagram.jpg" width="300">
Data sources and AI methods
Data was synthetically generated to simulate real-world home features and pricing patterns.

AI methods:

Fully connected neural network with 2 hidden layers

ReLU activation functions

Linear output layer for regression

Example forward pass:

ini
Copy
Edit
h1 = np.maximum(0, np.dot(x, w0) + b0)
h2 = np.maximum(0, np.dot(h1, w1) + b1)
out = np.dot(h2, w2) + b2
Challenges
This model does not:

Use real-world datasets (yet)

Account for market seasonality, school zones, or economic factors

Guarantee generalization to other geographic regions

Ethical considerations:

Must avoid reinforcing socioeconomic bias

Should explain predictions clearly to users

What next?
Future improvements:

Use real housing datasets (e.g., Zillow)

Improve architecture with dropout or regularization

Deploy with a web interface

Add interpretability tools like SHAP or LIME

I’d benefit from:

Collaboration with data engineers for pipeline building

Access to large, anonymized housing datasets

Acknowledgments
Inspired by the Building AI course by Reaktor and the University of Helsinki

Image: House Diagram / CC BY-SA 3.0

Thanks to NumPy and Python for enabling fast prototyping
