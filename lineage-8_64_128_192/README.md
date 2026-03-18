# lineage-8_64_128_192
Testing LLM reasoning abilities with lineage relationship quizzes. 

This directory contains [lineage-bench](https://github.com/fairydreaming/lineage-bench) results for lineage-8, lineage-64, lineage-128 and lineage-192 problem sizes.

## Changelog

* 2026-03-18 - Added results for gpt-5-mini (high) and gpt-5.4-mini (high, xhigh).
* 2026-03-17 - Added results for mistral-small-2603.
* 2026-03-16 - Added results for glm-5-turbo.
* 2026-03-13 - Added results for nemotron-3-super-120b-a12b.
* 2026-03-07 - Added missing result for gpt-5 (high).
* 2026-03-06 - Added results for gpt-5.4 (high/xhigh).
* 2026-03-02 - Added results for qwen3.5-4b and qwen3.5-9b.
* 2026-03-01 - Added results for claude-opus-4.6 (high).
* 2026-02-26 - Added results for qwen3.5-27b, qwen3.5-35b-a3b and qwen3.5-122b-a10b.
* 2026-02-19 - Added results for claude-sonnet-4.6 (high) and gemini-3.1-pro-preview (high).
* 2026-02-16 - Added results for qwen3.5-397b-a17b and qwen3.5-plus-02-15.
* 2026-02-15 - Added results for doubao-seed-2.0-mini, doubao-seed-2.0-lite and doubao-seed-2.0-pro.
* 2026-02-13 - Added results for qwen3-max-thinking, glm-5 and minimax-m2.5.
* 2026-02-08 - Added results for gpt-oss-20b (medium, high).
* 2026-02-03 - Added results for solar-pro-3 (medium, high) and step-3.5-flash.
* 2026-01-27 - Added results for gpt-5.2 xhigh and kimi-k2.5. Retested gpt-oss-120b with explicit medium and high reasoning effort.
* 2026-01-24 - Added results for glm-4.7, glm-4.7-flash, minimax-m2.1 and olmo-3.1-32b-think.
* 2025-12-18 - Added results for some legacy models (gemini-2.5-flash, gemini-2.5-pro), for high reasoning effort (gpt-5.1, gpt-5.2) and other recently released models (nemotron-3-nano-30b-a3b, doubao-seed-1-8, gemini-3-flash-preview, mimo-v2-flash, ministral-14b-2512). Stacked results plot shows only top 30 scores now.
* 2025-12-03 - Updated results for ring-1t model. Added results for seed-oss-36b-instruct (courtesy of [@mokieli](https://github.com/mokieli)).
* 2025-12-01 - Added results for ring-1t, deepseek-r1-0528, glm-4.5-air, glm-4.5, intellect-3, ernie-5.0-thinking-preview, deepseek-v3.2 and deepseek-v3.2-speciale. Updated results for glm-4.6 (works better with lower temperature). Results for ring-1t are not final (problems with model provider).
* 2025-11-25 - Added results for gpt-5.1, claude-opus-4.5, grok-4.1-fast and o4-mini.
* 2025-11-23 - Added results for qwen3-32b, o3-mini and o3 models.
* 2025-11-22 - Updated results to include recently released models, but only with 40 quizzes per problem size to reduce costs.

## Results

### Plot

The plot below shows only the 30 top-performing models. See the table for all results.

![results_stacked](https://github.com/user-attachments/assets/17319b50-a0e3-4a67-a067-ac420f422416)

### Table

The table below presents the benchmark results. If not explicitly stated default medium reasoning effort was used during benchmark.

|   Nr | model_name                         |   lineage |   lineage-8 |   lineage-64 |   lineage-128 |   lineage-192 |
|-----:|:-----------------------------------|----------:|------------:|-------------:|--------------:|--------------:|
|    1 | google/gemini-3.1-pro-preview (high) |     1.000 |       1.000 |        1.000 |         1.000 |         1.000 |
|    2 | deepseek/deepseek-v3.2-speciale      |     0.994 |       1.000 |        1.000 |         1.000 |         0.975 |
|    2 | qwen/qwen3.5-397b-a17b               |     0.994 |       1.000 |        1.000 |         0.975 |         1.000 |
|    4 | qwen/qwen3.5-plus-02-15              |     0.988 |       1.000 |        1.000 |         0.975 |         0.975 |
|    5 | google/gemini-3-pro-preview          |     0.981 |       1.000 |        1.000 |         0.925 |         1.000 |
|    6 | openai/gpt-5.1 (high)                |     0.969 |       1.000 |        0.975 |         0.975 |         0.925 |
|    7 | moonshotai/kimi-k2.5                 |     0.963 |       1.000 |        0.975 |         1.000 |         0.875 |
|    8 | openai/gpt-5.2 (xhigh)               |     0.962 |       1.000 |        1.000 |         0.925 |         0.925 |
|    9 | deepseek/deepseek-v3.2               |     0.956 |       1.000 |        1.000 |         0.975 |         0.850 |
|   10 | anthropic/claude-sonnet-4.6 (high)   |     0.956 |       1.000 |        1.000 |         0.925 |         0.900 |
|   11 | anthropic/claude-sonnet-4.5          |     0.944 |       0.975 |        0.975 |         0.900 |         0.925 |
|   11 | qwen/qwen3-max-thinking              |     0.944 |       1.000 |        0.950 |         0.925 |         0.900 |
|   11 | openai/gpt-5-mini (high)             |     0.944 |       1.000 |        1.000 |         0.875 |         0.900 |
|   11 | qwen/qwen3.5-27b                     |     0.944 |       1.000 |        1.000 |         0.925 |         0.850 |
|   15 | volcengine/doubao-seed-2.0-pro       |     0.931 |       1.000 |        0.975 |         0.925 |         0.825 |
|   16 | google/gemini-2.5-pro                |     0.925 |       1.000 |        0.900 |         0.900 |         0.900 |
|   17 | qwen/qwen3.5-122b-a10b               |     0.919 |       1.000 |        0.925 |         0.900 |         0.850 |
|   18 | openai/gpt-5 (high)                  |     0.919 |       1.000 |        1.000 |         0.975 |         0.700 |
|   19 | anthropic/claude-opus-4.6 (high)     |     0.913 |       1.000 |        0.975 |         0.875 |         0.800 |
|   19 | z-ai/glm-5                           |     0.913 |       1.000 |        0.925 |         0.925 |         0.800 |
|   21 | openai/gpt-5.1 (medium)              |     0.888 |       1.000 |        0.950 |         0.875 |         0.725 |
|   22 | openai/gpt-5.4 (xhigh)               |     0.881 |       1.000 |        1.000 |         0.750 |         0.775 |
|   23 | google/gemini-3-flash-preview        |     0.881 |       1.000 |        0.975 |         0.875 |         0.675 |
|   24 | openai/gpt-5.4-mini (xhigh)          |     0.881 |       0.975 |        0.925 |         0.825 |         0.800 |
|   25 | openai/gpt-5.4 (high)                |     0.875 |       1.000 |        0.900 |         0.900 |         0.700 |
|   25 | qwen/qwen3.5-35b-a3b                 |     0.875 |       0.975 |        0.925 |         0.925 |         0.675 |
|   27 | qwen/qwen3-max                       |     0.869 |       1.000 |        0.800 |         0.900 |         0.775 |
|   28 | x-ai/grok-4-fast (medium)            |     0.869 |       1.000 |        0.925 |         0.900 |         0.650 |
|   28 | x-ai/grok-4 (medium)                 |     0.869 |       1.000 |        0.950 |         0.900 |         0.625 |
|   28 | anthropic/claude-opus-4.5 (medium)   |     0.869 |       1.000 |        0.950 |         0.900 |         0.625 |
|   31 | qwen/qwen3-235b-a22b-thinking-2507   |     0.856 |       0.900 |        0.875 |         0.850 |         0.800 |
|   32 | inclusionai/ring-1t                  |     0.819 |       0.875 |        0.975 |         0.800 |         0.625 |
|   33 | deepseek/deepseek-v3.1-terminus      |     0.812 |       0.975 |        0.900 |         0.700 |         0.675 |
|   34 | openai/o3 (medium)                   |     0.800 |       1.000 |        0.925 |         0.800 |         0.475 |
|   35 | deepseek/deepseek-v3.2-exp           |     0.794 |       0.975 |        0.900 |         0.700 |         0.600 |
|   36 | z-ai/glm-4.7                         |     0.794 |       1.000 |        0.750 |         0.750 |         0.675 |
|   36 | anthropic/claude-haiku-4.5           |     0.794 |       0.975 |        0.925 |         0.575 |         0.700 |
|   38 | openai/gpt-5 (medium)                |     0.788 |       1.000 |        0.975 |         0.850 |         0.325 |
|   39 | deepseek/deepseek-r1-0528            |     0.787 |       1.000 |        0.975 |         0.650 |         0.525 |
|   40 | bytedance/seed-oss-36b-instruct      |     0.769 |       1.000 |        0.850 |         0.750 |         0.475 |
|   41 | stepfun/step-3.5-flash               |     0.769 |       1.000 |        0.700 |         0.725 |         0.650 |
|   42 | deepcogito/cogito-v2.1-671b          |     0.756 |       0.975 |        0.800 |         0.650 |         0.600 |
|   43 | x-ai/grok-4.1-fast (medium)          |     0.750 |       1.000 |        0.900 |         0.800 |         0.300 |
|   44 | openai/gpt-oss-120b (high)           |     0.731 |       1.000 |        1.000 |         0.725 |         0.200 |
|   45 | baidu/ernie-5.0-thinking-preview     |     0.719 |       1.000 |        0.850 |         0.650 |         0.375 |
|   46 | z-ai/glm-4.5                         |     0.700 |       1.000 |        0.775 |         0.625 |         0.400 |
|   47 | volcengine/doubao-seed-2.0-lite      |     0.694 |       1.000 |        0.875 |         0.650 |         0.250 |
|   48 | z-ai/glm-5-turbo                     |     0.681 |       0.975 |        0.800 |         0.625 |         0.325 |
|   49 | z-ai/glm-4.6                         |     0.644 |       0.925 |        0.725 |         0.525 |         0.400 |
|   50 | xiaomi/mimo-v2-flash                 |     0.600 |       1.000 |        0.900 |         0.425 |         0.075 |
|   51 | z-ai/glm-4.5-air                     |     0.594 |       1.000 |        0.750 |         0.450 |         0.175 |
|   51 | prime-intellect/intellect-3          |     0.594 |       1.000 |        0.950 |         0.325 |         0.100 |
|   53 | openai/gpt-oss-120b (medium)         |     0.581 |       1.000 |        0.875 |         0.375 |         0.075 |
|   53 | minimax/minimax-m2.1                 |     0.581 |       0.950 |        0.725 |         0.450 |         0.200 |
|   55 | minimax/minimax-m2.5                 |     0.581 |       1.000 |        0.825 |         0.350 |         0.150 |
|   56 | qwen/qwen3-next-80b-a3b-thinking     |     0.575 |       0.950 |        0.700 |         0.425 |         0.225 |
|   57 | google/gemini-2.5-flash              |     0.569 |       0.975 |        0.575 |         0.525 |         0.200 |
|   58 | minimax/minimax-m2                   |     0.562 |       0.975 |        0.700 |         0.350 |         0.225 |
|   59 | qwen/qwen3.5-9b                      |     0.556 |       1.000 |        0.775 |         0.275 |         0.175 |
|   60 | openai/o4-mini (medium)              |     0.525 |       1.000 |        0.775 |         0.300 |         0.025 |
|   60 | amazon/nova-2-lite-v1                |     0.525 |       1.000 |        0.700 |         0.325 |         0.075 |
|   60 | moonshotai/kimi-k2-thinking          |     0.525 |       1.000 |        0.850 |         0.200 |         0.050 |
|   63 | volcengine/doubao-seed-1.8           |     0.512 |       1.000 |        0.925 |         0.125 |         0.000 |
|   63 | openai/gpt-5-mini (medium)           |     0.512 |       1.000 |        0.950 |         0.075 |         0.025 |
|   65 | mistralai/mistral-small-2603 (high)  |     0.510 |       0.975 |        0.616 |         0.275 |         0.175 |
|   66 | openai/gpt-oss-20b (high)            |     0.500 |       1.000 |        0.800 |         0.175 |         0.025 |
|   67 | qwen/qwen3-30b-a3b-thinking-2507     |     0.494 |       1.000 |        0.575 |         0.275 |         0.125 |
|   67 | openai/gpt-5.2 (high)                |     0.494 |       1.000 |        0.700 |         0.175 |         0.100 |
|   69 | openai/gpt-5.4-mini (high)           |     0.481 |       1.000 |        0.550 |         0.225 |         0.150 |
|   70 | qwen/qwen3.5-4b                      |     0.469 |       1.000 |        0.650 |         0.175 |         0.050 |
|   71 | openai/gpt-5.2 (medium)              |     0.450 |       1.000 |        0.675 |         0.075 |         0.050 |
|   72 | allenai/olmo-3-32b-think             |     0.444 |       0.925 |        0.600 |         0.175 |         0.075 |
|   73 | nvidia/nemotron-3-super-120b-a12b    |     0.438 |       0.975 |        0.525 |         0.075 |         0.175 |
|   74 | volcengine/doubao-seed-2.0-mini      |     0.431 |       1.000 |        0.675 |         0.025 |         0.025 |
|   75 | mistralai/ministral-14b-2512         |     0.400 |       0.875 |        0.425 |         0.175 |         0.125 |
|   76 | qwen/qwen3-32b                       |     0.362 |       0.950 |        0.475 |         0.025 |         0.000 |
|   77 | z-ai/glm-4.7-flash                   |     0.344 |       0.725 |        0.225 |         0.250 |         0.175 |
|   78 | allenai/olmo-3.1-32b-think           |     0.312 |       0.950 |        0.275 |         0.025 |         0.000 |
|   79 | openai/gpt-oss-20b (medium)          |     0.306 |       1.000 |        0.200 |         0.025 |         0.000 |
|   80 | openai/gpt-5-nano (medium)           |     0.294 |       1.000 |        0.150 |         0.025 |         0.000 |
|   81 | upstage/solar-pro-3 (high)           |     0.288 |       0.700 |        0.275 |         0.075 |         0.100 |
|   82 | openai/o3-mini (medium)              |     0.287 |       0.950 |        0.200 |         0.000 |         0.000 |
|   83 | upstage/solar-pro-3 (medium)         |     0.281 |       0.725 |        0.225 |         0.100 |         0.075 |
|   84 | nvidia/nemotron-3-nano-30b-a3b       |     0.231 |       0.875 |        0.025 |         0.025 |         0.000 |

Each row contains the average benchmark score across all problem sizes, and separate scores for each problem size.
