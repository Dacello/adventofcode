## Part 1

```
Enum.reduce(l, {nil, 0}, fn item, {prev_item, count} ->
  cond do
    is_nil(prev_item) ->
      {item, count}
    prev_item < item ->
      {item, count + 1}
    true ->
      {item, count}
  end
end)
```

## Part 2
