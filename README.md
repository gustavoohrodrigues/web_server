# Ansible Role: Web Server

This Ansible role installs and configures a web server environment automatically.

The role is designed to be reusable and can be integrated into infrastructure automation pipelines or configuration management workflows.

---

## 📌 Overview

The **web_server** role automates the installation and configuration of a web server stack in Linux environments.

It is commonly used to deploy application servers inside automated infrastructure environments.

---

## 🚀 Features

* Automated web server installation
* Web service configuration
* Ready for infrastructure automation
* Compatible with Ansible Galaxy roles

---

## 🧰 Requirements

* Ansible >= 2.9
* Linux host (Ubuntu, Debian, CentOS, Rocky, AlmaLinux)

---

## 📂 Role Structure

```
web_server/
├── tasks
│   └── main.yml
├── handlers
│   └── main.yml
├── templates
│   └── *.j2
├── defaults
│   └── main.yml
├── vars
│   └── main.yml
├── meta
│   └── main.yml
```

---

## ⚙️ Role Variables

Example variables:

```yaml
web_server_port: 80
web_server_root: /var/www/html
```

Variables can be customized in:

```
defaults/main.yml
vars/main.yml
```

---

## ▶️ Example Playbook

```yaml
- hosts: webservers
  become: true
  roles:
    - gustavoohrodrigues.web_server
```

---

## 📦 Installation via Ansible Galaxy

```bash
ansible-galaxy install gustavoohrodrigues.web_server
```

---

## Author

**Gustavo Henrique Rodrigues**

LinkedIn
https://www.linkedin.com/in/gustavo-henrique-rodrigues-3070a5260

---

## 📜 License

MIT
