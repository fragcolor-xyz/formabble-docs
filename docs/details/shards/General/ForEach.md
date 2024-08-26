- This shard is able to use the internal variable `$0` and `$1` within its `Apply` parameter.

- If a sequence was provided as input, the variable `$0` will take the value of the current element of the sequence it is iterating over. ($1 does not exist when iterating over a sequence)
  For example:
  ```shards
  [1, 2, 3]
  ForEach( 
    Apply:{
      $0 | Math.Add(1)
    }
  )
  ```
  `$0` will take the value of 1 and then 2 and then 3 accordingly.

- If a table was provided as input, the variable `$0` will be the current key of the table it is iterating over while `$1` will take the value associated with the key.
  For example:
  ```shards
  {
    "a": 1,
    "b": 2,
    "c": 3
  }
  ForEach( 
    Apply:{
      $0 | Log
      $1 | Math.Add(1)
    }
  )
  ```
  `$0` will take the value of "a" and then "b" and then "c" while `$1` will take the value of 1 and then 2 and then 3 accordingly.

- When iterating over a table, the 'Apply' parameter receives a sequence of two elements as input, where the first element is the key and the second is the value. $0 and $1 are set to these values respectively.

- Do note that this instance of `$0` and `$1` are unique to the `ForEach` shard and do not exist outside of the context of its `Apply` parameter. Values set to this instance of `$0` and `$1` will not be reflected on other `$0` and `$1` created in a different call of another `ForEach` shard or any other shard that is also able to use `$0` and `$1`.

- `ForEach` returns the input unchanged unlike Map which returns the modified sequence or table.




