# BEM
- Block Element Modifier
- Block: Khối
- Element: Thành phần trong khối
- Modifier: Bổ sung ý nghĩa cho `Block` hoặc `Element`

# Lý do sử dụng
- Mỗi người một kiểu
- Members đặt class trùng nhau

# Cú pháp
- .block
- .block__element

- .block--modifier
- .block__element--modifier

# Ví dụ
- Thường:
```html
<div class="card">
  <h3 class="heading">Saved</h3>
  <p class="desc">lorem ipsum</p>
  <div class="btn">Close</div>
</div>
```
- BEM:
```html
<div class="card">
  <h3 class="card__heading">Saved</h3>
  <p class="card__desc">lorem ipsum</p>
  <div class="card__btn">Close</div>
</div>
```
- BEM variants:
```html
<div class="card card--success">
  <h3 class="card__heading">Saved</h3>
  <p class="card__desc">lorem ipsum</p>
  <div class="card__btn card__btn--size-l">Close</div>
</div>
```
```html
<div class="card card--error">
  <h3 class="card__heading">Not Saved</h3>
  <p class="card__desc">lorem ipsum</p>
  <div class="card__btn card__btn--size-m">Close</div>
</div>
```
```css
.card {}
.card--success .card__btn {}
.card--error .card__btn {}
.card__heading {}
.card__desc {}
.card__btn {}
.card__btn--size-l {}
.card__btn--size-m {}
```

# Ứng dụng
- Xây dựng layout website
- Xây dựng thành phần website

# Ưu điểm
- Tính rõ ràng
- Tái sử dụng: ko sợ bị trùng tên class
- Team work: dễ dàng đọc hiểu code của nhau

# Khi nào dùng BEM là PHÙ HỢP
- Dự án nhiều người
- Dự án lớn, nhiều page

