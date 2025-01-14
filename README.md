# refiner-cli

[CLI](https://pypi.org/project/refiner-cli/) for the [Refiner](https://pypi.org/project/refiner/) python package convert and store text and metadata as vector embeddings. Embeddings are generated using [OpenAI](https://openai.com/) and stored as vectors in [Pinecone](https://www.pinecone.io/). Stored embeddings can then be "queried" using the `search` command. Matched embeddings contain contextually relavant metadata that can be used for AI chatbots, semnatic search APIs, and can also be used for training and tuning large language models.

## Installation

```shell
pip install refiner-cli
```

## OpenAI and Pinecone API Keys.

You'll need API keys for OpenAI and Pinecone.

Once you have your API keys, you can either set local ENV variables in a shell:

```shell
export PINECONE_API_KEY="API_KEY"
export PINECONE_ENVIRONMENT_NAME="ENV_NAME"
export OPENAI_API_KEY="API_KEY"
```

or you can create a `.env` (dotenv) config file and pass it in with the `--config-file` option.

Your .env file should follow key/value format:

```shell
PINECONE_API_KEY="API_KEY"
PINECONE_ENVIRONMENT_NAME="ENV_NAME"
OPENAI_API_KEY="API_KEY"
```

## Help

The `--help` option can be used to learn about the `create` and `search` commands.

```shell
refiner --help
refiner create --help
refiner search --help
```
