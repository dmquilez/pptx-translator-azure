# pptx-translator

Python script that translates pptx files using Azure Translator. This script is built upon the [original AWS example](https://github.com/aws-samples/pptx-translator) but it uses Azure Translator services instead.

## Installation

```bash
$ virtualenv venv
$ source venv/bin/activate
$ pip install -r requirements.txt
```

## Usage

Basic translation:
```bash
python pptx-translator.py source_language_code target_language_code input_file_path --azure_key <api_key> --endpoint <URL>
```

Example execution:
```bash
python pptx-translator.py ja en input-file.pptx --azure_key 7ixyAnEmB72lPfFuxXCy71qQfJ8VOndnFJSuGDRWZlSxcumH2aiEPQQJ99AICCi5YpzXJ3w3ABBbACOGSBdi --endpoint https://contoso.cognitiveservices.azure.com/
```

For more information on available options:
```bash
python pptx-translator.py --help
```

## Command-line Arguments

```
usage: pptx-translator.py [-h] --azure_key AZURE_KEY --endpoint ENDPOINT source_language_code target_language_code input_file_path

Translate PPTX files using Azure Translator API

positional arguments:
  source_language_code  The language code for the language of the source text. Example: en
  target_language_code  The language code for the target text. Example: es
  input_file_path       The path to the PPTX file to translate

options:
  -h, --help            show this help message and exit
  --azure_key AZURE_KEY
                        Your Azure Translator API key
  --endpoint ENDPOINT   Your Azure Translator API endpoint
```

## Features

- Translates PowerPoint (.pptx) files from one language to another using Azure Translator

## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This library is licensed under the MIT-0 License. See the LICENSE file.