# 🧪 PokeAPI Testing Project with Postman, Newman, and GitHub Actions

Welcome! This project is a fully automated API testing suite created for the [PokeAPI](https://pokeapi.co), using **Postman**, **Newman**, and **GitHub Actions**.

- ✅ **10 API testing scenarios**
- ✅ **15+ individual test cases**
- ✅ **Pre-request & Post-request scripts**
- ✅ **Newman HTML & JSON reports**
- ✅ **Environment-based URL handling**
- ✅ **Automated test pipeline via GitHub Actions**

---

## 🔧 Tools & Technologies Used

| Tool          | Purpose                                 |
|---------------|-----------------------------------------|
| Postman       | Creating and managing test collections  |
| Newman        | Running tests in the terminal/CI        |
| GitHub Actions| Running tests automatically on push     |
| JavaScript    | Used in test assertions/scripts         |
| Node.js       | Running Newman via `npm`                |

---

## 🧪 How to Run Tests Locally

1. **Clone the repository:**

```bash
git clone https://github.com/your-username/pokeapi-testing.git
cd pokeapi-testing

🧙 Test Design
Tests are organized into logical scenarios such as:

Valid/invalid Pokémon data
Type matching
Error response testing
Edge case handling
Intentional failure scenarios (to test robustness)
Each request includes relevant:
Pre-request scripts (like setting environment vars)
Post-request test scripts using pm.test() assertions

🚀 CI/CD: GitHub Actions
Every time code is pushed to main, the test suite runs automatically via GitHub Actions.
Check it under the "Actions" tab in your GitHub repository.

Workflow file: .github/workflows/run-tests.yml

📁 Project Structure
PokeAPI/
├── .github/workflows/run-tests.yml      # GitHub Actions workflow
├── pokeapi-tests.postman_collection.json # Main Postman test collection
├── pokeapi-env.postman_environment.json # Environment variables
├── newman-report.html                   # HTML test report
├── newman-report.json                   # JSON test report
├── .gitignore                           # Ignore node_modules & reports
├── package.json                         # Project config + test script
└── README.md                            # You're reading it! 📖

👨‍🏫 Notes for Lecturer
Lecturer GitHub username: Dailius (invited as a collaborator).
Tests were designed with a mix of success and failure to simulate real-world quality assurance practices.

🧠 Author
Kipras
Just a guy who likes clean test cases, catching bugs, and Pikachu.

🐛 Known Issues / Fun Glitches
Some tests are meant to fail.
The PokeAPI sometimes returns 404s for made-up Pokémon — which we fully embrace for test coverage 🎯

🏁 Done & Dusted
Thanks for checking it out — feel free to run the tests or browse the code!