# PHP Loose Comparison Pitfall

This repository demonstrates a common, yet easily overlooked, error in PHP related to loose comparison (`==`) when comparing strings and integers.  The code showcases how the comparison `'0' == 0` evaluates to `true`, which can lead to unexpected and incorrect program behavior.

## Problem

PHP's loose comparison (`==`) does not check for type equality. This means that a string '0' is considered equal to an integer 0, which can cause logic errors in conditional statements.

## Solution

Always use strict comparison (`===`) when comparing values to ensure both type and value are identical.  This eliminates ambiguity and avoids unexpected results.