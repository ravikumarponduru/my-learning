# 🛠️ Java 21 + IntelliJ IDEA Setup Guide (Windows)

Start your Core Java journey by setting up Java 21 and IntelliJ IDEA properly.

---

## ✅ Step 1: Install Java 21 JDK (Java Development Kit)

1. **Download Java JDK 21**  
   - Use one of these links:
     - [Oracle JDK 21](https://www.oracle.com/java/technologies/javase/jdk21-archive-downloads.html)
     - [Adoptium Temurin OpenJDK 21](https://adoptium.net/en-GB/temurin/releases/?version=21)

2. **Install Java 21**  
   - Download the `.msi` or `.exe` installer (Windows x64).
   - Run the installer and follow the steps.

3. **Set Environment Variables** *(optional but recommended)*  
   - Open: `Start Menu → Edit the system environment variables`
   - Click `Environment Variables…`
     - Add system variable:  
       - `JAVA_HOME = C:\Program Files\Java\jdk-21`
     - Edit `Path`:
       - Add: `%JAVA_HOME%\bin`

4. **Verify Installation**  
   Open Command Prompt and run:
   ```bash
   java -version
   ```
   You should see something like:
   ```
   java version "21.0.1"
   ```

---

## ✅ Step 2: Install IntelliJ IDEA (Community Edition)

1. **Download IntelliJ IDEA**  
   - [IntelliJ IDEA Download Page](https://www.jetbrains.com/idea/download)
   - Choose **Community Edition** (free)

2. **Install IntelliJ**  
   - Run the installer
   - Recommended options:
     - ✅ Add “Open Folder as Project”
     - ✅ Create Desktop Shortcut
     - ✅ (Optional) Add to PATH

3. **Launch IntelliJ IDEA**

---

## ✅ Step 3: Configure Java SDK in IntelliJ

1. Click **New Project**
2. Choose **Java** as the project type
3. If no SDK is detected:
   - Click **Add SDK → JDK**
   - Navigate to your installed JDK path (e.g., `C:\Program Files\Java\jdk-21`)
4. Name the project and click **Finish**

---

## ✅ Step 4: Run Your First Java Program

1. In the `src` folder:
   - Right-click → **New → Java Class**
   - Name it `HelloWorld`
2. Paste this code:
   ```java
   public class HelloWorld {
       public static void main(String[] args) {
           System.out.println("Hello, Java 21!");
       }
   }
   ```
3. Right-click in the editor → **Run 'HelloWorld.main()'**

Expected Output:
```
Hello, Java 21!
```

---
