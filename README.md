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

## TODO

- [ ] **luffy/deepscaler/utils.py** - Implement full Gemini API integration (currently a placeholder)
  - [ ] Implement Vertex AI initialization and authentication
  - [ ] Configure safety settings for content generation
  - [ ] Set up GenerativeModel with proper system instructions
  - [ ] Implement retry logic with exponential backoff
  - [ ] Add comprehensive error handling for API access issues
  - [ ] Handle rate limiting and quota management
  - [ ] Implement response validation and text extraction
  - [ ] Add support for different generation configurations
- [ ] **luffy/deepscaler/utils.py** - Add logging for OpenAI API calls and errors
- [ ] **luffy/deepscaler/utils.py** - Support batch processing for multiple prompts
- [ ] **luffy/deepscaler/utils.py** - Add timeout configuration for API calls

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