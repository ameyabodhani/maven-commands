### **Maven Commands List**  

#### **Cleaning & Building**  
```bash
mvn clean                     # Deletes the target/ directory and compiled files  
mvn package                   # Compiles, tests, and packages the project (JAR/WAR)  
mvn install                   # Compiles, tests, and installs the artifact in the local repo  
mvn clean install             # Cleans and then installs the project  
mvn clean install -U          # Cleans, installs, and forces dependency updates  
mvn clean package             # Cleans and then packages the project  
mvn clean deploy              # Cleans, builds, and deploys the artifact to a remote repository  
```

#### **Compilation & Execution**  
```bash
mvn compile                   # Compiles the source code (src/main/java)  
mvn test-compile              # Compiles test classes (src/test/java)  
mvn exec:java -Dexec.mainClass="com.example.Main"   # Runs a Java class with main() method  
```

#### **Testing & Verification**  
```bash
mvn test                      # Runs unit tests  
mvn verify                    # Runs integration tests and checks build validity  
mvn clean verify              # Cleans and then verifies the build  
```

#### **Dependency Management**  
```bash
mvn dependency:tree           # Displays project dependencies in a tree format  
mvn dependency:resolve        # Resolves and downloads dependencies  
mvn dependency:analyze        # Analyzes unused and declared dependencies  
mvn versions:display-dependency-updates  # Shows available dependency updates  
```

#### **Project Information & Debugging**  
```bash
mvn help:effective-pom        # Displays the effective POM after applying inheritance  
mvn help:effective-settings   # Shows the effective Maven settings.xml configuration  
mvn validate                  # Validates the project structure and POM  
```

#### **Plugin & Profile Management**  
```bash
mvn help:describe -Dplugin=plugin-name   # Describes details about a plugin  
mvn help:active-profiles                 # Lists active Maven profiles  
mvn -Pprofile-name clean install         # Runs Maven with a specific profile  
```

#### **Skipping Tests**  
```bash
mvn clean install -DskipTests  # Skips test execution but compiles them  
mvn clean install -Dmaven.test.skip=true  # Skips compiling and running tests  
```

#### **Forcing Updates & Offline Mode**  
```bash
mvn clean install -U          # Forces dependency updates from remote repositories  
mvn clean package -o          # Runs Maven in offline mode  
```

