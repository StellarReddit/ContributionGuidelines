# Contribution Guidelines
We are excited to have you as a potential open source contributor! You are welcome to submit pull requests for any of our repositories. Please be mindful of these guidelines, as they will raise the likelihood of your contribution being accepted and in the hands of thousands of users world-wide.


## NO ChatGPT or AI contributions!
We noticed a significant increase in the use of AI generated code in professional settings. Because we cannot easily verify the license of the original source code used to train the models, we have made the decision to reject commits with AI generated code.

The main reason for this is that some code may come from projects with incompatible licenses. Another important reason is ethically sourcing code that can be cited.

## Concise commits
Try to keep commits relatively small. There is no specific minimum or maximum number of lines to change. However, it makes it much easier for us to audit changes.

Examples of concise commits:
* Renaming of a variable/function
* Error handling for variable/function
* Adding or removing structs/functions

## Miscellaneous code formatting
* Do not use tabs
* Generally use One-True-Brace style

## Variable naming
* Use `camelCase` for Swift variables and functions
* Use `PascalCase` for exported Go variables and functions
* Use `snake_case` for C++ variables and functions
* Do not encapsulate variables with leading underscores `_`

## Return early
We make use of `guard` to return early, and minimize code indentation.
```swift
guard isRaining,
      isMonday else {
      return
}

/// it is raining on a Monday
```

## Avoid weird and inconsistent spacing and braces/parentheses etc.
```c++
do_something( my_val);
```

```c++
for( int i = 0;i<3;++i){
}
```

# Check back before contributing
This is a living document, meaning it will be updated over time.
