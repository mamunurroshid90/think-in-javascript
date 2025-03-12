# JS scopes

```
** js scope **
সাধারণত scope টা ১টা দুনিয়া, তার মধ্যে ১টা হলো global / parents, অন্যটা হলো তার child এর দুনিয়া, যখন আমরা কোন কিছু normally var দিয়ে declare করি, তখন সেটা global দুনিয়ায় থাকে, এটা window এর মধ্যে থাকে।

আবার যখন আমরা function এর মধ্যে কোনো variable declare করি, তখন সেটা শুধু ঐ নির্দিষ্ট function এর দুনিয়ায় থাকে।

এখানে global / parents এ যদি var declare করা হয়, তাহলে সেটা সবার জন্য উম্মুক্ত হয় যায়, তাকে যেকোনো জায়গা থেকে ব্যবহার করা যায়, কিন্তু child এ কোন কিছু declare করা হইলে সেটা কে তার বাইরে থেকে আর ব্যবহার করা যায়না।

example

```

![scope example](/images/scope-1.png)

```
যদি আমরা গ্লোবাল এর var এর মান child এর ভিতরে পরিবর্তন করতে চাই তাহলে কিন্ত সেটাও সম্ভব।
example
```

![scope example 2](/images/scope-2.png)

```
কিন্তু যদি আমরা child এর মধ্যে আবার var declare করি তাহলে কিন্তু parents er var এর মান পরিবর্তন হবে না।

example
```

![scope example 3](/images/scope-3.png)

```
আমরা যদি কখনো গ্লোবাল এ কোন var declare না করি, আবার child এর মধ্যে var না লিখে শুধু x = 10 লিখে দেই, তখন সেটা মনে মনে ধরে নেয় যে globally / parents এ এটা declare করা আছে,
example
```

![scope example 4](/images/scope-4.png)

```
উপরোক্ত সমস্যার সমাধানের জন্যে আমরা একদম কোড এর শুরুতে "use strict" লিখে নিতে পারি, তাহলে আমাদের কে এই প্রব্লেম থেকে আটকায় দিবে,

example
```

![scope example 5](/images/scope-5.png)
