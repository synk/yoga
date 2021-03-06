---
path: "docs/flex"
title: "Flex Basis, Grow, and Shrink"
hasPlayground: true
editableProperties: ['flexGrow', 'flexShrink', 'flexBasis']
---

## Flex Basis, Grow, and Shrink

### Flex Grow

Flex grow describes how any space within a container should be distributed
among its children along the main axis. After laying out its children, a container will
distribute any remaining space according to the flex grow values specified by its children.

flex grow accepts any floating point value >= 0, with 0 being the default value.
A container will distribute any remaining space among its children weighted by the child’s flex grow value.

### Flex Shrink

Flex shrink describes how to shrink children along the main axis in the
case that the total size of the children overflow the size of the container on the main axis.
flex shrink is very similar to flex grow and can be thought of in the same way if
any overflowing size is considered to be negative remaining space.
These two properties also work well together by allowing children to grow and shrink as needed.

flex shrink accepts any floating point value >= 0, with 1 being the default value.
A container will shrink its children weighted by the child’s flex shrink value.

### Flex Basis

Flex basis is an axis-independent way of providing the default size of an item
along the main axis. Setting the flex basis of a child is similar to setting the Width of that
child if its parent is a container with FlexDirection = row or setting the Height of a child
if its parent is a container with FlexDirection = column. The flex basis of an item is the 
efault size of that item, the size of the item before any flex grow and flex shrink
calculations are performed.
