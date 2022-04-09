# String operation collection

``StrOpColl`` is a PHP class which contains functions for common string operations.

Instanceing the class is not necessary because the functions are static.

## Functions

### isStringContainNumber

```php
isStringContainNumber(string $stringToCheck): bool
```

Finds whether the given string is contain number.

### isStringContainLowercase

```php
isStringContainLowercase(string $stringToCheck): bool
```

Finds whether the given string is contain lowercase.

### isStringContainUppercase

```php
isStringContainUppercase(string $stringToCheck): bool
```

Finds whether the given string is contain uppercase.

### checkStringLength

```php
checkStringLength(string $stringToCheck, int $minLength, int $maxLength): bool
```

Decides whether the given string is lower than given minimum and greater than the given maximum.

### isStringEmail

```php
isStringEmail($stringToCheck): bool
```

Finds whether the given string has email format.

### isStringsAreEqual

```php
isStringsAreEqual(string ...$strings): bool
```

Finds whether the given strings are equal.

### generateRandomString

```php
generateRandomString(int $stringLength, bool $caseSensitive = false, bool $specialChars = false): string
```

Generate a random string with the given length. Containing lower and uppercase letters or special characters are optional.

### encryptWithSalt

```php
encryptWithSalt($stringToEncrypt, $salt):string
```

It concatenate the given string and the given salt then encrypt the result with using ``sha512`` and ``md5`` algorithm.
