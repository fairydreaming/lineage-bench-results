# lineage-8_16_32_64
Testing LLM reasoning abilities with lineage relationship quizzes.

This directory contains lineage-bench results for lineage-8, lineage-16, lineage-32 and lineage-64 problem sizes.

## Changelog

* 2024-03-07 - Added results for qwq-32b (used Parasail provider with 0.01 temp, observed some infinite loop generations, but mostly for lineage-64 where the model performs bad anyway).
* 2024-03-04 - Updated results for perplexity/r1-1776. (apparently there was a problem with the model serving stack, that's why r1-1776 initially performed worse than expected)
* 2024-02-26 - Added results for claude-3.7-sonnet (also with :thinking) and r1-1776
* 2024-02-20 - Updated results for deepseek/deepseek-r1-distill-llama-70b. (used Groq provider with 0.5 temperature)
* 2024-02-18 - Added results for kimi-k1.5-preview and llama-3.1-tulu-3-405b.
* 2024-02-06 - Added results for o1, o3-mini, qwen-max, gemini-exp-1206, deepseek-r1-distill-qwen-14b and deepseek-r1-distill-qwen-32b.
* 2024-01-24 - Added results for deepseek-r1-distill-llama-70b.
* 2024-01-20 - Added results for deepseek-r1.
* 2024-01-15 - Added results for deepseek-v3, gemini-2.0-flash-exp, gemini-2.0-flash-thinking-exp-1219 and minimax-01.

## Results

### Plot

![results_stacked](https://github.com/user-attachments/assets/559e686c-ce1e-4c9d-851e-1d9e2eb6f6b1)

### Table

The table below presents the benchmark results.

|   Nr | model_name                             |      mean |   lineage-8 |   lineage-16 |   lineage-32 |   lineage-64 |
|-----:|:---------------------------------------|----------:|------------:|-------------:|-------------:|-------------:|
|    1 | perplexity/r1-1776                     |     0.934 |       0.965 |        0.985 |        0.935 |        0.850 |
|    2 | openai/o1                              |     0.921 |       1.000 |        0.980 |        0.925 |        0.780 |
|    3 | deepseek/deepseek-r1                   |     0.917 |       0.965 |        0.980 |        0.945 |        0.780 |
|    4 | anthropic/claude-3.7-sonnet:thinking   |     0.898 |       0.985 |        0.970 |        0.910 |        0.725 |
|    5 | deepseek/deepseek-r1-distill-llama-70b |     0.734 |       0.925 |        0.830 |        0.660 |        0.520 |
|    6 | openai/o3-mini                         |     0.726 |       0.970 |        0.945 |        0.795 |        0.195 |
|    7 | qwen/qwq-32b                           |     0.695 |       0.960 |        0.915 |        0.690 |        0.215 |
|    8 | kimi-k1.5-preview                      |     0.613 |       0.830 |        0.655 |        0.635 |        0.330 |
|    8 | deepseek/deepseek-r1-distill-qwen-32b  |     0.613 |       0.805 |        0.685 |        0.595 |        0.365 |
|   10 | deepseek/deepseek-chat                 |     0.610 |       0.860 |        0.590 |        0.530 |        0.460 |
|   11 | openai/o1-mini                         |     0.562 |       0.955 |        0.820 |        0.400 |        0.075 |
|   12 | gemini-exp-1206                        |     0.517 |       0.640 |        0.495 |        0.455 |        0.480 |
|   13 | google/gemini-pro-1.5                  |     0.492 |       0.620 |        0.530 |        0.440 |        0.380 |
|   14 | openai/gpt-4o-2024-11-20               |     0.490 |       0.755 |        0.545 |        0.425 |        0.235 |
|   15 | meta-llama/llama-3.1-405b-instruct     |     0.489 |       0.660 |        0.590 |        0.465 |        0.240 |
|   16 | qwen/qwq-32b-preview                   |     0.476 |       0.845 |        0.585 |        0.315 |        0.160 |
|   17 | mistralai/mistral-large-2411           |     0.475 |       0.695 |        0.510 |        0.360 |        0.335 |
|   17 | allenai/llama-3.1-tulu-3-405b          |     0.475 |       0.710 |        0.505 |        0.335 |        0.350 |
|   19 | qwen/qwen-max                          |     0.463 |       0.710 |        0.435 |        0.410 |        0.295 |
|   20 | meta-llama/llama-3.3-70b-instruct      |     0.438 |       0.625 |        0.485 |        0.340 |        0.300 |
|   21 | deepseek/deepseek-r1-distill-qwen-14b  |     0.428 |       0.830 |        0.600 |        0.200 |        0.080 |
|   22 | x-ai/grok-2-1212                       |     0.405 |       0.580 |        0.395 |        0.360 |        0.285 |
|   23 | gemini-2.0-flash-thinking-exp-1219     |     0.395 |       0.595 |        0.465 |        0.325 |        0.195 |
|   24 | anthropic/claude-3.7-sonnet            |     0.359 |       0.790 |        0.440 |        0.155 |        0.050 |
|   25 | minimax/minimax-01                     |     0.292 |       0.560 |        0.370 |        0.155 |        0.085 |
|   26 | gemini-2.0-flash-exp                   |     0.247 |       0.460 |        0.190 |        0.200 |        0.140 |
|   27 | anthropic/claude-3.5-sonnet            |     0.221 |       0.645 |        0.205 |        0.035 |        0.000 |

Each row contains the average benchmark score across all problem sizes, and separate scores for each problem size.
