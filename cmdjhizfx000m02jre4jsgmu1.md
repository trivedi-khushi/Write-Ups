---
title: "OpenAPI Sample Library: Complete Project Workflow"
seoTitle: "OpenAPI Documentation: Project Workflow Guide"
seoDescription: "Explore OpenAPI Sample Library for modular API documentation using OpenAPI 3.0 for GitHub, Jira, Notion, Slack, and Stripe"
datePublished: Sat Jul 26 2025 00:01:17 GMT+0000 (Coordinated Universal Time)
cuid: cmdjhizfx000m02jre4jsgmu1
slug: openapi-sample-library-project
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1753483304800/87fad77b-4281-46ca-a10f-9ee541fd0547.png
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1753487990971/a3402180-4146-4356-8566-02672a6f9949.png
tags: docker, github, opensource, community, apis, hashnode, swagger, rest-api, linting, crud, openapi, restful-apis, docker-images, khushitrivedi, redocly

---

## 💼Project Overview

**<mark>Project Link - </mark>** [**<mark>https://github.com/trivedi-khushi/openapi-sample-library/</mark>**](https://github.com/trivedi-khushi/openapi-sample-library/)

The **OpenAPI Sample Library** is a modular and extensive documentation project designed to simplify interaction with various APIs (GitHub, Jira, Notion, Slack, and Stripe). The project utilizes the latest OpenAPI 3.0 specification and serves as a combination of hands-on technical documentation with developer experience (DevEx). [Reposiorty Link](https://github.com/trivedi-khushi/openapi-sample-library/)

This project brings together real-world API Endpoints from 5 widely-used developer platforms, each with different use cases. OpenAPI Sample Library showcases how to write, structure, test, lint, debug, and publish OpenAPI specs in a scalable and professional way.

Intended Audience - Developer, Technical Writers, Project Managers, Developer Advocates (DevRel), Open-Source Contributors.

## 🎯Goals & Objectives

OpenAPI Sample Library is an interactive API documentation project to make it accessible for developers to test APIs in a zero-setup playground. These are instant, ready-to-use, descriptive, browser-based, supported with copy-paste commands, and even sample values.

<div data-node-type="callout">
<div data-node-type="callout-emoji">💡</div>
<div data-node-type="callout-text">The primary objective of this project is to enhance the <strong>Developer Experience (DevEx)</strong> for testing an API’s output by trying endpoints directly in the browser! As a result, <strong>allows developers to test, judge, and onboard an API faster.</strong></div>
</div>

The purpose doesn’t compromise on intricacies like easy-navigation, and consistent formatting. The intended outcome is to turn passive documentation into an active tool for developers.

## 🛠️Project Specifications & Toolchain

| **Requirement for the Project** | **Tool/Utility to solve it** |
| --- | --- |
| Specification standard for RESTful APIs compatibility. | **OpenAPI 3.0** |
| Modularized & Human-readable data format to make OpenaPI specs. | **YAML** |
| Local linting, bundling OpenAPI specs, enforcing schema validation. | **Redocly CLI** |
| Preview, validate, debug OpenAPI YAML file. | **Swagger Editor (browser-based)** |
| Get Swagger-UI for local preview, get a consistent environment for all systems | **Docker** |
| official Docker image to render with OpenAPI spec in browser. | **Swagger-UI (Docker Image)** |
| Automate build, publish Docker Image, set workflows on commit & PRs, and look for easy contributor onboarding. | **GitHub Actions (CI/CD)** |
| Source code & version management | **Git** |
| Hosting, project management, contribution, remote collab, issue tracking | **GitHub** |
| Open-source licensing (MIT, Apache, etc. as per your selection). | **Project License** |

## 🏗️ Project Structure

For ease of maintenance, modularity, and following the standard to draft OpenAPI Documentation for RESTful APIs, the project is managed in a descriptive structure. This structure employs a direct layout:

**👇Must read for an entire understanding of the project!**

```plaintext
openapi-sample-library/
├── .github/workflows/     ---> includes GitHub Actions workflows (CI/CD, code checks, etc.)
├── api_catalog/           ---> contains all API endpoints based-on org
├── apis/                  ---> contains main OpenAPI specs for each endpoint respective to its org
│   ├── github/
│   ├── jira/
│   ├── notion/
│   ├── slack/
│   └── stripe/
├── components/            ---> includes API components like parameters & schemas for each org
│   ├── github/
│   │   ├── parameters/
│   │   └── schemas/
│   ├── jira/
│   └── ...
├── examples/               ---> YAML file to state sample request/response payloads for each API endpoint
├── images/                 ---> project's media files mainly images.
├── .gitattributes          ---> enforce consistent line endings & text file normalization
├── .gitignore              ---> Ignores generated/local dev files for git not to track them.
├── Dockerfile              ---> Docker setup to preview docs locally via Swagger UI
├── LICENSE  
├── README.md                 ---> about/project description/setup/troubleshooting.
├── about-the-project.mdx     ---> design decisions for the project
├── apis-to-document.mdx      ---> list of API endpoints to documented.
├── getting-started.mdx       ---> Quickstart guide for contributors/new users. [Recommended to reaed]
├── index.html                ---> CStatic Landing Page 

└── openapi.yaml              ---> Root OpenAPI file containing global declarations, (all files are directly/indirectly linked to this)
```

## 🛍️Deciding Which APIs to Include?

The project initially (currently) focuses on demonstrating 20 APIs across various Dev tools and services. Following factors were considered for choosing the APIs to demonstrate for the OpenAPI Sample Library:

* Reflect common developer **workflows**.
    
* **Variety** inclusion in case of task **use-cases**.
    
* Broad **coverage**—no repetitive APIs.
    
* **Popular** & Familiar APIs from each major platform.
    
* Covers **CRUD** operations clearly.
    
* Rich **examples** and clearly defined **schema**.
    

## 🌱 Step-by-Step Workflow

Here’s an easy & visual representation of this project’s workflow.

![How to make API Documentation? Workflow to draft OpenAPI specs. Design by Khushi Trivedi on workflow for OpenAPI Documentation.](https://cdn.hashnode.com/res/hashnode/image/upload/v1753450093995/c094880f-7f83-4e44-b8bc-1befc4b615e6.jpeg align="center")

### **Step-1: Initial Planning & API Research**

After deciding on the target APIs and collecting the respective endpoints. For instance, here is an API endpoint for GitHub’s `Update an Issue` API as :

`PATCH /repos/{owner}/{repo}/issues/{issue_number}`

To document and implement an API endpoint, you must gather these key details from its official documentation, like:

1. Endpoint URL and Methods (HTTPS, & Authentication)
    
2. Parameters (body, query, request)
    
3. Schema definitions- requests & responses
    
4. All the possible response-codes & error-codes
    
5. Note the required fields specifically
    

---

### **Step-2: Plan & Design a Modular Project Structure**

A repository layout must have a basic structure with a minimum 3 folders: `apis/` (endpoint specs), `components/` (schemas & parameters) & `examples/` (example payloads). Meanwhile, in case of files, maintaining `README.md`, `.gitignore` and `.gitattribute` is considered to be a healthy practice while working on a project or operating a repository.

**What Does “Modular” Mean? Why Build a Project This Way?**  
By modular, it means building your project in independent pieces, and structured so that it becomes easier for reuse & maintenance. It’s just like a toolbox, where the big tools, screws, and wires all live in their own trays within the toolbox.

Hence, a modular project framework makes it easier to:  
🔹 Reuse easily,  
🔹 Swap or upgrade a single component without disturbing the other  
🔹 Quick locating & maintaining.

---

### **Step-3: Working on your selected API spec**

Writing an API endpoint in OpenAPI Spec is itself a combination of sub-tasks that need to be done carefully. It’s easy with the flow; however, debugging might be a big headache in case of tiny errors like character mismatch or wrong indentation. Make sure you’ve followed the steps carefully so far.

Here’s a table to well define each sub-task for writing an API spec.

| **Sub‑Task** | **Chore description for it** | **Concept behind (Why?)** |
| --- | --- | --- |
| **Parameter Definition:** | Under the folder, create separate file, & define each of them. They must be YAML files for each parameter (e.g., `owner.yaml`, `repo.yaml`, `issue_number.yaml`). In case you’re working on a GitHub API, a sample file path would be `components/github/parameters/owner.yaml`, but in case of Notion, there must be a separate folder at the same level, like: `components/notion/parameters/owner.yaml` | if the definition changes, you edit it once and every reference updates automatically. Even for deletion of an API, it becomes far easier to delete the entire folder. |
| **Schema Definition** | Stored within the same folder as parameter. However, in this case, schema definition will store draft requests/response schemas. A sample path would look like: `components/github/schema/issue-response.yaml` | Enables schema re‑use across APIs and tests. |
| **Referncing with** `$ref` | In case of a GitHub API usage, we wire these files together at `apis/github/github-api.yaml` | `$ref` is defined at the endpoint file of that API. |
| **Practical Examples** | Place example payloads under `examples/github/update-issue-request.yaml` (in case of GitHub API). Also, make sure to have different files for success and error examples. It could be something like: `update-issue-validation-error.yaml` and `update-issue-success.yaml` | Study the API and include examples/sample values accordingly. Redoc/Swagger‑UI renders examples into “Try it out” blocks. |

<div data-node-type="callout">
<div data-node-type="callout-emoji">💡</div>
<div data-node-type="callout-text"><strong>Conformance Check </strong>- Run <code>redocly lint openapi.yaml</code> after each addition. This way, you can catch the error right after an update you just made! 🧠</div>
</div>

---

### **Step-4: Linting and Validating the Specification**

* **Why do we lint our docs?**
    

Linting helps with OpenAPI compliance and reports missing fields/schema/example/mismatches, which are required for the API to work. Linting could be done via various tools, and could even be customized with styles and rules to serve your documentation purposes.

* **Set up & Run Redocly CLI:**
    

Install Redocly globally. Make this one-line install `npm install -g @redocly/cli` command for all OS. Once installed, use the tool for linting and validation within the terminal as: `redocly lint openapi.yaml`.

* **Fixing errors after the Linting tool reports them**
    

You’ll first need to understand the structure of the error message. Each comes with an exact error-statement, line number, file name, and a description/hint for fixing it.  
Your next step would be opening that dedicated file, and its line number to find the error, then making suitable change(s) to fix it. Save your changes, and re-run the command to check. Repeat this cycle until you find 0 warnings.

Here’s how linting tools (here Redocly) report errors & validation:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1753485978827/4295c951-a0b6-47ce-9a99-9f84e3215307.png align="center")

---

### **Step-5: Setting Up Local Preview with Docker + Swagger UI**

* **Declaring a Dockerfile:**
    

Use the `swaggerapi/swagger-ui` image create with docker dektop and copy in your OpenAPI spec. This will be configured as the entry point.

#### Build & Run

```plaintext
bashCopyEdit# 1 – Build the image once (re‑run when Dockerfile or YAML changes)
docker build -t api-docs:latest .

# 2 – Launch Swagger‑UI, mapping container port 8080 → host port 8080
docker run --rm -p 8080:8080 api-docs:latest
```

> **Access:** open [http://localhost:8080 to view the interac](http://localhost:8080)tive docs and “Try it out” console.

---

### **Step-6: Generalizing & Repeating the Process for Other APIs**

Repeat the above steps for another API that you’d like to work on. It’s that simple!

Maintaining such a uniform workflow is a professional practice to have consistency, easy maintenance, and scalability in the project.

---

## 👥**Contribution Guidelines**

The following steps answer the question which most beginner contributors might be worried about- “How can collaborators work on this repository?”

**Step-1:** Fork this repository- [https://github.com/trivedi-khushi/openapi-sample-library](https://github.com/trivedi-khushi/openapi-sample-library)

**Step-2:** Create a dedicated Git branch and name it to clearly reflect the specific change you’re working on (e.g., **feature/stripe‑api-add** or **fix/schema‑typo**).

**Step-3:** Follow the structure, guidelines, and flow so far. Work on your contribution.

**Step-4:** Use tools to validate & test your changes.

**Step-5:** Push your changes to the dedicated branch of your forked repository.

**Step-6**: Go to the [main repository](https://github.com/trivedi-khushi/openapi-sample-library). Open a Pull Request (PR) and make it something like `main-branch ← “your-branch-name”`

**Step-7:** Add a valid message & description, and submit a Merge Request(MR) for the same, after the checks are passed.

**Step-8:** Automated checks will pass before submitting your MR. Here’s what to do in each case:

* All checks pass (green)→ PR gets submitted to the reviewer.
    
* Something fails (red) → review the logs, fix, and push again.
    

---

## 🏋️‍♀️Challenges Faced

Here are tabular pointers to list the **Blockers** faced while working on the project, with an explanation of the **issue-faced** and **how were they tackled**.

If you face a new issue while contributing to this project, or working on a similar one, [the reach out to me](https://www.linkedin.com/in/trivedi-khushi) for assistance.

| **Challenge/Blocker** | **Explanation** | **How to Tackle?** |
| --- | --- | --- |
| **1) YAML Schema and Example Mismatches** | Encountered multiple instances where example values did not strictly match the defined schemas, resulting in validation warnings and errors. | (1) Audit the examples to ensure they match the schema definitions exactly, (2) verify no additional unexpected properties exist, (3) include all required fields explicitly. |
| **2) Dockerfile Parsing Errors** | Persistent Dockerfile build errors due to hidden formatting characters. | (1) Read Docker documentation for support, (2) rewrite affected Dockerfile instructions manually, (3) verify with ASCII-only editors. |
| **3) Git Workflow Adjustments** | Line-ending differences between Windows (CRLF) & Unix-based systems (LF). This shows warning as inconsistent file formatting in the repository. | Manage the line-endings using `.gitattributes`. Write & push only a stable development environment for collaborators across all environments. |
| **4) Docker Build Error** | The Docker image failed to build due to `incorrect file references` in the Dockerfile. | This can also occur for issues like `syntax errors`, and `invisible/invalid characters`. Recheck the above errors manually. |
| **5) CI Failure** | Automated workflow (GitHub Actions) can fail due to `invalid YAML`, build `script errors`, or `missing dependencies`. | (1) Check CI logs for error details, (2)Before pushing, re-check with linting tool & validate (3) Update configuration files, example `.github/workflows/` |
| **6) Blank Swagger‑UI page** | The specification path is either incorrect or it’s an empty file | Recheck all the spec endpoint paths again. Make sure there’s no empty file linked inside the main `openapi.yaml` file. |
| **7) Minor Indentation Error in YAML** | parsing error due to formatting or indentation in YAML files. This could be caught in web-editor tools, or in local linting, both. | (1) Track & fix YAML file indentation/formatting. (2) Optionally can use online YAML formatter tool to fix such errors. |
| **8) Port Conflicts When Running Docker** | Docker containers couldn’t start because the local port 8080 was already in use by another process or a previously running container. | Stop that conflicting container/process (`docker stop <container_id>`) OR, run Docker container on a different, available port (e.g., `-p 8081:8080`). |
| **9) Download Instead of API Preview** | While visiting localhost for preview, it downloaded `openapi.yaml` file instead of showing the Swagger-UI/ ReDoc preview. | (1) Check if the correct ENV variable is set (e.g., `SWAGGER_JSON` for Swagger-UI), (2) Check if YAML file is copied into the right location within Docker container. |

