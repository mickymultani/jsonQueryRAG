# jsonQueryRAG
LLM query engine to retrieve augmented responses from json files.

```markdown
# JSON Query RAG (jsonQueryRAG)

This repository contains a Colab notebook that demonstrates how to set up a system to query JSON data using natural language and obtain responses. The implementation utilizes the `jsonpath-ng`, `llama-index`, `openai`, `transformers`, and `accelerate` libraries.

## Getting Started

1. Open the notebook in Google Colab by clicking the badge below:
   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mickymult/jsonQueryRAG/blob/main/jsonQueryRAG.ipynb)
   
2. Install the necessary libraries by running the first few cells in the notebook.

## Usage

- The notebook contains cells for installing necessary libraries, setting up logging, specifying Open AI API keys, and importing required modules.
- It also includes cells for specifying the paths to your JSON and schema files, reading these files, and setting up the JSON query engines.
- To query the JSON data, modify the query text in the cell with `nl_query_engine.query()` and run the cell.

## Example Query

The notebook includes an example query that asks for the types of toppings available for a donut cake, and displays the natural language response.

```python
nl_response = nl_query_engine.query(
    "what type of toppings are available for donut cake?",
)
display(Markdown(f"<h1>Natural language Response</h1><br><b>{nl_response}</b>"))
```

The expected output for this query is:

```
The available toppings for the donut cake are None, Glazed, Sugar, Powdered Sugar, Chocolate with Sprinkles, Chocolate, and Maple.
```

## Dependencies

- jsonpath-ng
- llama-index
- openai
- transformers
- accelerate

## License

MIT


```
