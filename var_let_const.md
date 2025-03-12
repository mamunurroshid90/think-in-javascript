# var, let, const difference

## var & let scope difference

```
var & let এর মধ্যে পার্থক্য কি?
var কে মূলত বলা হয় function/global scope, এটা তার function / global এর দুনিয়ায় যেকোনো জায়গা থেকে তাকে use করা যায়।
আমরা যে ফাইলে কাজ করি ঐটাও এক ধরনের function scope এর মধ্যে পড়ে।

let হলো সে একটা block scope এর মধ্যেই সুধু কাজ করবে, যেমন {} এর ভিতরে declare করলে এর বাহিরে থেকে তাকে আর use করা যাবে না। সে শুধু block scope / {} দুনিয়ায় কাজ করবে।

নিচে তার পার্থক্য দেখানো হলো -
```

![var & let er moddhe scope kivabe kaj kore](/images/var-1.png)
![var & let er moddhe scope kivabe kaj kore](/images/var-2.png)

## var & let declaration difference

```
var দিয়ে আমরা কোন variable declare করলে সেই একই variable কে আমরা আবার redeclare & reassign ও করতে পারবো।

let দিয়ে কোন variable declare করলে সেই variable কে আমরা redeclare করতে পারবো না, কিন্তু reassign করতে পারবো, সেটা কিন্তু আবার block scope / { } এর মধ্যেই করতে হবে।

নিম্মে তার উদাহরণ দেওয়া হলো -
```

![var & let declare and reassign difference](/images/var-3.png)

## const difference

```
const হলো সবার থেকে আলাদা, এটা দিয়ে কোন variable declare করা হলে তাকে redeclare / reassign কিছুই করা যায়না, এটা সম্পুর্ন স্বতন্ত্র
নিম্মে তার উদাহরণ দেওয়া হলো -
```

![const er difference](/images/var-4.png)

## const change only object value

```
const দিয়ে যদি কোন object declare করা হয়, তাহলে কিন্তু আমরা ঐ একই object এর value পরিবর্তন করে দিতে পারবো,
যেমন -
```

![const object value change](/images/var-5.png)

## var function access parent and child

```
var দিয়ে যখন কোন variable কোন function এর ভিতরে declare করা হয়, তখন কিন্তু ঐ variable কে তার বাহিরে থেকে use করা যায়না, ঐটা তখন শুধু ঐ function এর ভিতরেই কাজ করবে,
যেমন -
```

![function er moddhye var declaration](/images/var-6.png)

```
var দিয়ে কোন variable declare করলে ঐ variable এর child সেটা কে use করতে পারে, কিন্তু child এর ভিতরে থাকলে তাকে parent থেকে আর use করা যায়না,
যেমন -
```

![var variable access parents and child](/images/var-7.png);
