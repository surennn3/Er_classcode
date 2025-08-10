# Er_classcode

## Overview

Er_classcode is a comprehensive repository containing educational materials and practical implementations for learning LangChain, LangGraph, and multi-agent systems using CrewAI. This repository includes hands-on Jupyter notebooks that progressively build understanding from basic concepts to advanced agentic architectures.

## Notebooks List

### LangChain Foundations
- **langchain.ipynb** - Introduction to LangChain basics and core concepts
- **langchain_updated.ipynb** - Advanced LangChain patterns and updated implementations

### LangGraph Step-by-Step Tutorial
- **Step1_Lanngraph.ipynb** - Getting started with LangGraph fundamentals
- **Step2_Langgraph.ipynb** - Building simple graph-based workflows
- **Step3_Langgraph.ipynb** - Advanced graph patterns and state management
- **Step4_Langgraph.ipynb** - Complex multi-node graph implementations
- **Step5_Langgraph_AgenticRAG.ipynb** - Implementing Agentic RAG with LangGraph

### Multi-Agent Systems
- **MultiAgentSystem_CrewAI_HierarchicalArchitecture.ipynb** - Building hierarchical multi-agent systems with CrewAI
- **MultiAgentSystem_TravelPlanner.ipynb** - Practical travel planning application using multi-agent architecture

### Additional Resources
- **Session1_2_3_Notes.pdf** - Course notes covering sessions 1-3
- **Session1_2_3_4_updated_Notes.pdf** - Updated course notes including session 4

## Setup

### Prerequisites
- Python 3.8 or higher
- pip or conda for package management
- Jupyter Notebook or JupyterLab
- Git for version control

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/surennn3/Er_classcode.git
   cd Er_classcode
   ```

2. **Create a virtual environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Launch Jupyter:**
   ```bash
   jupyter notebook
   ```

## Environment Variables

Several notebooks require API keys and configuration. Create a `.env` file in the root directory with the following variables:

```bash
# OpenAI API Key (required for most notebooks)
OPENAI_API_KEY=your_openai_api_key_here

# LangChain API Key (optional, for LangSmith tracing)
LANGCHAIN_API_KEY=your_langchain_api_key_here
LANGCHAIN_TRACING_V2=true
LANGCHAIN_PROJECT=er_classcode

# Other API keys as needed
ANTHROPIC_API_KEY=your_anthropic_key_here
GOOGLE_API_KEY=your_google_api_key_here

# Environment settings
PYTHONPATH=.
NUMBA_DISABLE_JIT=1
```

**Important:** Never commit your `.env` file to version control. It's already included in `.gitignore`.

## Run Instructions

### Getting Started
1. Start with the **langchain.ipynb** notebook for basic concepts
2. Progress through the **Step1-Step5** LangGraph tutorials in order
3. Explore the multi-agent systems notebooks for advanced implementations

### Running Individual Notebooks
1. Ensure your virtual environment is activated
2. Launch Jupyter: `jupyter notebook`
3. Navigate to the desired notebook
4. Run cells sequentially, following any specific instructions within each notebook

### Recommended Learning Path
```
Basic LangChain → LangGraph Steps 1-5 → Multi-Agent Systems → Advanced Topics
```

### Working with Different Branches
- **main branch**: Stable versions of all notebooks
- **add-meta-files branch**: Contains additional documentation and meta files
- **development**: Latest experimental features (use with caution)

## Troubleshooting

### Common Issues

**1. API Key Errors**
- Ensure all required API keys are set in your `.env` file
- Verify API keys are valid and have sufficient credits/quota
- Check that `.env` file is in the project root directory

**2. Import Errors**
- Reinstall dependencies: `pip install -r requirements.txt --upgrade`
- Ensure virtual environment is activated
- Check Python version compatibility (3.8+ required)

**3. Jupyter Kernel Issues**
- Install kernel in virtual environment: `python -m ipykernel install --user --name=venv`
- Restart Jupyter server
- Clear notebook outputs and restart kernel

**4. Memory/Performance Issues**
- Close unused notebooks
- Restart Jupyter kernel periodically
- Consider using smaller model variants for development
- Set `NUMBA_DISABLE_JIT=1` in environment variables

**5. Package Compatibility**
- Create fresh virtual environment if conflicts arise
- Use specific package versions from requirements.txt
- Check for version conflicts with: `pip check`

### Getting Help
- Review the PDF notes for theoretical background
- Check individual notebook documentation cells
- Ensure you're following the recommended learning path
- Verify all prerequisites are met before starting

## Contributing

We welcome contributions to improve the educational content and fix issues!

### How to Contribute
1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature/your-feature-name`
3. **Make your changes** following the existing code style and documentation patterns
4. **Test your changes** by running the affected notebooks
5. **Commit your changes**: `git commit -m "Add meaningful commit message"`
6. **Push to your branch**: `git push origin feature/your-feature-name`
7. **Create a Pull Request** with a clear description of your changes

### Contribution Guidelines
- Maintain educational focus and clarity
- Include proper documentation and comments
- Test notebooks thoroughly before submitting
- Follow existing naming conventions
- Update README.md if adding new notebooks or features
- Ensure compatibility with the specified Python version

### Types of Contributions Welcome
- Bug fixes and error corrections
- Additional example notebooks
- Improved documentation and explanations
- Performance optimizations
- New educational content following the existing structure

For major changes, please open an issue first to discuss your proposed modifications.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### MIT License Summary
- **Freedom to use**: Use the code for any purpose, including commercial applications
- **Freedom to modify**: Modify the code to suit your needs
- **Freedom to distribute**: Share the code with others
- **Attribution required**: Include the original license and copyright notice
- **No warranty**: The code is provided "as is" without warranty

By contributing to this repository, you agree that your contributions will be licensed under the same MIT License.

---

**Happy Learning!** 🚀

For questions or support, please open an issue in this repository.
