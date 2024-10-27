# 🐱 Catnip

![catnip-banner](https://github.com/lucianoayres/catnip/blob/main/images/banner_catnip.png?raw=true)

## Generate Comprehensive Categories for Any Topic Effortlessly

[What's Catnip? 🐱](#whats-catnip) · [Why Use Catnip? 🚀](#why-use-catnip) · [How Does It Work? ⚙️](#how-does-it-work) · [Who Is It For? 🎯](#who-is-it-for) · [How to Use 🛠️](#how-to-use) · [Using Nino with Ollama 🐶](#using-nino-with-ollama) · [Templates 📄](#templates) · [Examples 📂](#examples) · [License 📄](#license) · [Contribution 🤝](#contribution)

### What's Catnip? 🐱

**Catnip** is an AI model designed to help you generate comprehensive lists of categories related to any topic you provide. By leveraging [Ollama](https://github.com/ollama/ollama), Catnip simplifies the process of brainstorming and organizing information, enabling you to create customized AI assistants that generate detailed category lists. It's like having a personal librarian that organizes information for you!

### Why Use Catnip? 🚀

-   **Effortless Brainstorming 🔍**: Automatically generate detailed category lists for any topic, saving you time and effort.
-   **Enhanced Organization ⏳**: Organize complex subjects into manageable categories quickly.
-   **Customizable Output 🎨**: Tailor the AI assistant to produce categories that suit your specific needs.
-   **Versatility 🔄**: Fully compatible with [Ollama](https://github.com/ollama/ollama), ensuring seamless model creation and deployment.

### How Does It Work? ⚙️

Catnip uses Modelfiles that define AI models capable of generating comprehensive category lists based on user-provided input. By creating these models with Ollama, you can interact with Catnip to produce organized category structures for your specific needs.

## Who Is It For? 👥

Catnip is for anyone who wants to organize and categorize information more effectively:

-   **Students 📚**: For creating study guides and breaking down complex subjects.
-   **Researchers 🔬**: To map out areas of study and identify key categories.
-   **Content Creators ✍️**: For outlining content topics and subtopics.
-   **Educators 👩‍🏫**: To develop structured curricula and lesson plans.
-   **Business Analysts 📈**: For organizing business domains and market segments.
-   **Project Managers 📋**: To break down projects into manageable categories.

## How to Use 🛠️

Follow these steps to use Catnip and generate comprehensive category lists:

1. **Clone the Repository**:

    ```bash
    git clone https://github.com/lucianoayres/catnip.git
    cd catnip
    ```

2. **Ensure Ollama is Installed**:

    Make sure you have [Ollama](https://github.com/ollama/ollama) installed on your system.

3. **Create the Catnip Model**:

    ```bash
    ollama create catnip1.0 -f ./modelfiles/Catnip1.0
    ```

4. **Run Catnip**:

    ```bash
    ollama run catnip1.0
    ```

5. **Provide Your Topic or Area**:

    When prompted, input your topic or area of interest. For example:

    ```
    Modern Programming Languages
    ```

6. **Review the Generated Categories**:

    Catnip will output a list of categories based on your input. Review this output and make any necessary adjustments.

7. **Save the Category List (Optional)**:

    You can copy the output and save it as a plain text file for future reference.

## Using Nino with Ollama 🐶

You can also use [**Nino**](https://github.com/lucianoayres/nino-cli) to interact with your Ollama models more freely. Nino allows you to send prompts directly to the models from the command line without entering interactive mode, and it also allows you to export the AI's response to a local file.

### Example Command

**Non-Interactive Mode**:

```bash
nino "Mathematics for Computer Science" --model catnip1.0 --output categories.txt
```

## Templates 📄

### Structure 🏗️

The Catnip templates streamline task definition by organizing key components, making it easy to configure and customize AI models while ensuring compatibility with Ollama. The structure includes:

1. **Objective and Rules** 📜: Defines the assistant's purpose and lays out guidelines to ensure the generated category list meets your needs.

2. **Command Specification** 🍳: Details essential commands used in a Modelfile, such as:

    - **META**: Contains metadata about the Modelfile, added as comments.
    - **FROM**: Specifies the base model version (e.g., `llama2`).
    - **PARAMETER**: Sets model parameters like `temperature`, `num_ctx`, and `top_p`.
    - **MESSAGE**: Provides initial messages or prompts for the assistant.
    - **LICENSE**: Includes licensing information for the Modelfile.

3. **Template and Configuration** 🧩: Offers a standard Modelfile template with placeholders (`<< >>`) that can be customized based on your specific idea, goal, or problem.

4. **User Input** 💡: The specific idea, goal, or problem to generate the most effective category list.

### Prompts

The original prompt templates are available for reference in the [prompts directory](./prompts). These resources are valuable for understanding the structure of Modelfiles and can serve educational purposes.

## Examples 📂

### User Input Examples 📝

Examples of prompts you can provide to Catnip:

-   **Topic**: "Renewable Energy Technologies"
-   **Area**: "Ancient Civilizations"
-   **Field**: "Artificial Intelligence Applications"

## License 📄

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contribution 🤝

Contributions are welcome! Please fork the repository and submit a pull request if you'd like to propose any changes.
