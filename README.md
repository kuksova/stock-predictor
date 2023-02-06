# stock-predictor

Deploying a stock prediction model as a RESTful API using FastAPI to AWS EC2, and make it available (i.e., public) to end users. Less focus is put on how well the model performs, yet the goal is to get an initial working system quickly into production:

data -> model -> API -> deployment


To run the predictions:

curl \
--header "Content-Type: application/json" \
--request POST \
--data '{"ticker":"MSFT", "days":7}' \
http://54.200.241.2:8000/predict
