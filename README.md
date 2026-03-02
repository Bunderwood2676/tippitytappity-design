# tippitytappity-design

tippitytappity is a program to practice typing


## Data model

```mermaid
classDiagram
   TippityTappity<|-- Phrases
   TippityTappity<|-- Accuracy
  class TippityTappity{
        - Phrase: string
        - Accuracy: string
        + Accurate(Correct: string, incorrect: string) boolean
        + get_accuracty() int
        + get_phrase() string
  }
  class Phrases{
        - Phrase string
        + add_phrase(phrase: string)
        + get_phrase() string
  }

  class Accuracy{
}
        
```
