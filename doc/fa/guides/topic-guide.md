<!--
@license
Copyright (c) <YOUR_COPYRIGHT_HOLDER>

Use of this source code is governed by terms that can be
found in the LICENSE file in the root of this package.
-->

# راهنمای موضوع

TODO: یک یا دو جمله درباره‌ی آنچه این لایه‌ی DNA فراهم می‌کند.

## چه چیزی پیکربندی شده است <a id="what-is-configured"></a>

- TODO: آنچه فایل‌های `dna/` راه‌اندازی می‌کنند را فهرست کنید
- متغیرهای در دسترس در قالب‌ها: `<YOUR_COPYRIGHT_HOLDER>`، `<YOUR_COMPANY>`
  (مقادیر در `dna/_vars.json`)

## افزودن یک فایل <a id="add-a-file"></a>

- آن را در `dna/` قرار دهید. یک `dot-` ابتدایی در مخزنِ مصرف‌کننده به `.`
  تبدیل می‌شود (`dna/dot-foo/bar.json` → `.foo/bar.json`)
- `dart test` را اجرا کنید تا DNA نمونه‌سازی شود و `dna/_generated.json`
  به‌روز شود

## بازنویسی در مخزنِ مصرف‌کننده <a id="override-in-a-consuming-repo"></a>

- فایلی با همان مسیر در لایه‌ای بعدی، این فایل را به‌طور کامل جایگزین می‌کند
- یک `<name>.overrides.json` به جای آن ادغام می‌کند: اشیا به‌صورت عمیق ادغام
  می‌شوند، `"key!"` بدون ادغام جایگزین می‌کند، `"key+"` به یک آرایه اضافه
  می‌کند — برای نحو کامل README مربوط به helix را ببینید
