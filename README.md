# Terraform Jenkins Pipeline Demo

This project creates **two files** and **two directories** using Terraform via a Jenkins pipeline.

---

### Structure

- `main.tf` – Terraform code to create files/directories using `local_file` resource  
- `Jenkinsfile` – CI pipeline to run Terraform stages (`init`, `validate`, `plan`, `apply`)

---

### How to Use

1. Connect this repo to Jenkins (Pipeline script from SCM)
2. Run the pipeline
3. Check Jenkins workspace – it will contain:
    ```
    file1.txt
    file2.txt
    dir1/.placeholder
    dir2/.placeholder
    ```

---

### Requirements

- Jenkins with Git and Terraform installed  
- GitHub SCM access
