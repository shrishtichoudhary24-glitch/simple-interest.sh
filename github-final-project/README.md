# github-final-project

## Simple Interest Calculator

This project contains a Bash script, `simple-interest.sh`, that calculates **simple interest** from user input: principal, rate of interest and time period.

### Purpose
To practice the GitHub workflow (repository, license, code of conduct, contributing guide) while building a small, useful command-line tool.

### Formula
```
Simple Interest = (Principal x Rate x Time) / 100
```
- **Principal**: the initial amount of money
- **Rate**: the annual rate of interest (%)
- **Time**: the time period in years

### Requirements
- Bash
- `bc` (basic calculator, used for decimal arithmetic)

### How to Use
```bash
chmod +x simple-interest.sh
./simple-interest.sh
```
The script asks for the principal, rate of interest and time period, then prints the simple interest.

### Example
```
Enter principal amount: 1000
Enter rate of interest (%): 5
Enter time period (years): 2
Simple Interest = 100.00
```

### Code Snippet
```bash
read -p "Enter principal amount: " principal
read -p "Enter rate of interest (%): " rate
read -p "Enter time period (years): " time
interest=$(echo "scale=2; ($principal * $rate * $time) / 100" | bc)
echo "Simple Interest = $interest"
```

### Project Files
| File | Description |
|---|---|
| `README.md` | Project name and details |
| `LICENSE` | Apache License 2.0 |
| `CODE_OF_CONDUCT.md` | Contributor Covenant Code of Conduct |
| `CONTRIBUTING.md` | How to contribute |
| `simple-interest.sh` | Simple interest calculator script |

### Contributing
See [CONTRIBUTING.md](CONTRIBUTING.md). Please follow the [Code of Conduct](CODE_OF_CONDUCT.md).

### License
Licensed under the Apache License 2.0. See [LICENSE](LICENSE).
