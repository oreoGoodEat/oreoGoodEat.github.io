---
layout: page
categories: ["代码"]
---

```html
<div class="div_form_2">
    <form action="">
        <!--style="border-collapse: collapse;"这是选择将边框合在一起，默认边框分开-->
        <table style="border-collapse: collapse;">
            <tr>
                <td>用户名</td>
                <td><input type="text"></td>
            </tr>
            <tr>
                <td>性别</td>
                <td>
                    <!-- type="radio" 单选类型-->
                    <input type="radio" value="man" name="sex">男
                    <input type="radio" value="woman" name="sex">女
                </td>
            </tr>
            <tr>
                <td>出生年月</td>
                <td><input type="datetime" value="20200202"></td>
            </tr>
            <tr>
                <td>身份证号</td>
                <td><input type="text"></td>
            </tr>
            <tr>
                <td>邮箱</td>
                <td><input type="email"></td>
            </tr>
            <tr>
                <td>学历</td>
                <td>
                    <!--下拉框选项-->
                    <select name="" id="">
                        <option value="xl">--请选择--</option>
                        <option value="xl">初中</option>
                        <option value="xl">大学</option>
                    </select>
                </td>
            </tr>
            <tr>
                <td>国家区号</td>
                <td>
                    <!--maxlength 这是选择最大输入的字数 value是输入框的默认显示-->
                    <input type="text" maxlength="2" style="width: 15px;" value="86">
                    -地区区号
                    <input type="text" maxlength="" style="width: 40px;" value="">
                    -电话号码
                    <input type="tel" maxlength="11" style="width: 80px;" value="">
                    -分机号码
                    <input type="tel" maxlength="11" style="width: 80px;" value="">
                </td>
            </tr>
            <tr>
                <td>兴趣爱好</td>
                <td>
                    <!--type="checkbox" 多选-->
                    <input type="checkbox">游泳
                    <input type="checkbox">健身
                    <input type="checkbox">学习
                </td>
            </tr>
            <tr>
                <td>手机号码</td>
                <td>
                    <input type="tel" maxlength="11">
                </td>
            </tr>
            <tr>
                <td>多选select控件</td>
                <td>
                    <!--multiple是一个布尔属性，规定用户允许输入到input中的多个值 -->
                    <!---->
                    <select name="" id="" multiple style="width: 180px;">
                        <option value="xl">多选1</option>
                        <option value="xl">多选2</option>
                        <option value="xl">多选3</option>
                        <option value="xl">多选4</option>
                        <option value="xl">多选5</option>
                        <option value="xl">多选6</option>
                    </select>
                </td>
                <td>按住CTRL多选</td>
            </tr>
            <tr>
                <td>描述</td>
                <td>
                    <textarea name="" id="" cols="30" rows="10"></textarea>
                </td>
            </tr>
        </table>
    </form>
</div>

```

#### 总结

table   标签中`style="border-collapse: collapse;"`这是选择将边框合在一起，默认边框分开

select  创建下拉列表
    
    - autofocus 规定下拉时自动获得焦点
    - disabled  规定该属性为true时禁用下拉列表
    - form      值：form_id  定义select所属字段一个或多个表单，即添加了表单的id，即使不在表单内也属于表单
    - multiple  规定可以选择多个选项
    - name      值：text 规定下拉列表的名称
    - required  规定在提交表单之前必须选择一个选项
    - size      值：number 规定可见项目


option  定义下拉列表的一个选项 标签中的内容作为<select>或<datalist>一个元素使用
    - <option> 标签可以在不带有任何属性的情况下使用 通常需要使用 value 属性，此属性会指示出被送往服务器的内容
    - 与 select 元素配合使用此标签，否则这个标签是没有意义的
    - 如果列表选项很多，可以使用 <optgroup> 标签对相关选项进行组合