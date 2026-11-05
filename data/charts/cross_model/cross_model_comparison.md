# Cross-model comparison

## google/gemini-3-flash-preview

|              |   Level 0 |   Level 1 |   Level 2 |   Level 3 |
|:-------------|----------:|----------:|----------:|----------:|
| COMPATIBLE   |      1.00 |      1.00 |      1.00 |      1.00 |
| PARTIAL      |      1.00 |      1.00 |      1.00 |      1.00 |
| INCOMPATIBLE |      0.00 |      0.00 |      0.43 |      1.00 |

## openai/gpt-5.4-mini

|              |   Level 0 |   Level 1 |   Level 2 |   Level 3 |
|:-------------|----------:|----------:|----------:|----------:|
| COMPATIBLE   |      1.00 |      1.00 |      1.00 |      1.00 |
| PARTIAL      |      1.00 |      1.00 |      1.00 |      1.00 |
| INCOMPATIBLE |      0.47 |      0.40 |      0.53 |      0.47 |

## anthropic/claude-3-haiku

|              |   Level 0 |   Level 1 |   Level 2 |   Level 3 |
|:-------------|----------:|----------:|----------:|----------:|
| COMPATIBLE   |      1.00 |      1.00 |      1.00 |      1.00 |
| PARTIAL      |      1.00 |      1.00 |      1.00 |      1.00 |
| INCOMPATIBLE |      1.00 |      0.86 |      0.82 |      0.94 |

## Pairwise differences

### google/gemini-3-flash-preview − openai/gpt-5.4-mini

|              |   Level 0 |   Level 1 |   Level 2 |   Level 3 |
|:-------------|----------:|----------:|----------:|----------:|
| COMPATIBLE   |     +0.00 |     +0.00 |     +0.00 |     +0.00 |
| PARTIAL      |     +0.00 |     +0.00 |     +0.00 |     +0.00 |
| INCOMPATIBLE |     -0.47 |     -0.40 |     -0.10 |     +0.53 |

### google/gemini-3-flash-preview − anthropic/claude-3-haiku

|              |   Level 0 |   Level 1 |   Level 2 |   Level 3 |
|:-------------|----------:|----------:|----------:|----------:|
| COMPATIBLE   |     +0.00 |     +0.00 |     +0.00 |     +0.00 |
| PARTIAL      |     +0.00 |     +0.00 |     +0.00 |     +0.00 |
| INCOMPATIBLE |     -1.00 |     -0.86 |     -0.38 |     +0.06 |

### openai/gpt-5.4-mini − anthropic/claude-3-haiku

|              |   Level 0 |   Level 1 |   Level 2 |   Level 3 |
|:-------------|----------:|----------:|----------:|----------:|
| COMPATIBLE   |     +0.00 |     +0.00 |     +0.00 |     +0.00 |
| PARTIAL      |     +0.00 |     +0.00 |     +0.00 |     +0.00 |
| INCOMPATIBLE |     -0.53 |     -0.46 |     -0.28 |     -0.47 |

