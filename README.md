---

# Bubble Sort Method

This project implements a method `#bubble_sort` that sorts an array using the bubble sort algorithm.

## Description

The `#bubble_sort` method takes an array as an argument and returns a sorted array. It repeatedly steps through the list, compares adjacent elements, and swaps them if they are in the wrong order. This process continues until the array is sorted.

## Usage

### Method Definition

```ruby
def bubble_sort(arr)
  n = arr.length
  loop do
    swapped = false
    (n-1).times do |i|
      if arr[i] > arr[i+1]
        arr[i], arr[i+1] = arr[i+1], arr[i]
        swapped = true
      end
    end
    break unless swapped
  end
  arr
end
```

### Example

```ruby
puts bubble_sort([4, 3, 78, 2, 0, 2]).inspect
# => [0, 2, 2, 3, 4, 78]
```

## Contributing

Contributions are welcome! Please fork the repository, create a new branch, and submit a pull request.

## License

This project is licensed under the MIT License.

---
