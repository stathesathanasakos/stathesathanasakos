## MessageBox.Show("Hi 👋, my name is Stathis!");

```csharp
public class Stathis : Person, IStudent
{
    public string University => "University of Piraeus (Dept. of Informatics)";
    public string Specialization => "Software Technologies & Intelligent Systems";
    public string CurrentStatus => "BSc Degree compiling... 🎓";

    // My own properties
    public List<string> MainStack => new() { "C#", "ASP.NET", "Java", "Android SDK" };
    public List<string> SecondaryStack => new() { "Python", "SQL", "NoSQL", "Firebase" };
}

public interface IStudent
{
    string University { get; }
    string Specialization { get; }
    string CurrentStatus { get; }
}
```

```json
{
  "purpose": "Hosting my personal projects",
  "bugs_included": true,
  "status": "Refactoring my life, one commit at a time",
  "linkedIn_profile": "Stathis Panagiotis Athanasakos"
}
```
