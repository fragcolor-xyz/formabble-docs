---
authors: Formabble & contributors
license: CC-BY-SA-4.0
---


# Tensor.Split

<div class="sh-parameters" markdown="1">
| Name | Mandatory | Description | Default | Type |
|------|---------------------|-------------|---------|------|
| `⬅️ Input` ||The input of the shard, if any | | [`Object`](../../types/#object) |
| `Output ➡️` ||The resulting output of the shard | | [`[Object]`](../../types/#seq) |
| `Dim` | :fontawesome-solid-circle-plus:{title="No"} No  | The dimension along which to split the tensor. Default is 0. | `0` | [`Int`](../../types/#int)[`Var(Int)`](../../types/#contextvar)[`None`](../../types/#none) |
| `Size` | :fontawesome-solid-circle-xmark:{title="Yes"} Yes  | The size of the sections to split the tensor into. | `None` | [`Int`](../../types/#int)[`Var(Int)`](../../types/#contextvar) |

</div>

Splits a tensor into multiple tensors along a specified dimension.

--8<-- "includes/license.md"
