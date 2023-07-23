## k8gpt + local AI
Give your Kubernetes cluster a brain.

## Install k8gpt cli
- Setup auth for localai: `k8sgpt auth add --backend localai --model ggml-gpt4all-j --baseurl http://localhost:8080/v1`
- Set default provider: `k8sgpt auth default -p localai`
## Usage
- ``k8sgpt analyze --explain --backend localai`
## Resources 
- [k8gtp-operator in k8 guide](https://github.com/k8sgpt-ai/k8sgpt-operator)