# Components Diagram
> One example "Section" contains one or more "Features". Each "Feature" contains one or more "Pages". Each "Page" contains one or more "Blocks". Each "Block" contains one or more "Components". The CMS allows for adding, hiding, and modifying these components, but the scope of what is included in the base project varies by component type. For details on what is included in the base scope, please refer to: [Scope Summary v1](../SCOPES/PRD_6K.md#scope-summary-v1)

```mermaid
flowchart TD
	n_section["Section"]
	n_feature["Feature"]

	n_page_left["Page"]
	n_page_right["Page"]

	n_block_left_a["Block"]
	n_block_left_b["Block"]
	n_block_right_a["Block"]
	n_block_right_b["Block"]
	n_block_nested["Block"]

	n_component_left_a["Component"]
	n_component_left_b["Component"]
	n_component_right_a["Component"]
	n_component_right_b["Component"]

	n_section --> n_feature
	n_feature --> n_page_left
	n_feature --> n_page_right

	n_page_left --> n_block_left_a
	n_page_left --> n_block_left_b
	n_page_right --> n_block_right_a
	n_page_right --> n_block_right_b

	n_block_left_a --> n_component_left_a
	n_block_left_b --> n_component_left_b
	n_block_right_a --> n_block_nested
	n_block_right_b --> n_component_right_b
	n_block_nested --> n_component_right_a
```

## Legend

| Component       | Add           | Hide          | Modify        |
| --------------- | ------------- | ------------- | ------------- |
| **Section**     | at risk       | supported     | at risk       |
| **Feature**     | at risk       | at risk       | supported     |
| **Page**        | supported     | supported     | not supported |
| **Block**       | not supported | not supported | supported     |
| **Component**   | not supported | not supported | supported     |
