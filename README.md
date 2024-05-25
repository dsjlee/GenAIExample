# GenAIExample

Created from Microsoft tutorial: https://learn.microsoft.com/en-us/windows/ai/models/get-started-models-genai

Add a model and vocabulary file to your project:
In Solution Explorer, right-click your project and select Add->New Folder. Name the new folder "Models". For this example, we will be using the model from https://huggingface.co/microsoft/Phi-3-mini-4k-instruct-onnx/tree/main/directml/directml-int4-awq-block-128.

There are several different ways to retrieve models. For this walkthrough, we will use the Hugging Face Command Line Interface (CLI). If you get the models using another method, you may have to adjust the file paths to the model in the example code. For information on installing the Hugging Face CLI and setting up your account to use it, see Command Line Interface (CLI).

After installing the CLI, open a terminal, navigate to the Models directory you created, and type the following command.

huggingface-cli download microsoft/Phi-3-mini-4k-instruct-onnx --include directml/* --local-dir .

When the operation is complete verify that the following file exists: [Project Directory]\Models\directml\directml-int4-awq-block-128\model.onnx.

In Solution Explorer, expand the "directml-int4-awq-block-128" folder and select all of the files in the folder. In the File Properties pane, set Copy to Output Directory to "Copy if newer".
