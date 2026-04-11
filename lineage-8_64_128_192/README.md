# lineage-8_64_128_192
Testing LLM reasoning abilities with lineage relationship quizzes. 

This directory contains [lineage-bench](https://github.com/fairydreaming/lineage-bench) results for lineage-8, lineage-64, lineage-128 and lineage-192 problem sizes.

## Changelog

* 2026-04-11 - Added results for gemma-4-26b-a4b-it, gemma-4-31b-it, glm-5.1 and qwen3.6-plus.
* 2026-03-20 - Added results for minimax-m2.7.
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

![results_stacked](https://github.com/user-attachments/assets/8a0fca78-7aaa-45b7-9354-92612d939a60)

### Table

The table below presents the benchmark results. If not explicitly stated default medium reasoning effort was used during benchmark.

|   Nr | model_name                           |   lineage |   lineage-8 |   lineage-64 |   lineage-128 |   lineage-192 |
|-----:|:-------------------------------------|----------:|------------:|-------------:|--------------:|--------------:|
|    1 | google/gemini-3.1-pro-preview (high) |     1.000 |       1.000 |        1.000 |         1.000 |         1.000 |
|    2 | deepseek/deepseek-v3.2-speciale      |     0.994 |       1.000 |        1.000 |         1.000 |         0.975 |
|    2 | qwen/qwen3.5-397b-a17b               |     0.994 |       1.000 |        1.000 |         0.975 |         1.000 |
|    4 | google/gemma-4-31b-it                |     0.988 |       1.000 |        1.000 |         1.000 |         0.950 |
|    4 | qwen/qwen3.5-plus-02-15              |     0.988 |       1.000 |        1.000 |         0.975 |         0.975 |
|    6 | google/gemini-3-pro-preview          |     0.981 |       1.000 |        1.000 |         0.925 |         1.000 |
|    6 | qwen/qwen3.6-plus                    |     0.981 |       1.000 |        1.000 |         0.975 |         0.950 |
|    8 | openai/gpt-5.1 (high)                |     0.969 |       1.000 |        0.975 |         0.975 |         0.925 |
|    9 | moonshotai/kimi-k2.5                 |     0.963 |       1.000 |        0.975 |         1.000 |         0.875 |
|   10 | openai/gpt-5.2 (xhigh)               |     0.962 |       1.000 |        1.000 |         0.925 |         0.925 |
|   11 | deepseek/deepseek-v3.2               |     0.956 |       1.000 |        1.000 |         0.975 |         0.850 |
|   12 | anthropic/claude-sonnet-4.6 (high)   |     0.956 |       1.000 |        1.000 |         0.925 |         0.900 |
|   13 | qwen/qwen3.5-27b                     |     0.944 |       1.000 |        1.000 |         0.925 |         0.850 |
|   13 | qwen/qwen3-max-thinking              |     0.944 |       1.000 |        0.950 |         0.925 |         0.900 |
|   13 | openai/gpt-5-mini (high)             |     0.944 |       1.000 |        1.000 |         0.875 |         0.900 |
|   13 | anthropic/claude-sonnet-4.5          |     0.944 |       0.975 |        0.975 |         0.900 |         0.925 |
|   17 | volcengine/doubao-seed-2.0-pro       |     0.931 |       1.000 |        0.975 |         0.925 |         0.825 |
|   18 | google/gemini-2.5-pro                |     0.925 |       1.000 |        0.900 |         0.900 |         0.900 |
|   19 | qwen/qwen3.5-122b-a10b               |     0.919 |       1.000 |        0.925 |         0.900 |         0.850 |
|   20 | openai/gpt-5 (high)                  |     0.919 |       1.000 |        1.000 |         0.975 |         0.700 |
|   21 | z-ai/glm-5                           |     0.913 |       1.000 |        0.925 |         0.925 |         0.800 |
|   21 | anthropic/claude-opus-4.6 (high)     |     0.913 |       1.000 |        0.975 |         0.875 |         0.800 |
|   23 | openai/gpt-5.1 (medium)              |     0.888 |       1.000 |        0.950 |         0.875 |         0.725 |
|   24 | openai/gpt-5.4 (xhigh)               |     0.881 |       1.000 |        1.000 |         0.750 |         0.775 |
|   25 | google/gemini-3-flash-preview        |     0.881 |       1.000 |        0.975 |         0.875 |         0.675 |
|   26 | openai/gpt-5.4-mini (xhigh)          |     0.881 |       0.975 |        0.925 |         0.825 |         0.800 |
|   27 | qwen/qwen3.5-35b-a3b                 |     0.875 |       0.975 |        0.925 |         0.925 |         0.675 |
|   27 | openai/gpt-5.4 (high)                |     0.875 |       1.000 |        0.900 |         0.900 |         0.700 |
|   29 | qwen/qwen3-max                       |     0.869 |       1.000 |        0.800 |         0.900 |         0.775 |
|   30 | anthropic/claude-opus-4.5 (medium)   |     0.869 |       1.000 |        0.950 |         0.900 |         0.625 |
|   30 | x-ai/grok-4-fast (medium)            |     0.869 |       1.000 |        0.925 |         0.900 |         0.650 |
|   30 | x-ai/grok-4 (medium)                 |     0.869 |       1.000 |        0.950 |         0.900 |         0.625 |
|   33 | qwen/qwen3-235b-a22b-thinking-2507   |     0.856 |       0.900 |        0.875 |         0.850 |         0.800 |
|   34 | z-ai/glm-5.1                         |     0.850 |       1.000 |        0.800 |         0.875 |         0.725 |
|   35 | inclusionai/ring-1t                  |     0.819 |       0.875 |        0.975 |         0.800 |         0.625 |
|   36 | deepseek/deepseek-v3.1-terminus      |     0.812 |       0.975 |        0.900 |         0.700 |         0.675 |
|   37 | openai/o3 (medium)                   |     0.800 |       1.000 |        0.925 |         0.800 |         0.475 |
|   38 | deepseek/deepseek-v3.2-exp           |     0.794 |       0.975 |        0.900 |         0.700 |         0.600 |
|   39 | anthropic/claude-haiku-4.5           |     0.794 |       0.975 |        0.925 |         0.575 |         0.700 |
|   39 | z-ai/glm-4.7                         |     0.794 |       1.000 |        0.750 |         0.750 |         0.675 |
|   41 | openai/gpt-5 (medium)                |     0.788 |       1.000 |        0.975 |         0.850 |         0.325 |
|   42 | deepseek/deepseek-r1-0528            |     0.787 |       1.000 |        0.975 |         0.650 |         0.525 |
|   43 | google/gemma-4-26b-a4b-it            |     0.775 |       1.000 |        0.975 |         0.725 |         0.400 |
|   44 | bytedance/seed-oss-36b-instruct      |     0.769 |       1.000 |        0.850 |         0.750 |         0.475 |
|   45 | stepfun/step-3.5-flash               |     0.769 |       1.000 |        0.700 |         0.725 |         0.650 |
|   46 | deepcogito/cogito-v2.1-671b          |     0.756 |       0.975 |        0.800 |         0.650 |         0.600 |
|   47 | x-ai/grok-4.1-fast (medium)          |     0.750 |       1.000 |        0.900 |         0.800 |         0.300 |
|   48 | openai/gpt-oss-120b (high)           |     0.731 |       1.000 |        1.000 |         0.725 |         0.200 |
|   49 | baidu/ernie-5.0-thinking-preview     |     0.719 |       1.000 |        0.850 |         0.650 |         0.375 |
|   50 | z-ai/glm-4.5                         |     0.700 |       1.000 |        0.775 |         0.625 |         0.400 |
|   51 | volcengine/doubao-seed-2.0-lite      |     0.694 |       1.000 |        0.875 |         0.650 |         0.250 |
|   52 | z-ai/glm-5-turbo                     |     0.681 |       0.975 |        0.800 |         0.625 |         0.325 |
|   53 | z-ai/glm-4.6                         |     0.644 |       0.925 |        0.725 |         0.525 |         0.400 |
|   54 | xiaomi/mimo-v2-flash                 |     0.600 |       1.000 |        0.900 |         0.425 |         0.075 |
|   55 | prime-intellect/intellect-3          |     0.594 |       1.000 |        0.950 |         0.325 |         0.100 |
|   55 | z-ai/glm-4.5-air                     |     0.594 |       1.000 |        0.750 |         0.450 |         0.175 |
|   57 | minimax/minimax-m2.7                 |     0.588 |       0.975 |        0.725 |         0.450 |         0.200 |
|   58 | openai/gpt-oss-120b (medium)         |     0.581 |       1.000 |        0.875 |         0.375 |         0.075 |
|   58 | minimax/minimax-m2.1                 |     0.581 |       0.950 |        0.725 |         0.450 |         0.200 |
|   60 | minimax/minimax-m2.5                 |     0.581 |       1.000 |        0.825 |         0.350 |         0.150 |
|   61 | qwen/qwen3-next-80b-a3b-thinking     |     0.575 |       0.950 |        0.700 |         0.425 |         0.225 |
|   62 | google/gemini-2.5-flash              |     0.569 |       0.975 |        0.575 |         0.525 |         0.200 |
|   63 | minimax/minimax-m2                   |     0.562 |       0.975 |        0.700 |         0.350 |         0.225 |
|   64 | qwen/qwen3.5-9b                      |     0.556 |       1.000 |        0.775 |         0.275 |         0.175 |
|   65 | moonshotai/kimi-k2-thinking          |     0.525 |       1.000 |        0.850 |         0.200 |         0.050 |
|   65 | amazon/nova-2-lite-v1                |     0.525 |       1.000 |        0.700 |         0.325 |         0.075 |
|   65 | openai/o4-mini (medium)              |     0.525 |       1.000 |        0.775 |         0.300 |         0.025 |
|   68 | volcengine/doubao-seed-1.8           |     0.512 |       1.000 |        0.925 |         0.125 |         0.000 |
|   68 | openai/gpt-5-mini (medium)           |     0.512 |       1.000 |        0.950 |         0.075 |         0.025 |
|   70 | mistralai/mistral-small-2603 (high)  |     0.510 |       0.975 |        0.616 |         0.275 |         0.175 |
|   71 | openai/gpt-oss-20b (high)            |     0.500 |       1.000 |        0.800 |         0.175 |         0.025 |
|   72 | qwen/qwen3-30b-a3b-thinking-2507     |     0.494 |       1.000 |        0.575 |         0.275 |         0.125 |
|   72 | openai/gpt-5.2 (high)                |     0.494 |       1.000 |        0.700 |         0.175 |         0.100 |
|   74 | openai/gpt-5.4-mini (high)           |     0.481 |       1.000 |        0.550 |         0.225 |         0.150 |
|   75 | qwen/qwen3.5-4b                      |     0.469 |       1.000 |        0.650 |         0.175 |         0.050 |
|   76 | openai/gpt-5.2 (medium)              |     0.450 |       1.000 |        0.675 |         0.075 |         0.050 |
|   77 | allenai/olmo-3-32b-think             |     0.444 |       0.925 |        0.600 |         0.175 |         0.075 |
|   78 | nvidia/nemotron-3-super-120b-a12b    |     0.438 |       0.975 |        0.525 |         0.075 |         0.175 |
|   79 | volcengine/doubao-seed-2.0-mini      |     0.431 |       1.000 |        0.675 |         0.025 |         0.025 |
|   80 | mistralai/ministral-14b-2512         |     0.400 |       0.875 |        0.425 |         0.175 |         0.125 |
|   81 | qwen/qwen3-32b                       |     0.362 |       0.950 |        0.475 |         0.025 |         0.000 |
|   82 | z-ai/glm-4.7-flash                   |     0.344 |       0.725 |        0.225 |         0.250 |         0.175 |
|   83 | allenai/olmo-3.1-32b-think           |     0.312 |       0.950 |        0.275 |         0.025 |         0.000 |
|   84 | openai/gpt-oss-20b (medium)          |     0.306 |       1.000 |        0.200 |         0.025 |         0.000 |
|   85 | openai/gpt-5-nano (medium)           |     0.294 |       1.000 |        0.150 |         0.025 |         0.000 |
|   86 | upstage/solar-pro-3 (high)           |     0.288 |       0.700 |        0.275 |         0.075 |         0.100 |
|   87 | openai/o3-mini (medium)              |     0.287 |       0.950 |        0.200 |         0.000 |         0.000 |
|   88 | upstage/solar-pro-3 (medium)         |     0.281 |       0.725 |        0.225 |         0.100 |         0.075 |
|   89 | nvidia/nemotron-3-nano-30b-a3b       |     0.231 |       0.875 |        0.025 |         0.025 |         0.000 |

Each row contains the average benchmark score across all problem sizes, and separate scores for each problem size.
