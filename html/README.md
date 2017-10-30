# HTML

* [Validation](#Validation)
* [Attributes and Tags](#attributes-and-tags)
* [Indentation](#indentation)
* [Whitespace](#whitespace)
* [Quotes](#quotes)
* [Self-closing elements](#self-closing-elements)

## Validation
All HTML pages should be verified against the [W3C validator](https://validator.w3.org/) to ensure that the markup is well formed. This in and of itself is not directly indicative of good code, but it helps to weed out problems that are able to be tested via automation. It is no substitute for manual code review.


## Attributes and Tags
* All tags and attributes must be written in lowercase.
* Additionally, attribute values should be lowercase when the purpose of the text therein is only to be interpreted by machines. For instances in which the data needs to be human readable, proper title capitalization should be followed.

For machines:
```html
<meta http-equiv="content-type" content="text/html; charset=utf-8" />
```

For humans:
```html
<a href="http://example.com/" title="Description Here">Example.com</a>
```

## Indentation
4 spaces tab

## Whitespace
* Lines should have no trailing whitespace at the end.
* Files should be formatted with `\n` as the line ending (Unix line endings), not `\r\n` (Windows line endings).
* All text files should end in a single newline `\n`. This avoids the verbose "\ No newline at end of file" patch warning and makes patches easier to read since it's clearer what is being changed when lines are added to the end of a file.

## Quotes
* All attributes must have a value, and must use double- or single-quotes.

Correct:
```html
<input type="text" name="email" disabled="disabled" />
<input type='text' name='email' disabled='disabled' />
```
Incorrect:
```html
<input type=text name=email disabled>
```

## Self-closing elements
* All tags must be properly closed. 
* For tags that are self-closing, the forward slash should have exactly one space preceding it:

Correct:
```html
<br />
```
Incorrect:
```html
<br/>
```