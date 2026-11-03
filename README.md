# Group Cloud Showcase Web Application

**Course:** IT2402 – Cloud Computing  
**Assessment:** Continuous Assessment 2 (CA2) – Group Assignment  
**Group Number:** Group 6  

This repository contains the source code for the **Group 6 Cloud Showcase** website. It is designed, built, and versioned using Git/GitHub, and automatically deployed to **Microsoft Azure Static Web Apps** via a CI/CD pipeline using GitHub Actions.

---

## Live Links
* **Live Site URL:** https://kind-river-0c0389700.8.azurestaticapps.net
* **GitHub Repository URL:** https://github.com/reezmahanan/ca2-group6-webapp

---

## The Cloud Team Roles
Our junior cloud team is organized according to the following assignments:

* **Azure Lead:** M.R.Ginige,H.M.C.B Herath (Responsible for Task 1 & 2, Portal checks, Resource Group provisioning, and subscription cost logging)
* **Repo Lead:** M.A.Hamas (Responsible for Task 3, repository hygiene, branch management, merge conflict resolution, and synchronization)
* **Front-End Lead:** M.R.Hanan (Responsible for Task 4, structural HTML layout, styling, and local functional browser testing)
* **Deployment Lead:**  W.R.K.W.Hansamali 
 (Responsible for Task 5, Azure Static Web Apps provisioning, CI/CD validation, and post-deployment text updates)


---

## Project Architecture & Naming Conventions
Following the required cloud naming standards (`lower-case` and `hyphen-separated`), this project uses the following topology:

* **Resource Group Name:** `rg-ca2-groupG`
* **Static Web App Name:** `ca2-webapp-groupG`
* **Deployment Plan:** Free Tier
* **Target Region:** Central India
* **Deployment Branch:** `main`
* **Resource Tag:** `environment = ca2`

---

##  Technical Infrastructure

### 1. Repository Structure
The codebase follows a minimal, high-efficiency structure for static landing pages. All build elements are placed directly at the repository root:
```text
├── .gitignore          # Excludes OS metadata, local caches, and IDE environment folders
├── index.html          # Single-page core document containing structural sections and layout logic
└── README.md           # Deployment documentation and group asset configuration
```

### 2. CI/CD Architecture (GitHub Actions)
Continuous Integration and Deployment are automatically handled via an Azure-generated pipeline workflow. 
* **Workflow Location:** Located within `.github/workflows/`
* **Trigger Mechanism:** Listens for `push` events and target `pull_request` interactions bound to the `main` branch.
* **Build Configurations:** Configured with a zero-build-step structure (`app_location: "/"`, `api_location: ""`, `output_location: ""`), bypassing external compilation steps to serve native assets instantly.

---

## Step-by-Step Practical Tracking

### Task 1 & 2: Infrastructure Setup
1. Authenticated into the Azure Portal using an active academic subscription verification.
2. Formed the dedicated resource boundary `rg-ca2-groupG` tagged explicitly with `environment = ca2`.
3. Executed baseline cost analytics metrics reporting to confirm standard starting balances.

### Task 3: Collaborative Version Control
1. Every team member set global local variables configurations using:
   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "your.email@example.com"
   ```
2. Forked and synchronized the centralized repository downstream using individual local feature additions.
3. Successfully committed sequential records into the branch history without generating overlapping merge state errors.

### Task 4 & 5: Build and Validation
1. Created an interface featuring responsive target sections (`Home`, `Team`, `Cloud`, `Contact`) with interactive JavaScript DOM triggers to render date elements dynamically.
2. Pushed the project assets upstream, spawning automated cloud validation jobs via GitHub Actions.
3. Executed an automated update verification by changing the core copy to `"Version 2, deployed automatically"` and watching it populate live in seconds without human manual intervention.
