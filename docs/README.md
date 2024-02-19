# Eco Documentation
> [!IMPORTANT]  
> I forgot to say about the file extension of files in eco-lang is ".eco". Thanks for your time.
Welcome to the documentation for Eco, a language designed for human-friendly data serialization.

## Defining Data Structures

Keywords for defining data structures:

- **data**: Defines a new data structure
- **object**: Similar to data, but object-oriented
- **table**: Tabular/relational structure like a database table

### Examples

```eco
data user
  name ""
  email ""

object car
  brand ""
  model ""
  year ""

table books
  id ""
  title ""
  author ""
```

## Supported Data Types

Eco supports primitive types like strings, numbers, and booleans without the need for explicit declaration.

For dates, a specific naming convention can be used, such as "fecha", and for arrays, elements are simply listed:

```eco
data invoice 
  date "fecha"
  items ""
```

## References Between Structures

Structures can reference others by their name:

```eco
object user
  name ""

data order
  user_id "user"
``` 

## Nesting Structures

Structures can be nested using indentation, and dashes are used to indicate elements of complex arrays:

```eco
data user 
  name ""
  address ""
   -
      city ""
   -
  description ""
```

## Best Practices

- Use descriptive names
- Keep definitions small and modular
- Add comments for complex parts

## Contributing

Contributions to Eco are welcome! If you have any ideas for improvements or new features, feel free to submit a pull request.

## License

Eco is licensed under the [MIT License](../LICENSE).
