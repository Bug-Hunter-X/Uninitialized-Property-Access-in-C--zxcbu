# Uninitialized Property Access in C#

This repository demonstrates a common error in C#: accessing a property before it's been initialized.  The `bug.cs` file shows the problematic code, where `MyProperty` is used in `MyMethod` without first assigning a value.  This can lead to unpredictable behavior, often a `NullReferenceException` if the property is a reference type or unexpected results if it's a value type with a default value.

The `bugSolution.cs` file provides a corrected version, showing how to initialize `MyProperty` with a default value either in the declaration or before access to guarantee safe and predictable program execution.