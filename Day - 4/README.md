# Day 4 — Tools, Structured Output and Google Sheets

## Project: Sweet Crumbs Home Bakery
A LangChain agent that looks up prices and opening hours, checks menu availability, extracts structured orders and saves confirmed orders to Google Sheets.

## Technology
Python, Google Colab, LangChain, Groq API (`openai/gpt-oss-120b`), Pydantic and gspread.

## Tasks
| Task | Implementation | Expected evidence |
|---|---|---|
| 1 | `get_price`, `is_available`, `is_open` tools | Two chocolate cakes cost Rs 1300; Sunday hours 10 am to 6 pm |
| 2 | `Order` schema and `with_structured_output` | Five validated records from messy messages |
| 3 | `log_order` and Google Sheets | Ravi, chocolate cake, 2, 24 Dec, yes, 1300 |
| 4 | Compare `get_price` with `tool1` (does stuff) | Actual selected tools and answers; vague tool may still work |
| 5 | `pretty_print()` trace | Actual tool call count and model response rounds |

## Setup
1. Open `Day_4_Solutions.ipynb` in Colab.
2. Add `GROQ_API_KEY` to Secrets and enable notebook access.
3. Run cells in order and authorize Google Sheets when prompted.
4. Check the test sheet. Do not repeatedly run the save cell, which can append duplicates.

## Validation
Test an unknown donut, missing pickup date and zero quantity. No invalid order should be saved. Add these cases to the Day 3 CSV. Menu availability does not represent live inventory.

## Results
Live API and Sheets execution is pending. Record actual structured-output successes, tool selections, trace counts and negative-test results after running in Colab. No measured results are claimed here.

## Learning outcome
Tools provide deterministic lookups and actions, Pydantic validates records, and agent traces show how the model uses tools. Google Sheets provides persistent storage. Keep API keys out of GitHub.

## Before Day 5
Prepare a business facts text file for RAG. Confirm any additional business policies before treating them as facts.
