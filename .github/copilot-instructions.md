- This project uses uv to manage Python environments and dependencies.
    - The virtual environment is created in the `.venv` directory. Create it with `uv create venv` if it doesn't exist.
    - To activate the environment, use `source .venv/bin/activate` (Linux/Mac) or `.venv\Scripts\activate` (Windows).
    - Install dependencies with `uv pip install -e .`.
- Unit tests are run with pytest, but remember you must activate the virtual environment first as described above.
- The solution must meet the functionality as explained in the [README.md](README.md) file.
- The general high-level basis to the solution is depicted in [APPROACH.md](../../APPROACH.md). 
- When developing functionality, we need to respect our own [CONTRIBUTING.md](../../CONTRIBUTING.md) file.
The architectural decisions and basis for the project in that document are only the inspiring foundation. It can and should always be challenged when needed and is not meant as the only truth, but a very useful context and grounding research.
- The project is meant for the Open Source community and should be open to contributions and follow the standards of the community.
- The project is meant to be used by developers and should be easy to use, with a focus on developer experience.
- The philosophy when architecting and implementing the project is to prime speed and simplicity over complexity. Do NOT implement backwards compatibility: ship fast. Do NOT over-engineer, but rather build a solid foundation that can be iterated on. 
- We have no users, we do not need backwards compatibility, we do not need migration guides when we ship breaking changes, we do not need to worry.
- The goal is to deliver a solid and scalable architecture but simple starting implementation. Not building something complex from the start and then having to simplify it later. Remember we are delivering a new tool to the developer community and we will need to rapidly adapt to what's really useful, evolving standards, etc. 