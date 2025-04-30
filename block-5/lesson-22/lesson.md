# Lesson 22: Algorithms: Search and Evaluation

## Topics
- Nearest point search algorithm (Euclidean distance)
- Implementation in Python

## Notes
Algorithms are a set of instructions or rules designed to solve a specific problem or perform a specific task. In this lesson, we will focus on the nearest point search algorithm using Euclidean distance and its implementation in Python.

### Nearest Point Search Algorithm
The nearest point search algorithm is used to find the closest point to a given reference point from a set of points. The Euclidean distance is commonly used to measure the distance between two points in a Euclidean space.

### Euclidean Distance
The Euclidean distance between two points \( P(x_1, y_1) \) and \( Q(x_2, y_2) \) in a 2D space is calculated as:
\[ d(P, Q) = \sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2} \]

### Implementation in Python
Here is an example of how to implement the nearest point search algorithm using Euclidean distance in Python:

```python
import math

def euclidean_distance(point1, point2):
    return math.sqrt((point2[0] - point1[0])**2 + (point2[1] - point1[1])**2)

def find_nearest_point(reference_point, points):
    nearest_point = None
    min_distance = float('inf')
    
    for point in points:
        distance = euclidean_distance(reference_point, point)
        if distance < min_distance:
            min_distance = distance
            nearest_point = point
    
    return nearest_point

# Example usage
reference_point = (2, 3)
points = [(1, 2), (4, 6), (5, 1), (2, 4)]
nearest_point = find_nearest_point(reference_point, points)
print(f"The nearest point to {reference_point} is {nearest_point}")
```

In this example, the `euclidean_distance` function calculates the Euclidean distance between two points, and the `find_nearest_point` function finds the nearest point to the given reference point from a list of points.

By understanding and implementing the nearest point search algorithm using Euclidean distance, we can solve various problems that require finding the closest point in a given set of points.
