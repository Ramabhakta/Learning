# Easy #
## Problem1 ##
```cs
bool ContainsDuplicate(int[] nums)
{
    HashSet<int> set = new HashSet<int>();
    for (int i = 0; i < nums.Length; i++)
    {
        if (set.Contains(nums[i]))
            return true;

        set.Add(nums[i]);
    }
    return false;
}

Console.WriteLine(ContainsDuplicate(new int[] { 1, 2, 3 }));

```

