![cms diagram png](cms_diagram_canvas-1.png)


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

| Component   | Add           | Hide          | Modify        |
| ----------- | ------------- | ------------- | ------------- |
| Section     | at risk       | supported     | at risk       |
| Feature     | at risk       | at risk       | supported     |
| Page        | supported     | supported     | not supported |
| Block       | not supported | not supported | supported     |
| Component   | not supported | not supported | supported     |
