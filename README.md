# tippitytappity-design

tippitytappity is a program to practice typing


## Data model

```mermaid
classDiagram
   TippityTappity<|-- Phrases
   TippityTappity<|-- Accuracy
   TippityTappity<|-- Result
  class TippityTappity{
        - Phrase: string
        - Accuracy: string
        - Result: string
        + Accurate(Correct: string, incorrect: string) boolean
        + get_accuracy() int
        + get_phrase() string
  }
  class Phrases{
        - Phrase string
        + add_phrase(phrase: string)
        + get_phrase() string
  }

  class Accuracy{
        - Accuracy int
        + get_AccuracyPercentage() int
  }

  class Result{
        - Result string
        + get_pass() string
        + get_fail() string
  }
        
```
