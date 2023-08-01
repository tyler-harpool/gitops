# k8gpt + local AI
Give your Kubernetes cluster a brain.

## Install k8gpt cli
- Setup auth for localai: `k8sgpt auth add --backend localai --model ggml-gpt4all-j --baseurl http://localhost:8080/v1`
- Set default provider: `k8sgpt auth default -p localai`
## Usage
- `k8sgpt analyze --explain --backend localai`
## Resources 
- [k8gtp-operator in k8 guide](https://github.com/k8sgpt-ai/k8sgpt-operator)

## Run a test
`curl http://local-ai.local-ai.svc.cluster.local:8080/v1/completions -H "Content-Type: application/json" -d '{"model": "ggml-gpt4all-j.bin", "prompt": "A long time ago in a galaxy far, far away", "temperature": 0.7}'`