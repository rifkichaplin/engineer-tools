# Prometheus

## Documentation
- Website [https://prometheus.io/docs/introduction/overview/]
- Github [https://github.com/cloudalchemy/ansible-prometheus]

## How to Run
- virtualenv -p python3 venv_prometheus
- source venv_prometheus/bin/activate
- pip install ansible==2.9.9
- brew install gnu-tar #just for mac as deployer
- export OBJC_DISABLE_INITIALIZE_FORK_SAFETY=YES #just for mac as deployer
- mkdir -p roles/prometheus
- git clone https://github.com/cloudalchemy/ansible-prometheus.git roles/prometheus
- vagrant up (first booting up) or vagrant provision

## How to Access
- http://localhost:9090

