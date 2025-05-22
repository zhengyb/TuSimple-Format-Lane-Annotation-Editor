# Lane Annotation Guidelines

## Principles
- Annotate up to **4 lane lines** closest to the vehicle's center. Typically: Left-Left, Left, Right, Right-Right;
- **Start/End positions**: Cover as much of the reference line as possible; for areas near the bottom of the image, use reasonable inference when necessary;
- **Road edges**: If fewer than 4 lane lines are visible, the road edge should be treated as a lane line;
- **Splits**: Should be annotated as 2 separate lane lines; these two lines share the same starting point but have different endpoints;
- **Merges**: Should be annotated as 2 separate lane lines; these two lines share the same endpoint but have different starting points;
- **Occlusion/Blur**: Use reasonable inference to complete the lane lines based on the context;

## Practical Tips
- First label the start point, end point, and key turning points, then use interpolation tools in the software to auto-complete the rest;
- For curved lane lines, label as many key points as possible to ensure the final lane closely matches the real-world curvature;
- How to modify: Clear all pixel points of the lane → re-annotate the key points. You don’t need to delete and re-add the lane line. This keeps the lane’s position and color in the list unchanged.
