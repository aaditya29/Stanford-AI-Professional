# Notes of CS221: Artificial Intelligence Principles and Techniques

## Lecture-0: Overview

### Gradient Descent

Imagine you're trying to find the lowest point in a hilly landscape while blindfolded. Gradient descent is like a systematic method of exploring that landscape to find the absolute lowest point, which in mathematical terms represents the minimum of a function.

#### The Basic Intuition

At its core, gradient descent is an iterative optimization algorithm used to find the minimum of a cost function. Think of a cost function as a measure of how "wrong" your current solution is. The goal is to minimize this wrongness by taking smart steps in the right direction.

Let's break down the key components:

1. **Starting Point**: You begin at some initial point on your mathematical "landscape".

2. **Calculating the Gradient**: The gradient tells you two crucial things:

   - The direction of the steepest increase
   - How steep that increase is

3. **Taking Steps**: You move in the opposite direction of the gradient, which means going downhill towards the minimum point.

### A Simple Mathematical Analogy

Imagine you're walking down a hill with your eyes closed. At each step, you:

- Feel the slope beneath your feet
- Determine which way is steepest downhill
- Take a small step in that direction
- Repeat until you can't go any lower

In mathematical terms, this means:

- Calculate the derivative (slope) at your current point
- Move a small distance in the opposite direction of that slope
- Recalculate and repeat

#### Mathematical Concepts Required for Gradient Descent

To fully understand gradient descent, it's essential to grasp a few key mathematical concepts:

#### 1. Derivatives

A derivative represents the rate at which a function is changing at any given point. In the context of gradient descent, the derivative (or gradient in multiple dimensions) helps us understand the slope of the cost function.

- **Notation**: If \( f(x) \) is our function, the derivative is denoted as \( f'(x) \) or \( \frac{df}{dx} \).

#### 2. Partial Derivatives

When dealing with functions of multiple variables, partial derivatives come into play. They measure how the function changes as each variable changes, holding the other variables constant.

- **Notation**: For a function $( f(x, y))$, the partial derivatives are $( \frac{\partial f}{\partial x})$ and \( $frac{\partial f}{\partial y})$.

#### 3. Gradient

The gradient is a vector that contains all the partial derivatives of a function. It points in the direction of the steepest ascent.

- **Notation**: For a function $( f(x, y))$, the gradient is $( \nabla f = \left( \frac{\partial f}{\partial x}, \frac{\partial f}{\partial y} \right))$.

#### 4. Learning Rate

The learning rate is a crucial hyperparameter in gradient descent. It determines the size of the steps we take towards the minimum. A learning rate that's too high can cause overshooting, while one that's too low can make the process painfully slow.

- **Notation**: The learning rate is often denoted by $( \alpha )$ or $( \eta )$.

#### 5. Convergence

Convergence refers to the process of approaching the minimum of the cost function. In gradient descent, we iteratively update our parameters until the changes become negligibly small, indicating that we've reached (or are very close to) the minimum.

By understanding these concepts, you'll have a solid foundation for grasping how gradient descent works and why it's such a powerful optimization technique.
