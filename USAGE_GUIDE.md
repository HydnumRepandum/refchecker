# How to Run RefChecker on a Text File

You can allow RefChecker to process a plain text file containing a bibliography or raw reference text.

## Command

Run the following command in your terminal:

```bash
python run_refchecker.py --paper /path/to/your/document.txt
```

## Using with Llama 3.1 (Local)

To use your local Llama 3.1 model for extracting references from the text file (recommended for unstructured text):

```bash
python run_refchecker.py \
  --paper /path/to/your/document.txt \
  --llm-provider openai \
  --llm-endpoint http://localhost:11434/v1 \
  --llm-model llama3.1
```

## Notes

- The text file should ideally contain the bibliography section or the raw text of the paper.
- If the file is structured (e.g., BibTeX), you can use the same command.
