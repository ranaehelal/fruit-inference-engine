# Expert System with Backward and Forward Chaining

A simple rule-based expert system implementation in Python that demonstrates both backward and forward chaining inference algorithms.

## Features

- **Backward Chaining**: Goal-driven reasoning that works backward from a goal to determine if it can be proved using available facts and rules.
- **Forward Chaining**: Data-driven reasoning that applies rules to known facts to infer new facts until no more rules can be applied.
- **Rule Parsing**: Supports rules with AND and OR conditions.
- **Fact Handling**: Supports boolean facts, numeric comparisons, and "is" relationships.

## Usage

1. Create a `facts.txt` file with your initial facts:
```
#goal prove citrus_fruit
color is yellow
taste is sour
```

2. Create a `rules.txt` file with your rules:
```
IF color is yellow AND taste is sour THEN citrus_fruit
IF has_segments AND round THEN citrus_fruit
```

3. Run the expert system:
```
python expert_system.py
```

The system will attempt to prove the goal using backward chaining and then demonstrate forward chaining to infer all possible facts from the initial knowledge base.
