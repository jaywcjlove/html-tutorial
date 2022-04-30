HTML \<input> type Attribute
===

## 示例

具有两个输入字段的 HTML 表单； 一个文本字段和一个提交按钮：

```html idoc:preview:iframe
<form action="/action_page.php">
  <label for="username">Username: </label>
  <input type="text" id="username" name="username"><br>
  <input type="submit" value="Submit">
</form>
```

## 定义和用法

`type` 属性指定要显示的 `<input>` 元素的类型。

如果未指定 `type` 属性，则默认类型为“文本”。

## 浏览器支持

| Element | ![chrome][1] | ![edge][2] | ![firefox][3] | ![safari][4] | ![opera][5] |
| ------- | --- | --- | --- | --- | --- |
| type      | Yes | Yes | Yes | Yes | Yes |

## 语法

```html
<input type="value">
```

## 属性值 Attribute Values

| 值 | 描述 |
| ---- | ---- |
| [button](./input_type_button.md)                 | 定义一个可点击按钮（主要与 JavaScript 一起使用以激活脚本） |
| [checkbox](./input_type_checkbox.md)             | 定义一个复选框 |
| [color](./input_type_color.md)                   | 定义颜色选择器 |
| [date](./input_type_date.md)                     | 定义日期控件（年、月、日（无时间）） |
| [datetime-local](./input_type_datetime-local.md) | 定义日期和时间控制（年、月、日、时间（无时区） |
| [email](./input_type_email.md)                   | 定义电子邮件地址的字段 |
| [file](./input_type_file.md)                     | 定义文件选择字段和“浏览”按钮（用于文件上传） |
| [hidden](./input_type_hidden.md)                 | 定义一个隐藏的输入字段 |
| [image](./input_type_image.md)                   | 将图像定义为提交按钮 |
| [month](./input_type_month.md)                   | 定义月份和年份控制（无时区） |
| [number](./input_type_number.md)                 | 定义用于输入数字的字段 |
| [password](./input_type_password.md)             | 定义密码字段 |
| [radio](./input_type_radio.md)                   | 定义一个单选按钮 |
| [range](./input_type_range.md)                   | 定义范围控件（如滑块控件） |
| [reset](./input_type_reset.md)                   | 定义一个重置按钮 |
| [search](./input_type_search.md)                 | 定义用于输入搜索字符串的文本字段 |
| [submit](./input_type_submit.md)                 | 定义提交按钮 |
| [tel](./input_type_tel.md)                       | 定义用于输入电话号码的字段 |
| [text](./input_type_text.md)                     | 默认。 定义单行文本字段 |
| [time](./input_type_time.md)                     | 定义输入时间的控件（无时区） |
| [url](./input_type_url.md)                       | 定义用于输入 URL 的字段 |
| [week](./input_type_week.md)                     | 定义周和年控制（无时区） |

## 更多示例

### Input 类型: button

单击时激活 JavaScript 的按钮：

```html idoc:preview:iframe
<script>
function msg() {
  alert("Hello world!");
}
</script>
<input type="button" value="Click me" onclick="msg()">
```

### Input 类型: checkbox

复选框让用户从有限数量的选项中选择一个或多个选项：

```html idoc:preview:iframe
<input type="checkbox" id="vehicle1" name="vehicle1" value="Bike">
<label for="vehicle1"> I have a bike</label><br>
<input type="checkbox" id="vehicle2" name="vehicle2" value="Car">
<label for="vehicle2"> I have a car</label><br>
<input type="checkbox" id="vehicle3" name="vehicle3" value="Boat">
<label for="vehicle3"> I have a boat</label><br>
```

### Input 类型: color

从颜色选择器中选择一种颜色：

```html idoc:preview:iframe
<label for="favcolor">Select your favorite color:</label>
<input type="color" id="favcolor" name="favcolor">
```

### Input 类型: date

定义一个日期控件：

```html idoc:preview:iframe
<label for="birthday">Birthday:</label>
<input type="date" id="birthday" name="birthday">
```

### Input 类型: datetime-local

定义日期和时间控件（无时区）：

```html idoc:preview:iframe
<label for="birthdaytime">Birthday (date and time):</label>
<input type="datetime-local" id="birthdaytime" name="birthdaytime">
```

### Input 类型: email

为电子邮件地址定义一个字段（提交时将自动验证）：

```html idoc:preview:iframe
<label for="email">Enter your email:</label>
<input type="email" id="email" name="email">
```

### Input 类型: file

定义一个文件选择字段和一个“浏览...”按钮（用于文件上传）：