## FAQs

<details data-node-type="hn-details-summary"><summary>Can I contribute to this repository?</summary><div data-type="detailsContent">Yes, we’d love to get your contribution here. Propose an API you’d like to work on. submit a GitHub Issue. Upon reviewing, you’d be assigned to work on your chosen API for this!</div></details><details data-node-type="hn-details-summary"><summary>I’m a beginner in open-source. Can I contribute to this project?</summary><div data-type="detailsContent">Sure, this is a beginner-friendly repository❤️. I’d love to assist you with your first contribution. Meanwhile, you can go through my <a target="_self" rel="noopener noreferrer nofollow" href="https://khushitrivedi.hashnode.dev/how-to-git" style="pointer-events: none">“How to Git?” blog </a>to understand v<code>ersion-control</code> and <code>open-source</code> better.</div></details><details data-node-type="hn-details-summary"><summary>What dependencies/installations are needed to set-up a local preview?</summary><div data-type="detailsContent">Here is a short<a target="_self" rel="noopener noreferrer nofollow" href="https://github.com/trivedi-khushi/openapi-sample-library/blob/main/getting-started.mdx" style="pointer-events: none"> getting-started guide</a> for OpenAPI Sample Library. This lists the steps in detail, the installation commands &amp; links, <strong>listing all the commands you’ll be using throughout.</strong></div></details><div data-node-type="callout">
<div data-node-type="callout-emoji">💡</div>
<div data-node-type="callout-text"><strong>Contact - </strong>Reach out for queries, collaboration, or catching-up - <a target="_self" rel="noopener noreferrer nofollow" href="https://x.com/KhushiT113" style="pointer-events: none">Twitter</a> , <a target="_self" rel="noopener noreferrer nofollow" href="https://www.linkedin.com/in/trivedi-khushi/" style="pointer-events: none">LinkedIn</a> , <a target="_self" rel="noopener noreferrer nofollow" href="https://github.com/trivedi-khushi" style="pointer-events: none">GitHub</a> ✨</div>
</div>