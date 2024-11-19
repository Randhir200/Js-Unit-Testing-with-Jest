## Steps to write unit test case
- write a test function that takes three parameter
    - name
    - function
    - Timeout it is optional (default value is 5sec)
 

Example : 
``` js
test('Returns sold out tagline when no ticket left', () => {
  const event = new Event(1, "Summer BBQ", 40, 100, 0);
  const tagline = getTagline(event, 10, true);
  expect(tagline).toBe("Event Sold out!"); 
})
```
- The argument  for the  'expect' function is the value that you want to validate
- Matchers are used to perform validation (tobe())
