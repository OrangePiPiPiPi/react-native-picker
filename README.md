# react-native-pickers
纯JS实现的React-Native 日期选择控件、地址选择控件等。

时间不多，肯定有bug，欢迎留言第一时间维护。

由于很多属性并没有封装好开放，所以暂时直接以源码形式分享，未插件化（2018年3月5日）

欢迎直接下载代码删改使用，欢迎沟通了解实现原理，有帮得上的，记得给星哦~


<code>AlertDialog:</code>
<table>
    <thead>
        <tr>
            <th>属性</th>
            <th>默认值</th>
            <th>描述</th>
            <th>截图</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>messageText</td>
            <td>'Alert Message'</td>
            <td>消息文本</td>
            <td rowspan="10">
                <img src="https://github.com/iberHK/react-native-pickers/blob/master/screenshot/AlertDialog.png"/>
            </td>
        </tr>
        <tr>
            <td>messageTextColor</td>
            <td>'#444444'</td>
            <td>消息文本字体颜色</td>
        </tr>
        <tr>
            <td>messageTextSize</td>
            <td>14</td>
            <td>消息文本字体大小</td>
        </tr>
        <tr>
            <td>negativeText</td>
            <td>'cancel'</td>
            <td>取消文本</td>
        </tr>
        <tr>
            <td>negativeColor</td>
            <td>'#666666'</td>
            <td>取消文本颜色</td>
        </tr>
        <tr>
            <td>negativeSize</td>
            <td>16</td>
            <td>取消文本字体大小</td>
        </tr>
        <tr>
            <td>positiveText</td>
            <td>'ok'</td>
            <td>确定文本</td>
        </tr>
        <tr>
            <td>positiveColor</td>
            <td>'#1097D5'</td>
            <td>确定文本颜色</td>
        </tr>
        <tr>
            <td>positiveSize</td>
            <td>16</td>
            <td>确定文本字体大小</td>
        </tr>
        <tr>
            <td>onPress</td>
            <td>null</td>
            <td>
                <code>positive(确定)返回true</code> or
                <code>negative(取消)返回false</code>
            </td>
        </tr>
    </tbody>
</table>



<code>SimpleItemsDialog:</code>
<table>
    <thead>
        <tr>
            <th>属性</th>
            <th>默认值</th>
            <th>描述</th>
            <th>截图</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>items</td>
            <td>['a', 'b', 'c']</td>
            <td>列表数据，可以string、object(需要指定itemKey)</td>
            <td rowspan="10">
                <img src="https://github.com/iberHK/react-native-pickers/blob/master/screenshot/items.png"/>
            </td>
        </tr>
        <tr>
            <td>itemKey</td>
            <td>'key'</td>
            <td>
                当item为object时，来指定显示的属性<br>
                <code>items:[{id:0, value: 'v1'},{id:0, value: 'v1'}]</code><br>
                <code>itemKey设为'value',则等同于<code>['v1', 'v2']</code><br>
            </td>
        </tr>
        <tr>
            <td>itemStyle</td>
            <td>
                    {<br>
                        fontSize: 14,<br>
                        fontWeight: '400',<br>
                        color: '#333333'<br>
                    }
            </td>
            <td>列表文字样式</td>
        </tr>
        <tr>
            <td>cancel</td>
            <td>true</td>
            <td>是否在列表最后 增加 ‘取消’ 项</td>
        </tr>
        <tr>
            <td>cancelText</td>
            <td>'取消'</td>
            <td>取消项文本</td>
        </tr>
        <tr>
            <td>cancelTextStyle</td>
            <td>
                    {<br>
                        fontSize: 14,<br>
                        fontWeight: '400',<br>
                        color: '#999999'<br>
                    }
            </td>
            <td>取消文本字体样式</td>
        </tr>
        <tr>
            <td>onPress</td>
            <td>null</td>
            <td>
                返回选中index
            </td>
        </tr>
    </tbody>
</table>


