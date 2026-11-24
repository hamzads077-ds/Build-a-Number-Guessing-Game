# 🎲 Build a Number Guessing Game

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Bash](https://img.shields.io/badge/Bash_Script-121011?style=for-the-badge&logo=gnu-bash&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![freeCodeCamp](https://img.shields.io/badge/freeCodeCamp-0A0A23?style=for-the-badge&logo=freecodecamp&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

---

An interactive command-line Number Guessing Game built with **Bash** and **PostgreSQL** as the final certification project for the **freeCodeCamp Relational Database** curriculum.

---

## 📋 Overview

The script generates a random secret integer between `1` and `1000`, tracks returning and first-time players in a PostgreSQL database (`number_guess`), validates integer inputs, gives higher/lower hints, and records each player's total games played and best (fewest guesses) score.

---

## 🗄️ Database Schema

The `number_guess` database consists of two normalized relational tables:

1. **`users`**
   - `user_id` (`SERIAL`, Primary Key)
   - `username` (`VARCHAR(22)`, Unique, Not Null)

2. **`games`**
   - `game_id` (`SERIAL`, Primary Key)
   - `user_id` (`INT`, Foreign Key → `users.user_id`, Not Null)
   - `guesses` (`INT`, Not Null)

---

## 🚀 Usage

### 1. Restore the Database
Rebuild the PostgreSQL database from the included SQL dump:
```bash
psql -U postgres < number_guess.sql
chmod +x number_guess.sh
./number_guess.sh
```

---

## 📊 Repository Stats

[![Stars](https://img.shields.io/github/stars/hamzads077-ds/Build-a-Number-Guessing-Game?style=for-the-badge&logo=github&color=yellow)](https://github.com/hamzads077-ds/Build-a-Number-Guessing-Game/stargazers)
[![Forks](https://img.shields.io/github/forks/hamzads077-ds/Build-a-Number-Guessing-Game?style=for-the-badge&logo=github&color=blue)](https://github.com/hamzads077-ds/Build-a-Number-Guessing-Game/network/members)
[![Views](https://komarev.com/ghpvc/?username=hamzads077-ds-number-guess&style=for-the-badge&color=brightgreen&label=VIEWS)](https://github.com/hamzads077-ds/Build-a-Number-Guessing-Game)
