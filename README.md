# DocumentationDemo

<h1 align="center">Welcome to <%= projectName %> 👋</h1>
<p>
This repository was created for a demonstration of the new Documentation templates, methodologies and styles.
<br>
It was automatically generated using the [ReadME Generator] (https://github.com/kefranabg/readme-md-generator) using Github Actions. 
  <br>
  


### 🏠 [Homepage](<%= projectHomepage %>)
<% } -%>
<% if (projectDemoUrl) { -%>

### ✨ [Demo](<%= projectDemoUrl %>)
<% } -%>
<% if (projectPrerequisites && projectPrerequisites.length) { -%>

## Prerequisites

<% projectPrerequisites.map(({ name, value }) => { -%>
- <%= name %> <%= value %>
<% }) -%>
<% } -%>
<% if (installCommand) { -%>

## Install

```sh
<%= installCommand %>
```
<% } -%>
<% if (usage) { -%>

## Usage

```sh
<%= usage %>
```
<% } -%>
<% if (testCommand) { -%>

## Run tests

```sh
<%= testCommand %>
```
<% } -%>


## Author
<% if (authorName) { %>
👤 **<%= Sarah McGeough %>**
<% }

## 🤝 Contributing

Contributions, issues and feature requests are welcome!<br />

***
<%- include('footer.md'); -%>
