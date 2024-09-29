**Declarative Pipelines** in Jenkins are written in **Groovy**, just like Scripted Pipelines. However, the syntax for Declarative Pipelines is much simpler, more structured, and human-readable compared to the fully scriptable nature of Scripted Pipelines.

Even though Declarative Pipelines are written in Groovy, you don’t need deep knowledge of Groovy to use them. The Declarative Pipeline syntax is designed to be beginner-friendly, with predefined blocks like `pipeline`, `agent`, `stages`, `steps`, and `post`.

### Example of Declarative Pipeline (written in Groovy):

```groovy
pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
    }
}
```

### Key Points:
- **Groovy Language**: Declarative Pipeline is still based on Groovy, but the syntax is simplified to make pipeline definitions easier and more structured.
- **Structured Blocks**: It uses blocks like `pipeline`, `agent`, `stages`, and `steps` to organize the pipeline in a more readable format, even though it's Groovy code under the hood.

Declarative Pipeline is easier to use and designed for most common CI/CD workflows without needing to dive deep into Groovy programming.


