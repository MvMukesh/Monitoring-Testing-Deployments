<div align="center"> 
&nbsp;&nbsp;&nbsp;&nbsp;
<a href="https://www.linkedin.com/in/mukesh-manral/"><img src="https://img.shields.io/badge/LinkedIn-411AFF?style=for-the-badge&logo=LinkedIn&logoColor=white" /></a>  
&nbsp;&nbsp;&nbsp;&nbsp;
<a href="https://www.kaggle.com/mukeshmanral"><img src="https://img.shields.io/badge/Kaggle-411AFF?style=for-the-badge&logo=Kaggle&logoColor=white" /></a>
&nbsp;&nbsp;&nbsp;&nbsp;
<a href="https://medium.com/@manralai/lists"><img src="https://img.shields.io/badge/Medium-411AFF?style=for-the-badge&logo=Medium&logoColor=white" /></a>
&nbsp;&nbsp;&nbsp;&nbsp;
<a href="https://www.youtube.com/@manralai"><img src="https://img.shields.io/badge/Youtube-411AFF?style=for-the-badge&logo=Youtube&logoColor=white" /></a>
&nbsp;&nbsp;&nbsp;&nbsp; 
<a href="https://www.instagram.com/manralai/"><img src="https://img.shields.io/badge/Instagram-411AFF?style=for-the-badge&logo=Instagram&logoColor=white" /></a>
</div>

