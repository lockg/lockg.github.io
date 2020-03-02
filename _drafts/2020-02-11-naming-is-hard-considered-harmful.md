---
title: "“Naming is hard” considered harmful"
tags: [c++, naming]
abstract: "Is good naming inherently hard - or is it a design smell?<br/>
  Does good design beget good naming?"
---

Let's start by taking as given that good naming is important. Many
people smarter than I have already covered this, and *this* article is
not about persuading the unconvinced.

Next — I was inspired to actually sit down and commit my thoughts
to text after watching Kate Gregory's[^1] excellent
[“Naming is Hard: Let's Do Better”](https://www.youtube.com/watch?v=MBRoCdtZOYg "Kate Gregory at CppCon 2019")
talk from CppCon 2019. I highly recommend it.

Good naming *should* be easy. We should be able to name a thing — a
variable, function, class, module, etc. — just by describing what it
is or what it does, right? Some easy examples:

``` C++
  class Invoice {
  public:
    currency GetAmountDue() const;
    void MarkAsPaid(time_point When);
    bool IsPaid() const;
  }
```

`class Invoice`

Classes model things — real-world things. This class
is the model of an invoice. Each instance of this class represents an
actual, real-world invoice. If you were new to OOP, you could be
excused for thinking of the class as just a collection of code that
manages the details of an invoice”. You might wonder if you should
call it `InvoiceDetailManager`. That would be a bad name, but you
didn't choose it because naming is hard — you chose it because you
weren't thinking OOP.


# End of test sample

[^1]: Kate's deets
