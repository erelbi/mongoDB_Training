---
description: $and $or $nor $not
---

# Logic Operators

| Operatör | Açıklaması |
| :--- | :--- |
| $and | Match all of the specified query clauses |
| $or | At least one of the query clauses is matched |
| $nor | Fail to match both given clauses |
| $not | Negates the query requirement |

![](.gitbook/assets/logic.png)

### $nor example

![](.gitbook/assets/nor.png)

{% hint style="info" %}
{$nor:\[{watlev:"always dry"},{watlev:"always under water/submerged"},{watlev:"covers and uncovers"}\]}
{% endhint %}



