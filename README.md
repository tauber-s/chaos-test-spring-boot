# Chaos Testing Demo Spring Boot
This is an example project prepared for demonstrating Chaos Engineering experiment on a Spring boot application using Chaos Monkey and Chaos Toolkit

## REST endpoints
- `/employees/` - Return list of employees
- `/actuator/chaosmonkey` - Chaos Monkey for Spring Boot
- `/swagger-ui/index.html` - Swagger UI


## Chaos Experiments
Set virtual environment in python and install `chaostoolkit-spring`
```
python3 -m venv ~/.venvs/chaostk
source  ~/.venvs/chaostk/bin/activate
pip install chaostoolkit
pip install chaostoolkit-spring
```
Run the experiment:
`chaos run experiments/experiments.json --journal-path=experiments/journal.json`