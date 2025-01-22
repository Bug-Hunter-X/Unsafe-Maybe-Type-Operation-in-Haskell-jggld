# Haskell Maybe Type Unsafety

This repository demonstrates a common error in Haskell programming involving unsafe operations on `Maybe` types.  The `bug.hs` file contains code that attempts to add a `Just` value to a `Nothing` value without proper error handling, resulting in a runtime error. The `bugSolution.hs` file provides a corrected version using pattern matching to safely handle the `Maybe` types.

The issue is that the `+` operator is not directly defined for `Maybe` types. Attempting to perform this operation without proper handling leads to unexpected behavior and crashes.  The solution illustrates the importance of safe programming practices in Haskell, particularly when dealing with potentially null or missing values.