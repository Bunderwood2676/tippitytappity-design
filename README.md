# tippitytappity-design

tippitytappity is a program to practice typing


## Data model

```mermaid
classDiagram
   TippityTappity..> Account
   TippityTappity<|-- Phrases
   TippityTappity<|-- Accuracy
   TippityTappity<|-- Result
   TippityTappity<|-- History
  class TippityTappity{
        - Account: string
        - Phrase: string
        - Accuracy: string
        - Result: string
        + Accurate(Correct: string, incorrect: string) boolean
        + get_accuracy() int
        + get_phrase() string
        + get_account() string
        + get_history() string
  }
  class History{
        - History string
        + get_phrase string
        + add_phrase(phrase: string)

  class Account{
        - Account string
        - Password int
        + get_username() string
        + get_password() int
  }
  class Phrases{
        - Account string
        - Phrase string
        + get_account() string
        + add_phrase(phrase: string)
        + get_phrase() string
  }

  class Accuracy{
        - AccuracyPercentage int
        + get_AccuracyPercentage() int
  }

  class Result{
        - Result string
        + get_pass() string
        + get_fail() string
  }
        
```
