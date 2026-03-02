# tippitytappity-design

tippitytappity is a program to practice typing


## Data model

```mermaid
classDiagram
  Stats <|-- Results
  class Stats{
        - Words: int
        - NumWrong: int
        - StringLength: int
        + get_Words() int
        + get_Wrong() int
        + get_Total() int
  }
  class Results{
        - badges vector~string~
        + get_WPM() int
        + get_Percent() int
  }
```
