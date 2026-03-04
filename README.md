# tippitytappity-design

tippitytappity is a program to practice typing


## Data model

```mermaid
classDiagram
  Results <|-- Stats
  Users <|-- Results
  class Stats{
        - Words_Typed: int
        - Num_Wrong: int
        - Total_Words: int
        + set_Stats(user: int, int, int)
        + get_Words() int
        + get_Wrong() int
        + get_Total() int
  }
  class Results{
        - Work_Stats: Stats
        + get_WPM() int
        + get_Percent() int
  }
  class Users{
        - Previous_Tests[]: Results
        - Name: string
        + get_Name() string
        + get_Results() Results[]
  }
```