```html idoc:preview:iframe
<label for="myfile">Select a file:</label>
<input type="file" id="myfile" name="myfile">
```

### Input 类型: hidden

定义一个隐藏字段（对用户不可见）。

隐藏字段通常存储提交表单时需要更新的数据库记录：

```html idoc:preview:iframe
<input type="hidden" id="custId" name="custId" value="3487">
```

### Input 类型: image

将图像定义为提交按钮：

```html idoc:preview:iframe
<input type="image" src="../assets/chrome.svg" alt="Submit">
```

### Input 类型: month

定义月份和年份控制（无时区）：

```html idoc:preview:iframe
<label for="bdaymonth">Birthday (month and year):</label>
<input type="month" id="bdaymonth" name="bdaymonth">
```

### Input 类型: number

定义一个用于输入数字的字段（您还可以设置接受哪些数字的限制）：

```html idoc:preview:iframe
<label for="quantity">Quantity (between 1 and 5):</label>
<input type="number" id="quantity" name="quantity" min="1" max="5">
```

使用以下属性来指定限制：

* [max](./input_max.md) - 指定允许的最大值
* [min](./input_min.md) - 指定允许的最小值
* [step](./input_step.md) - 指定合法数字区间
* [value](./input_value.md) - 指定默认值

### Input 类型: password

定义一个密码字段（字符被屏蔽）：

```html idoc:preview:iframe
<label for="pwd">Password:</label>
<input type="password" id="pwd" name="pwd">
```

### Input 类型: radio

单选按钮让用户只选择有限数量的选项之一：

```html idoc:preview:iframe
<input type="radio" id="html" name="fav_language" value="HTML">
<label for="html">HTML</label><br>
<input type="radio" id="css" name="fav_language" value="CSS">
<label for="css">CSS</label><br>
<input type="radio" id="javascript" name="fav_language" value="JavaScript">
<label for="javascript">JavaScript</label>
```

### Input 类型: range

定义一个用于输入精确值不重要的数字的控件（如滑块控件）。 默认范围是 0 到 100。但是，您可以使用 min、max 和 step 属性设置接受哪些数字的限制：

```html idoc:preview:iframe
<label for="vol">Volume (between 0 and 50):</label>
<input type="range" id="vol" name="vol" min="0" max="50">
```

使用以下属性来指定限制：

* [max](./input_max.md) - 指定允许的最大值
* [min](./input_min.md) - 指定允许的最小值
* [step](./input_step.md) - 指定合法数字区间
* [value](./input_value.md) - 指定默认值

### Input 类型: reset

定义一个重置按钮（将所有表单值重置为默认值）：

```html idoc:preview:iframe
<input type="reset">
```

**提示：** 小心使用重置按钮！ 对于意外激活重置按钮的用户来说，这可能会很烦人。

### Input 类型: search

定义搜索字段（如站点搜索或 Google 搜索）：

```html idoc:preview:iframe
<label for="gsearch">Search Google:</label>
<input type="search" id="gsearch" name="gsearch">
```

### Input 类型: submit

定义提交按钮：

```html idoc:preview:iframe
<input type="submit">
```

### Input 类型: tel

定义一个用于输入电话号码的字段：

```html idoc:preview:iframe
<label for="phone">Enter your phone number:</label>
<input type="tel" id="phone" name="phone" pattern="[0-9]{3}-[0-9]{2}-[0-9]{3}">
```

### Input 类型: text

定义用户可以在其中输入文本的两个单行文本字段：

```html idoc:preview:iframe
<label for="fname">First name:</label>
<input type="text" id="fname" name="fname"><br>
<label for="lname">Last name:</label>
<input type="text" id="lname" name="lname"><br>
```

### Input 类型: time

定义一个输入时间的控件（无时区）：

```html idoc:preview:iframe
<label for="appt">Select a time:</label>
<input type="time" id="appt" name="appt">
```

### Input 类型: url

定义一个用于输入 URL 的字段：

```html idoc:preview:iframe
<label for="homepage">Add your homepage:</label>
<input type="url" id="homepage" name="homepage">
```

**提示：** iPhone 上的 Safari 可识别 url 输入类型，并更改屏幕键盘以匹配它（添加 .com 选项）。

### Input 类型: week

定义周和年控制（无时区）：

```html idoc:preview:iframe
<label for="week">Select a week:</label>
<input type="week" id="week" name="week">
```


[1]: ../assets/chrome.svg
[2]: ../assets/edge.svg
[3]: ../assets/firefox.svg
[4]: ../assets/safari.svg
[5]: ../assets/opera.svg