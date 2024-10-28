

```bash
# start vllm
CUDA_VISIBLE_DEVICES=0 vllm serve meta-llama/Meta-Llama-3.1-8B-Instruct --dtype auto --api-key token-abc123 --port 17000 &
CUDA_VISIBLE_DEVICES=1 vllm serve meta-llama/Meta-Llama-3.1-8B-Instruct --dtype auto --api-key token-abc123 --port 17001 &

# 在code中指定
python run_with_earlystopping.py
```