# Monitoring and Testing Machine Learning Deployments
[![GitHub Issues](https://img.shields.io/github/issues/MvMukesh/Monitoring-N-Testing-Deployments.svg) ![GitHub followers](https://img.shields.io/github/followers/MvMukesh.svg?style=social\&label=Follow\&maxAge=2592000)](https://github.com/MvMukesh?tab=followers) [![GitHub forks](https://img.shields.io/github/forks/MvMukesh/Monitoring-N-Testing-Deployments.svg?style=social\&label=Fork\&maxAge=2592000)](https://github.com/MvMukesh/Monitoring-N-Testing-Deployments/network/) [![GitHub stars](https://img.shields.io/github/stars/MvMukesh/Monitoring-N-Testing-Deployments.svg?style=social\&label=Star\&maxAge=2592000)](https://github.com/MvMukesh/Monitoring-N-Testing-Deployments/stargazers/)

**`ML pipelines setup plus automated CI/CD routines`**

![mlops_cicd](https://user-images.githubusercontent.com/26667491/221462199-e714ae80-c84f-4398-a468-df4a04c574ac.png)


# Tree

<pre>
.
├── README.md
├── exercise_env
│   ├── docker_exercise
│   │   ├── Dockerfile
│   │   ├── app.py
│   │   ├── docker-compose.yml
│   │   └── requirements.txt
│   ├── elk_exercise
│   │   ├── Dockerfile
│   │   ├── app
│   │   │   ├── __init__.py
│   │   │   └── flask_app.py
│   │   ├── application.py
│   │   ├── docker-compose.yml
│   │   ├── elasticsearch
│   │   │   └── config
│   │   │       └── elasticsearch.yml
│   │   ├── gunicorn_logging.conf
│   │   ├── kibana
│   │   │   └── config
│   │   │       └── kibana.yml
│   │   ├── logstash
│   │   │   ├── config
│   │   │   │   └── logstash.yml
│   │   │   └── pipeline
│   │   │       └── logstash.conf
│   │   └── requirements.txt
│   ├── prometheus_exercise
│   │   ├── Dockerfile
│   │   ├── app
│   │   │   ├── __init__.py
│   │   │   ├── flask_app.py
│   │   │   └── helpers
│   │   │       ├── __init__.py
│   │   │       └── middleware.py
│   │   ├── application.py
│   │   ├── config
│   │   │   ├── grafana
│   │   │   │   ├── basic_cadvisor_dashboard.json
│   │   │   │   └── grafana_flask_basic_dashboard.json
│   │   │   └── prometheus
│   │   │       └── prometheus.yml
│   │   ├── docker-compose.yml
│   │   └── requirements.txt
│   ├── shadow_mode_exercise
│   │   ├── assessing_model_results.ipynb
│   │   └── requirements.txt
│   ├── unit_testing_exercise
│   │   ├── requirements.txt
│   │   ├── unit_testing_data_engineering.ipynb
│   │   ├── unit_testing_input_data.ipynb
│   │   ├── unit_testing_model_configuration.ipynb
│   │   └── unit_testing_model_predictions_quality.ipynb
│   └── utility_scripts
│       └── MapPortsForDocker.cmd
├── packages
│   ├── gradient_boosting_model
│   │   ├── MANIFEST.in
│   │   ├── gradient_boosting_model
│   │   │   ├── VERSION
│   │   │   ├── __init__.py
│   │   │   ├── config
│   │   │   │   ├── __init__.py
│   │   │   │   └── core.py
│   │   │   ├── config.yml
│   │   │   ├── datasets
│   │   │   │   └── __init__.py
│   │   │   ├── pipeline.py
│   │   │   ├── predict.py
│   │   │   ├── processing
│   │   │   │   ├── __init__.py
│   │   │   │   ├── data_management.py
│   │   │   │   ├── errors.py
│   │   │   │   ├── preprocessors.py
│   │   │   │   └── validation.py
│   │   │   ├── train_pipeline.py
│   │   │   └── trained_models
│   │   │       └── __init__.py
│   │   ├── mypy.ini
│   │   ├── requirements.txt
│   │   ├── setup.py
│   │   ├── test_requirements.txt
│   │   ├── tests
│   │   │   ├── __init__.py
│   │   │   ├── conftest.py
│   │   │   ├── test_config.py
│   │   │   ├── test_pipeline.py
│   │   │   ├── test_predict.py
│   │   │   ├── test_preprocessors.py
│   │   │   └── test_validation.py
│   │   └── tox.ini
│   └── ml_api
│       ├── Makefile
│       ├── __init__.py
│       ├── alembic
│       │   ├── env.py
│       │   ├── script.py.mako
│       │   └── versions
│       │       └── cf4abb13368d_create_prediction_tables.py
│       ├── alembic.ini
│       ├── api
│       │   ├── __init__.py
│       │   ├── app.py
│       │   ├── config.py
│       │   ├── controller.py
│       │   ├── monitoring
│       │   │   ├── __init__.py
│       │   │   └── middleware.py
│       │   ├── persistence
│       │   │   ├── __init__.py
│       │   │   ├── core.py
│       │   │   ├── data_access.py
│       │   │   └── models.py
│       │   └── spec
│       │       ├── __init__.py
│       │       └── api.yaml
│       ├── differential_tests
│       │   ├── __init__.py
│       │   ├── __main__.py
│       │   ├── compare.py
│       │   └── sample_payloads
│       │       └── sample_input1.json
│       ├── docker
│       │   ├── Dockerfile
│       │   ├── Dockerfile.test
│       │   ├── config
│       │   │   ├── grafana
│       │   │   │   ├── basic_cadvisor_dashboard_ml_api.json
│       │   │   │   ├── grafana_flask_basic_dashboard_ml_api.json
│       │   │   │   └── ml_api_dashboard.json
│       │   │   └── prometheus
│       │   │       └── prometheus.yml
│       │   ├── docker-compose-ci-candidate.yml
│       │   ├── docker-compose-ci-master.yml
│       │   ├── docker-compose-elk.yml
│       │   ├── docker-compose.test.yml
│       │   ├── docker-compose.yml
│       │   ├── elasticsearch
│       │   │   └── config
│       │   │       └── elasticsearch.yml
│       │   ├── kibana
│       │   │   └── config
│       │   │       ├── kibana.yml
│       │   │       └── kibana_example_inputs_dashboard.ndjson
│       │   ├── logstash
│       │   │   ├── config
│       │   │   │   └── logstash.yml
│       │   │   └── pipeline
│       │   │       └── logstash.conf
│       │   └── workaround_32_os
│       │       ├── Dockerfile.workaround
│       │       └── docker-compose-workaround.yml
│       ├── gunicorn_logging.conf
│       ├── mypy.ini
│       ├── requirements
│       │   ├── requirements.txt
│       │   └── test_requirements.txt
│       ├── run.py
│       ├── scripts
│       │   ├── differential_tests.sh
│       │   └── populate_database.py
│       ├── tests
│       │   ├── __init__.py
│       │   ├── conftest.py
│       │   ├── test_api.py
│       │   ├── test_back_to_back_models.py
│       │   └── test_persistence.py
│       └── tox.ini
└── research_env
    ├── gradient_boosting_model.ipynb
    └── requirements.txt
</pre>

<p align="center">
  <kbd><img src="https://user-images.githubusercontent.com/26667491/221332315-4716d85d-6e4b-4493-a363-94302d376163.png" alt="ml_lifecycle.png"></kbd>
</p>

## Resources
* [Google Cloud Architecture Center](https://cloud.google.com/architecture/mlops-continuous-delivery-and-automation-pipelines-in-machine-learning)
* [Google ML](https://developers.google.com/machine-learning)
