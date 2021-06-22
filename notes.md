# Notes

## Elixir

When a the anonymous functions with one param, ans return the return of a function, that use this param, we can use just `&` with the function and your number of params:

```elixir
# Anonymous F
element
|> List.update_at(1, fn elem -> String.to_float(elem) end)

# More Anonymous F
element
|> List.update_at(1, &String.to_float/1)
```

## Ecto

Reset executed migration:
```bash
mix ecto.reset
```
