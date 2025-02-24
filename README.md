# Unexpected Behavior with Falsy Values in JavaScript

This repository demonstrates a subtle bug in a JavaScript function that deals with null and undefined values. The function uses loose equality (==) which can lead to unexpected results when comparing with other falsy values like 0 or false. 

## Bug Description

The `foo` function is designed to return specific strings for null and undefined inputs. However, due to loose equality, it might not distinguish between these and other falsy values, leading to unintended behavior.

## Solution

The solution uses strict equality (===) to avoid type coercion and ensures that the function behaves as intended, handling only null and undefined correctly.