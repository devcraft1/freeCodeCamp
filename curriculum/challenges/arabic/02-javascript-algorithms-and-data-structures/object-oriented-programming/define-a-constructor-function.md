---
id: 587d7dad367417b2b2512b77
title: تعريف دالة البناء (Define a Constructor Function)
challengeType: 1
forumTopicId: 16804
dashedName: define-a-constructor-function
---

# --description--

الـ <dfn>Constructors</dfn> هي functions تقوم بأنشاء objects جديدة. وهي تحدد الخصائص والسلوكيات التي ستنتمي إلى الـ object الجديد. فكر فيها كمخطط لإنشاء objects جديدة.

وفيما يلي مثال على constructor:

```js
function Bird() {
  this.name = "Albert";
  this.color = "blue";
  this.numLegs = 2;
}
```

هذا الـ constructor يعرف object الـ `Bird` ذو خصائص `name`, `color` و `numLegs` تم تعيينهم إلى Albert و blue و 2 على التوالي. ويتبع الـ Constructors بعض الاتفاقيات:

<ul><li>يتم تعريف الـ Constructors مع اسم capitalized لتمييزهم عن الـ functions الأخرى التي ليست <code>constructors</code>.</li><li>يستخدم الـ Constructors كلمة <code>this</code> لتعيين خصائص الـ object الذي سينشئونه. داخل الـ constructor الكلمة <code>this</code> تشير إلى الـ object الجديد الذي ستقوم بإنشائه.</li><li>يقوم الـ Constructors بتحديد الخصائص والسلوكيات بدلاً من إرجاع قيمة مثل ما قد يفعل الـ functions الأخرى.</li></ul>

# --instructions--

قم بإنشاء constructor الـ `Dog`، بخصائص `name` و `color` و `numLegs` التي تم تعيينهم على string و string و رقم، على التوالي.

# --hints--

`Dog` يجب أن يكون لديه خاصية `name` من نوع string.

```js
assert(typeof new Dog().name === 'string');
```

`Dog` يجب أن يكون لديه خاصية `color` من نوع string.

```js
assert(typeof new Dog().color === 'string');
```

`Dog` يجب أن يكون لديه خاصية `numLegs` من نوع number.

```js
assert(typeof new Dog().numLegs === 'number');
```

# --seed--

## --seed-contents--

```js

```

# --solutions--

```js
function Dog (name, color, numLegs) {
  this.name = 'name';
  this.color = 'color';
  this.numLegs = 4;
}
```
