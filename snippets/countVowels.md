### countVowels

Retuns number of vowels in provided string.

Use a regular expression to count the number of vowels (A, E, I, O, U) in a string.

```php
function countVowels($string)
{
    preg_match_all('/[aeiou]/i', $string, $matches);
    $matches = $matches[0];

    return count($matches);
}
```

<details>
<summary>Examples</summary>

```php
countVowels('sampleInput'); // 4
```

</details>