<code>SimpleChooseDialog:</code>
<table>
    <thead>
        <tr>
            <th>属性</th>
            <th>默认值</th>
            <th>描述</th>
            <th>截图</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>items</td>
            <td>['a', 'b', 'c']</td>
            <td>列表数据，可以string、object<br>
                (需要指定itemKey)</td>
            <td rowspan="11">
                <img src="https://github.com/iberHK/react-native-pickers/blob/master/screenshot/simplechoosedialog.png"/>
            </td>
        </tr>
        <tr>
            <td>itemKey</td>
            <td>'key'</td>
            <td>
                当item为object时，来指定显示的属性<br>
                <code>items:[{id:0, value: 'v1'},{id:0, value: 'v1'}]</code><br>
                <code>itemKey设为'value',则等同于<br>
                <code>['v1', 'v2']</code><br>
            </td>
        </tr>
        <tr>
            <td>itemStyle</td>
            <td>
                    {<br>
                        fontSize: 14,<br>
                        fontWeight: '400',<br>
                        color: '#333333'<br>
                    }
            </td>
            <td>列表文字样式</td>
        </tr>
        <tr>
            <td>selectColor</td>
            <td>'#1097D5'</td>
            <td>选中颜色</td>
        </tr>
        <tr>
            <td>normalColor</td>
            <td>'#666666'</td>
            <td>未选中颜色</td>
        </tr>
        <tr>
            <td>pointSize</td>
            <td>18</td>
            <td>左侧选中标识大小</td>
        </tr>
        <tr>
            <td>pointBorderRadius</td>
            <td>9</td>
            <td>左侧选中标识边框弧度</td>
        </tr>
        <tr>
            <td>confirmText</td>
            <td>'确定'</td>
            <td>确定选择文本</td>
        </tr>
        <tr>
            <td>confirmBtnColor</td>
            <td>'#1097D5'</td>
            <td>确定选择按钮颜色</td>
        </tr>
        <tr>
            <td>confirmTextColor</td>
            <td>'#ffffff'</td>
            <td>确定选择文本颜色</td>
        </tr>
        <tr>
            <td>onPress</td>
            <td>null</td>
            <td>
                返回选中index
            </td>
        </tr>
    </tbody>
</table>


<code>SimpleChooseDialog:</code>
<table>
    <thead>
        <tr>
            <th>属性</th>
            <th>默认值</th>
            <th>描述</th>
            <th>截图</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>title</td>
            <td>'我要举报'</td>
            <td>标题文本</td>
            <td rowspan="11">
                <img src="https://github.com/iberHK/react-native-pickers/blob/master/screenshot/inputdialog.png"/>
            </td>
        </tr>
        <tr>
            <td>titleSize</td>
            <td>16</td>
            <td>标题文本字体大小</td>
        </tr>
        <tr>
            <td>titleColor</td>
            <td>'#333333'</td>
            <td>标题文本文本颜色</td>
        </tr>
        <tr>
            <td>cancelText</td>
            <td>'返回'</td>
            <td>取消文本</td>
        </tr>
        <tr>
            <td>cancelSize</td>
            <td>14</td>
            <td>取消文本字体大小</td>
        </tr>
        <tr>
            <td>cancelColor</td>
            <td>'#333333'</td>
            <td>取消文本字体颜色</td>
        </tr>
        <tr>
            <td>btnText</td>
            <td>'提交'</td>
            <td>提交文本</td>
        </tr>
        <tr>
            <td>btnTextSize</td>
            <td>12</td>
            <td>提交文本字体大小</td>
        </tr>
        <tr>
            <td>btnTextColor</td>
            <td>'#ffffff'</td>
            <td>提交文本字体颜色</td>
        </tr>
        <tr>
            <td>btnBgColor</td>
            <td>'#1097D5'</td>
            <td>提交按钮颜色</td>
        </tr>
        <tr>
            <td>placeholder</td>
            <td>'请尽量说明问题，我们将尽快处理...'</td>
            <td>输入框提示语</td>
        </tr>
        <tr>
            <td>onSubmit</td>
            <td>null</td>
            <td>
                返回输入的文本内容
            </td>
        </tr>
        <tr>InputDialog.show(text(输入框文字))</tr>
    </tbody>
</table>


![image](https://github.com/iberHK/react-native-pickers/blob/master/screenshot/inputdialog.png)


![image](https://github.com/iberHK/react-native-pickers/blob/master/screenshot/customer.png)
![image](https://github.com/iberHK/react-native-pickers/blob/master/screenshot/area.png)


![image](https://github.com/iberHK/react-native-pickers/blob/master/screenshot/date.png)
![image](https://github.com/iberHK/react-native-pickers/blob/master/screenshot/xxx.png)
