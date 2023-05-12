SonarQube docker build. (See docker-compose.yml)

## Instructions
Run `docker-compose -up -d` to install and run sonarqube server and database
```
    In your browser, connect to http://127.0.0.1:9000
    Default
        Username = admin
        Password = admin
```
Install and Run SonarScanner from zip file. Follow [guide](https://docs.sonarqube.org/latest/analyzing-source-code/scanners/sonarscanner/)

Run the following command from the project base directory to launch analysis and pass your authentication token:
````
	sonar-scanner -Dsonar.token=myAuthenticationToken
````

Store the auth token in an env file in the project base directory for recurring use

Install SonarLint extension [source](https://marketplace.visualstudio.com/items?itemName=SonarSource.sonarlint-vscode) to integrate SonarQube Server with linter from SonarQube