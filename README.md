# LNbits Transfer to Wallet of Satoshi

## Script for Lightning transfer to Lightning Address provided by Wallet of Satoshi

and then you just input 4 parameter at the top.

and run it baby. (python LN_Send_Sat_To_WOS.py)

<img width="993" height="523" alt="image" src="https://github.com/user-attachments/assets/3e06cc1e-5ba7-4236-838a-5cbc8dfbdc86" />

### Prerequisites

* [git](https://git-scm.com/) - --fast-version-control
* [python](https://www.python.org) 3.9 and above - High-level general-purpose programming language
* [uv](https://docs.astral.sh/uv) - Extremely fast Python package & project manager, written in Rust

The following guide walks through setting up your local working environment using `git`
as distributed version control system and `uv` as Python package and version manager.
If you do not have `git` installed, run the following command.

<details>
  <summary> Install using Homebrew (Darwin) </summary>
  
  ```bash
  brew install git
  ```
</details>

<details>
  <summary> Install via binary installer (Linux or Windows Subsystem for Linux [WSL]) </summary>
  
  * Debian-based package management
  ```bash
  sudo apt install git-all
  ```

  * Fedora-based package management
  ```bash
  sudo dnf install git-all
  ```
</details>

<details>
  <summary> Install using Winget (Windows Powershell) </summary>
  
  ```bash
  winget install --id Git.Git -e --source winget
  ```
</details>

If you do not have `uv` installed, run the following command.

<details>
  <summary> Install using Homebrew (Darwin) </summary>

  ```bash
  brew install uv
  ```
</details>

<details>
  <summary>
    Install using standalone installer (Darwin, Linux, or Windows Subsystem for Linux [WSL])
  </summary>

  ```bash
  curl -LsSf https://astral.sh/uv/install.sh | sh
  ```
</details>

<details>
  <summary> Install using Winget (Windows Powershell) </summary>

  ```bash
  winget install --id=astral-sh.uv -e
  ```
</details>

Once you have `git` distributed version control system installed, you can
clone the current repository and  install any version of Python above version
3.9 for this project. The following commands help you set up and activate a
Python virtual environment where `uv` can download project dependencies from the `PyPI`
open-sourced registry defined under `pyproject.toml` file.

<details>
  <summary> Set up environment and synchronize project dependencies </summary>

  ```bash
  git clone git@github.com:ta007403/LNbits-Lightning-Transfer.git
  cd etiquette
  uv venv --python 3.9.6
  source .venv/bin/activate
  uv sync --dev
  ```
</details>

### Getting started

Once you have virtual environment set up, install project dependencies with the following
command:

```bash
uv sync
```

<details>
  <summary> Sample output of successful dependency installation </summary>

  ```bash
  $ uv sync
  > Resolved 6 packages in 2ms
  > Prepared 1 package in 146ms
  > Installed 6 packages in 6ms
  >  + certifi==2025.7.14
  >  + charset-normalizer==3.4.2
  >  + idna==3.10
  >  + lnbits-tx-wos==0.0.1 (from file:///Users/mackasitt/workspaces/lnbits-lntx)
  >  + requests==2.32.4
  >  + urllib3==2.5.0
  ```
</details>
