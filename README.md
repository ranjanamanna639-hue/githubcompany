# githubcompany
I am Ranjana,"To start my career in a reputed organization where I can apply my technical knowledge in electronics and telecommunication, learn new technologies, and contribute to growth of the company while enhancing my professional skills."
# Function to standardize company name
def standardize_company(name):
    if not name or name.strip() == "":
        return "CAF SoftSol India Pvt Ltd."  # Empty or None hole default
    name_lower = name.lower()
    if "caf" in name_lower and ("softsol" in name_lower or "solution" in name_lower):
        return "CAF SoftSol India Pvt Ltd."
    else:
        return name  # onno company hole original name return

# Test cases
test_names = [
    "CAF softsol",
    "CAF solution",
    "CAF softSolution India Pvt Ltd",
    "",
    None,
    "Some Other Company"
]

for name in test_names:
    print("Original:", name, " → Standardized:", standardize_company(name))
