## System.out.println("Hi 👋, I'm Stathis!");

```java
import java.util.List;

public class Stathis extends Person implements SoftwareEngineer, Graduate {
    private final ProfileConfig config = JsonLoader.load("profile.json", ProfileConfig.class);

    @Override
    public String getAlmaMater() {
        return "University of Piraeus (Department of Informatics)";
    }

    @Override
    public String getSpecialization() {
        return "Software Technologies & Intelligent Systems";
    }

    @Override
    public String getDegreeStatus() {
        return "Build succeeded: 🎓";
    }

    @Override
    public List<String> getMainStack() {
        return List.of("Java", "Spring Boot", "Android SDK", "C#", ".NET");
    }

    @Override
    public List<String> getSecondaryStack() {
        return List.of("SQL", "NoSQL", "Docker", "Jenkins", "Git");
    }

    @Override
    public String getCurrentFocus() {
        return config.status();
    }
}

// utils
public record ProfileConfig(String purpose, String status, String linkedIn) {}

interface Graduate {
    String getAlmaMater();
    String getSpecialization();
    String getDegreeStatus();
}

interface SoftwareEngineer {
    List<String> getMainStack();
    List<String> getSecondaryStack();
    String getCurrentFocus();
}
```

### `profile.json`
```json
{
  "purpose": "Hosting my personal projects",
  "status": "Currently focused on development with Java/Sprin Boot",
  "linkedIn_profile": "Stathis Panagiotis Athanasakos"
}
```
