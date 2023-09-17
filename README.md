# MyGoWebAppTemplate

<p>
   <a href="http://makeapullrequest.com"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat" alt=""></a>
   <a href="https://golang.org"><img src="https://img.shields.io/badge/Made%20with-Go-1f425f.svg" alt="made-with-Go"></a>
   <a href="https://goreportcard.com/report/github.com/goodnessuc/MyGoWebAppTemplate"><img src="https://goreportcard.com/badge/github.com/goodnessuc/MyGoWebAppTemplate" alt="GoReportCard"></a>
   <a href="https://github.com/goodnessuc/MyGoWebAppTemplate"><img src="https://img.shields.io/github/go-mod/go-version/goodnessuc/MyGoWebAppTemplate.svg" alt="Go.mod version"></a>
   <a href="https://github.com/goodnessuc/MyGoWebAppTemplate/blob/master/LICENSE"><img src="https://img.shields.io/github/license/goodnessuc/MyGoWebAppTemplate.svg" alt="LICENSE"></a>
</p>

## 🗞️ Introduction

This is a template for initializing Go apps with the hexagonal structure according to the best practices as overviewed
through the community.

You're going to find this useful if you're building an app that you intend to use and support over a long period of
time.

## ⚠️ Understanding the Structure

First, you're going to tweak this structure for your app's use case. This template simply eliminates the overhead of
manually initializing a project.

Certainly, here's the directory explanation with clickable links for your GitHub README.md:


1. **[cmd](./cmd)**: This directory contains the main entry point for your server application.
    - **[server](./cmd/server)**: Subdirectory for the server application.
        - **[main.go](./cmd/server/main.go)**: The main Go source code file for your server application.

2. **[config](./config)**: This directory stores configuration files for your application.
    - **[config.yaml](./config/config.yaml)**: Configuration settings and parameters.

3. **[docs](./docs)**: Documentation related to your project.
    - **[Getting Started.md](./docs/Getting%20Started.md)**: Instructions on how to get started with your application.

4. **[internal](./internal)**: Contains internal application code not meant to be exposed as a public API.
    - **[handlers](./internal/handlers)**: Subdirectory for request handlers.
        - **[handlers.go](./internal/handlers/handlers.go)**: Code for defining and implementing request handlers.
    - **[utils](./internal/utils)**: Subdirectory for utility functions.
        - **[utils.go](./internal/utils/utils.go)**: Utility functions used within the application.

5. **[scripts](./scripts)**: Contains scripts for automating various tasks.
    - **[PushaG.sh](./scripts/PushaG.sh)**: A script for a task named "PushaG."
    - **[creator.sh](./scripts/creator.sh)**: A script that might be related to creating something for your application.

6. **[static](./static)**: Contains static assets like images.
    - **[img.jpg](./static/img.jpg)**: An image file used in your application.


Each of these subdirectories serves a specific purpose in organizing your application's code and resources. The
structure helps keep your codebase modular and maintainable by separating concerns and functionalities into different
directories.

## 🏁 Getting Started

You can use the `gonew` command or the bash [creator.sh](./scripts/creator.sh) script to initialize this project.

### 🤩 Using Gonew

Using `gonew` will ensure that you also get additional file and file content. Google `gonew` and check the LogRocket
blog for a tutorial I wrote on how you can use `gonew` to streamline your apps' development.


First, Install `gonew` with this command line


```shell
go install golang.org/x/tools/cmd/gonew@latest
```

Next, run this command to complete the setup with `gonew` and start building.


```shell

gonew -dir <directory-you-want> -v github.com/Goodnessuc/MyGoWebAppTemplate <your-project-name>

```


The command will create the exact structure of the project as is on GitHub.

### ⚙️ Using the Bash Script

Using the [creator.sh](./scripts/creator.sh) bash script is a fast alternative to getting started.

The bash script also affords you more control over the contents of your app files in a minimalistic manner

Run this command in the terminal of your project's working directory to create the directory structure and files


```bash
mkdir -p cmd/server config internal/handlers internal/utils scripts static docs

touch .gitignore LICENSE Makefile README.md Dockerfile .env.example go.mod go.sum scripts/PushaG.sh

```


You've successfully set up your project's structure with the Bash Script.


## 🛠️ Technologies and Tools
Go - The programming language used

GitHub Actions - GitHub CI/CD tool

Make - Build automation tool



## 👏 Contributing
Contributions are welcome! Feel free to open a pull request right away.

## 📃 License
This project is licensed under the MIT License - see the LICENSE.md file for details