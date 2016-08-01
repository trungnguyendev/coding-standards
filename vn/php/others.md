Một số quy tắc khác
=====================

Dưới đây là một số các quy tắc khác, không được quy định cụ thể trong các bộ PSR.

- Sử dụng phiên bản PHP mới nhất nếu có thể.
- Với phiên bản PHP >= 5.4, hãy sử dụng `[]` để khai báo array, thay vì dùng `array()`
```php
// Good
$a = [];
$b = [
    $key => $value,
    $key2 => $value2,
];

// Bad
$a = array();
$b = array(
    $key => $value,
    $key2 => $value2,
);
```

- Tên biến được viết dưới dạng `camelCase`. Đối với tên property bên trong Model thì
có thể viết dưới dạng `snake_case` cho phù hợp với tên của các cột trong các bảng của Database.
- Sử dụng dấu `'` đối với một string bình thường. Chỉ dùng `"` khi bên trong có khai triển biến PHP.
```php
$normalString = 'A String';
$specialString = "This is {$normalString}";
```
- Cần có 1 space trước và sau các toán tử như `+`, `-`, `*`, `/`, `.`, `>`, `<`, `==` ...
