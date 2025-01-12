# CSS Flexbox space-between Overflow Issue

This repository demonstrates a subtle bug related to using `justify-content: space-between;` in CSS flexbox layouts when the total width of flex items exceeds the container's width.

## Problem

The provided CSS intends to distribute space evenly between flex items using `space-between`.  However, when the combined width of the items surpasses the container's width, the items might overflow, defying expectations.

## Solution

The solution involves adding `width: auto;` to the flex items, allowing the flexbox layout to determine the optimal width based on available space. This prevents overflow, maintaining the intended spacing.