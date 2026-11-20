# LUFFY Development Repository

> 🚧 **Development Branch** - This is the main development repository for LUFFY (Learning to Reason Under Off‑Policy Guidance)

## About LUFFY

LUFFY is a reinforcement learning framework focused on learning reasoning under off-policy guidance. This repository contains the core implementation, training pipelines, and evaluation tools.

## Current Status

✅ **Recently Completed:**
- OpenAI API client with retry logic and exponential backoff for rate limits
- RAG (Retrieval Augmented Generation) module using sentence-transformers
- Reward type definitions, config dataclasses, and abstract RewardFn base class
- Math answer verification with sympy-based expression normalization and comparison
- DeepScaler dataset preparation script (produces train/val parquet files)
- OpenR1-Math dataset preparation with filtering and length-based truncation
- GRPO training scripts for DeepScaler 1.5B (8k and 16k response lengths)
- vLLM-based evaluation script supporting multiple math benchmarks
- LUFFY off-policy training script with prefix-sharing and off-policy loss
- Results collection utility that aggregates benchmark scores into Excel

## Complete TODO List

- [ ] **luffy/deepscaler/utils.py:47** - Add logging for API calls and errors
- [ ] **luffy/deepscaler/utils.py:48** - Support batch processing for multiple prompts
- [ ] **luffy/deepscaler/utils.py:49** - Add timeout configuration for API calls
- [ ] **luffy/deepscaler/utils.py:53** - Implement Vertex AI initialization and authentication
- [ ] **luffy/deepscaler/utils.py:54** - Configure safety settings for content generation
- [ ] **luffy/deepscaler/utils.py:55** - Set up GenerativeModel with proper system instructions
- [ ] **luffy/deepscaler/utils.py:56** - Implement retry logic with exponential backoff
- [ ] **luffy/deepscaler/utils.py:57** - Add comprehensive error handling for API access issues
- [ ] **luffy/deepscaler/utils.py:58** - Handle rate limiting and quota management
- [ ] **luffy/deepscaler/utils.py:59** - Implement response validation and text extraction
- [ ] **luffy/deepscaler/utils.py:60** - Add support for different generation configurations

## Development Setup

```bash
git clone https://github.com/FastGuideHarbor/LUFFY.git
cd LUFFY
git checkout dev
pip install -e .
```

## License

MIT

---

*This README was auto-updated based on recent dev branch changes*

Co-authored-by: Claude <noreply@anthropic.com>