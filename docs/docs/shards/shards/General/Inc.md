---
authors: Formabble & contributors
license: CC-BY-SA-4.0
---


# Inc

<div class="sh-parameters" markdown="1">
| Name | Mandatory | Description | Default | Type |
|------|---------------------|-------------|---------|------|
| `⬅️ Input` ||Any valid integer(s), floating point number(s), or a sequence of such entities supported by this operation. | | [`Any`](../../types/#any) |
| `Output ➡️` ||The result of the operation, usually in the same type as the input value. | | [`Any`](../../types/#any) |
| `Value` | :fontawesome-solid-circle-xmark:{title="Yes"}  | The value to apply the operation to. | `None` | [`&Int`](../../types/#contextvar)[`&Int2`](../../types/#contextvar)[`&Int3`](../../types/#contextvar)[`&Int4`](../../types/#contextvar)[`&Int8`](../../types/#contextvar)[`&Int16`](../../types/#contextvar)[`&Float`](../../types/#contextvar)[`&Float2`](../../types/#contextvar)[`&Float3`](../../types/#contextvar)[`&Float4`](../../types/#contextvar)[`&Color`](../../types/#contextvar)[`&[Any]`](../../types/#contextvar) |

</div>

Applies the unary operation on the input value and returns the result (or a sequence of results if the input and the operand are sequences).

--8<-- "includes/license.md"
