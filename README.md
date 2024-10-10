# quarkus-langchain4j-workshop

## AI Lab Recipes

This repository is a fork from https://github.com/cescoffier/quarkus-langchain4j-workshop 
adding `ai-lab.yaml` files and instructions to run the steps of the workshop 
as recipes in Podman AI Lab.

To add the steps (01 and 02 currently) of the workshop to your local catalog of recipes for Podman AI Lab,
you have to create the file `$HOME/.local/share/containers/podman-desktop/extensions-storage/redhat.ai-lab/user-catalog.json`
with the following content:

```
{
  "version": "1.0",
  "recipes": [
    {
      "id": "quarkus-langchain4j-step-01",
      "description" : "Quarkus Langchain4j Step 01",
      "name" : "Quarkus Langchain4j Step 01",
      "repository": "https://github.com/feloy/ai-lab-recipes-langchain4j",
      "ref": "main",
      "icon": "natural-language-processing",
      "categories": [
        "natural-language-processing"
      ],
      "basedir": "step-01",
      "readme": "",
      "recommended": [
        "hf.TheBloke.mistral-7b-instruct-v0.2.Q4_K_M"
      ],
      "backend": "llama-cpp"
    },
    {
      "id": "quarkus-langchain4j-step-02",
      "description" : "Quarkus Langchain4j Step 02",
      "name" : "Quarkus Langchain4j Step 02",
      "repository": "https://github.com/feloy/ai-lab-recipes-langchain4j",
      "ref": "main",
      "icon": "natural-language-processing",
      "categories": [
        "natural-language-processing"
      ],
      "basedir": "step-02",
      "readme": "",
      "recommended": [
        "hf.TheBloke.mistral-7b-instruct-v0.2.Q4_K_M"
      ],
      "backend": "llama-cpp"
    }
  ]
}
```

## Workshop

A workshop to learn how to build AI-Infused applications with Quarkus and LangChain4j.


The workshop is divided into several steps.
You can follow the instructions available in the [docs](docs) directory.

The final state of each step is available in the [step-XX](step-XX) directory.
You can quickly jump to the final state of a step by navigating to the corresponding directory, and then running the following command:

```shell
./mvnw quarkus:dev
```

The application runs on [http://localhost:8080](http://localhost:8080).