# Example of Regression Learning Models

## Usage
### API
```
payload = '
    {
        "freedom" : 0.616,
        "dystopia_residual" : 0.537,
        "internet_access_population[%]" : 0.516,
        "cellular_subscriptions" : 0.535,
        "familiy_income_gini_coeff" : 0.453,
        "GDP_per_capita[$]" : 0.547,
        "inflation_rate[%]" : 0.244,
        "military_expenditures[%]" : 0.586,
        "population"  : 0.437
    }'

echo $payload | curl \
    --header "Content-Type: application/json" \
    --request POST \
    --data @-\
    http://172.24.236.2:9696/score

unset payload
```