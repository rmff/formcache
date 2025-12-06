# jQuery Form Cache

Forked from Form Cache v0.0.3 by Fengyuan Chen
https://github.com/fengyuanchen/formcache

Demo by Fengyuan Chen (v0.0.3) 
https://fengyuanchen.github.io/formcache/

Added option to do not cache some fields
```js
FormCacheOptions = {
  key: 'formcache',
  local: true,
  session: true,
  autoStore: true,
  maxAge: 3600, //1 hour
  controls: [
    // Fields to be cached
    'select',
    'textarea',
    'input'
    // 'input[type="text"]',
    // 'input[type="password"]',
    // 'input[type="datetime"]',
    // 'input[type="checkbox"]',
    // 'input[type="radio"]',
    // 'input[type="datetime-local"]',
    // 'input[type="date"]',
    // 'input[type="month"]',
    // 'input[type="time"]',
    // 'input[type="week"]',
    // 'input[type="number"]',
    // 'input[type="email"]',
    // 'input[type="url"]',
    // 'input[type="search"]',
    // 'input[type="tel"]',
    // 'input[type="color"]'
  ],
  noCache: [
    // Do not cache those fields
    'input[type="hidden"]',
    'input[name="abc"]',
    'input[id="xyz"]'
  ]
}

//Start/Load form cache
$("#FORM").formcache(FormCacheOptions);
```
