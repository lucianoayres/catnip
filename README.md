# 🐱 Catnip

![catnip-banner](https://github.com/lucianoayres/catnip/blob/main/images/banner_catnip.png?raw=true)

## Generate Comprehensive Categories for Any Topic Effortlessly

[What's Catnip? 🐱](#whats-catnip) · [Why Use Catnip? 🚀](#why-use-catnip) · [How Does It Work? ⚙️](#how-does-it-work) · [Who Is It For? 🎯](#who-is-it-for) · [Modes of Catnip 🎛️](#modes-of-catnip) · [How to Use 🛠️](#how-to-use) · [Using Nino with Ollama 🐶](#using-nino-with-ollama) · [Templates 📄](#templates) · [Examples 📂](#examples) · [License 📄](#license) · [Contribution 🤝](#contribution)

### What's Catnip? 🐱

**Catnip** is an AI model designed to help you generate comprehensive categories related to your topics or areas of interest. By leveraging [Ollama](https://github.com/ollama/ollama), Catnip simplifies the process of organizing and categorizing information, enabling you to create customized AI assistants that generate detailed category lists tailored to your needs.

Catnip offers two modes to suit your needs:

-   **Catnip Panorama** 🌄: Generates a comprehensive list of categories related to your topic.
-   **Catnip Spotlight** 🔦: Provides a single, randomly selected category relevant to your topic.

### Why Use Catnip? 🚀

-   **Effortless Brainstorming 🔍**: Automatically generate detailed category lists or discover a single category for any topic.
-   **Enhanced Organization ⏳**: Organize complex subjects into manageable categories quickly.
-   **Customizable Output 🎨**: Tailor the AI assistant to produce categories that suit your specific needs.
-   **Versatility 🔄**: Fully compatible with [Ollama](https://github.com/ollama/ollama), ensuring seamless model creation and deployment.

### How Does It Work? ⚙️

Catnip uses Modelfiles that define AI models capable of generating comprehensive category lists or providing a single category based on user-provided input. By creating these models with Ollama, you can interact with Catnip in the mode that best suits your needs.

## Who Is It For? 👥

Catnip is for anyone who wants to organize and categorize information more effectively:

-   **Students 📚**: For creating study guides and breaking down complex subjects.
-   **Researchers 🔬**: To map out areas of study and identify key categories.
-   **Content Creators ✍️**: For outlining content topics and subtopics.
-   **Educators 👩‍🏫**: To develop structured curricula and lesson plans.
-   **Business Analysts 📈**: For organizing business domains and market segments.
-   **Project Managers 📋**: To break down projects into manageable categories.

## Modes of Catnip 🎛️

### Catnip Panorama 🌄

Generates a comprehensive list of categories related to your topic. Ideal for when you need an extensive overview or are brainstorming multiple aspects of a subject.

### Catnip Spotlight 🔦

Provides a single, randomly selected category relevant to your topic. Great for when you need a quick idea or focus point without the overload of a full list.

## How to Use 🛠️

Follow these steps to use Catnip and generate comprehensive category lists or a single category:

### 1. Clone the Repository

```bash
git clone https://github.com/lucianoayres/catnip.git
cd catnip
```

### 2. Ensure Ollama is Installed

Make sure you have [Ollama](https://github.com/ollama/ollama) installed on your system.

### 3. Create the Catnip Models

#### For Catnip Panorama

```bash
ollama create catnip-panorama1.0 -f ./modelfiles/Catnip-Panorama1.0
```

#### For Catnip Spotlight

```bash
ollama create catnip-spotlight1.0 -f ./modelfiles/Catnip-Spotlight1.0
```

### 4. Run Catnip

#### Using Catnip Panorama

```bash
ollama run catnip-panorama1.0
```

#### Using Catnip Spotlight

```bash
ollama run catnip-spotlight1.0
```

### 5. Provide Your Topic or Area

When prompted, input your topic or area of interest. For example:

```
Modern Programming Languages
```

### 6. Review the Output

-   **Catnip Panorama** will output a comprehensive list of categories based on your input.
-   **Catnip Spotlight** will output a single, randomly selected category relevant to your topic.

### 7. Save the Output (Optional)

You can copy the output and save it as a plain text file for future reference.

## Using Nino with Ollama 🐶

You can also use [**Nino**](https://github.com/lucianoayres/nino-cli) to interact with your Ollama models more freely. Nino allows you to send prompts directly to the models from the command line without entering interactive mode, and it also allows you to export the AI's response to a local file.

### Example Commands

#### Using Catnip Panorama

```bash
nino "Mathematics for Computer Science" --model catnip-panorama1.0 --output categories.txt
```

#### Using Catnip Spotlight

```bash
nino "Mathematics for Computer Science" --model catnip-spotlight1.0 --output category.txt
```

## Templates 📄

### Structure 🏗️

The Catnip templates streamline task definition by organizing key components, making it easy to configure and customize AI models while ensuring compatibility with Ollama. The structure includes:

1. **Objective and Rules** 📜: Defines the assistant's purpose and lays out guidelines to ensure the generated output meets your needs.

2. **Command Specification** 🍳: Details essential commands used in a Modelfile, such as:

    - **META**: Contains metadata about the Modelfile, added as comments.
    - **FROM**: Specifies the base model version (e.g., `llama2`).
    - **PARAMETER**: Sets model parameters like `temperature`, `num_ctx`, and `top_p`.
    - **MESSAGE**: Provides initial messages or prompts for the assistant.
    - **LICENSE**: Includes licensing information for the Modelfile.

3. **Template and Configuration** 🧩: Offers a standard Modelfile template with placeholders (`<< >>`) that can be customized based on your specific idea, goal, or problem.

4. **User Input** 💡: The specific idea, goal, or problem to generate the most effective output.

### Prompts

The original prompt templates are available for reference in the [prompts directory](./prompts). These resources are valuable for understanding the structure of Modelfiles and can serve educational purposes.

## Examples 📂

### Catnip Panorama Examples 📝

Examples of prompts you can provide to Catnip Panorama:

-   **Topic**: "Renewable Energy Technologies"
-   **Area**: "Ancient Civilizations"
-   **Field**: "Artificial Intelligence Applications"

#### Output Example

For the topic "Renewable Energy Technologies," Catnip Panorama might generate:

-   Solar Energy
-   Wind Energy
-   Hydroelectric Power
-   Geothermal Energy
-   Biomass Energy
-   Tidal Energy
-   Wave Energy
-   Hydrogen Fuel Cells

### Catnip Spotlight Examples 📝

Examples of prompts you can provide to Catnip Spotlight:

-   **Topic**: "Renewable Energy Technologies"
-   **Area**: "Ancient Civilizations"
-   **Field**: "Artificial Intelligence Applications"

#### Output Example

For the topic "Renewable Energy Technologies", Catnip Spotlight might output:

-   Tidal Energy

## License 📄

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contribution 🤝

Contributions are welcome! Please fork the repository and submit a pull request if you'd like to propose any changes.
