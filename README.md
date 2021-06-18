class Student

    {    
         private string name = "Dan";
         private string school = "University of Advancing Technology";
         private string major = "Game Programming"
         
         private int totalCreditsToGraduate = 120;
         private int currentCredits = 111;         
  
  
         void CalculateGraduation(int credits)
         {
              if (currentCredits < totalCreditsToGraduate)
              {
                  currentCredits += credits;
              }
              else if (currentCredits >= totalCreditsToGraduate)
              {
                  Console.WriteLine("GRADUATION!");
              }
         }
    }

class Programmer : Student

    {
         private string[] programmingLanguages = { "C#", "C++", "Python" };
         private string[] gameEngines = { "Unity", "UE4" };
         private string[] futureInterests = { "AR", "MR", "XR", "VR", "AI" };
         
         
         void FindProgrammingCareer()
         {
              foreach (string language in programmingLanguages)
              {
                   ProgrammingCareer.FindEntryLevelPosition(language);
              }
         }
    }
