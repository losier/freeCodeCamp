---
id: 5cdafbb0291309899753167f
title: إنشاء promise في جافا سكريبت (Create a JavaScript Promise)
challengeType: 1
forumTopicId: 301197
dashedName: create-a-javascript-promise
---

# --description--

الوعد (promise) في لغة JavaScript هو التوعد بالقيام بشيء ما، عادة بشكل غير متزامن. وعندما تنتهي المهمة، إما أن تفي بالوعد أو أن تخفق في ذلك. يكون `Promise` منشئ للوظيفة، لذا تحتاج إلى استخدام كلمة `new` لإنشاء واحد. إنه يأخذ وظيفة (كحجة) مع حجتين - `resolve` و `reject`. وهذه هي الطرق المستخدمة لتحديد نتيجة الوعد. يبدو بناء الجملة كهذا:

```js
const myPromise = new Promise((resolve, reject) => {

});
```

# --instructions--

قم بإنشاء وعد جديد يسمى `makeServerRequest`. قم بتمرير وظيفة بحجج `resolve` و `reject` ألى المنشئ (constructor).

# --hints--

يجب عليك تخصص وعد (promise) إلى متغير المعلن اسمه `makeServerRequest`.

```js
assert(makeServerRequest instanceof Promise);
```

يجب أن يتلقى الوعد الخاص بك الوظيفة مع `resolve` و `reject` كحجج.

```js
assert(
  code.match(
    /Promise\s*\(\s*(function\s*\(\s*resolve\s*,\s*reject\s*\)\s*{|\(\s*resolve\s*,\s*reject\s*\)\s*=>\s*{)[^}]*}/g
  )
);
```

# --seed--

## --seed-contents--

```js

```

# --solutions--

```js
const makeServerRequest = new Promise((resolve, reject) => {

});
```
