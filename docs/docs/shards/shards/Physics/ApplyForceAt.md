---
authors: Formabble & contributors
license: CC-BY-SA-4.0
---


# Physics.ApplyForceAt

<div class="sh-parameters" markdown="1">
| Name | Mandatory | Description | Default | Type |
|------|---------------------|-------------|---------|------|
| `⬅️ Input` ||The physics body to apply the force to. | | [`Physics.Body`](../../types/#physics.body) |
| `Output ➡️` ||Outputs the input physics body with the force applied. | | [`Physics.Body`](../../types/#physics.body) |
| `Force` | :fontawesome-solid-circle-plus:{title="No"} No  | The force to apply represented as a float3 containing the magnitude and direction of the force. | `@f3(0 0 0)` | [`Float3`](../../types/#float3)[`Var(Float3)`](../../types/#contextvar) |
| `Position` | :fontawesome-solid-circle-plus:{title="No"} No  | The position to apply the force at represented as a float3 | `@f3(0 0 0)` | [`Float3`](../../types/#float3)[`Var(Float3)`](../../types/#contextvar) |

</div>

Applies a force to the physics body at a specific location

--8<-- "includes/license.md"

