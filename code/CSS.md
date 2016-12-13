## CSS代码分析

- 滚动条
```stylesheet
::-webkit-scrollbar{
    width:5px;
    height:5px;
}
::-webkit-scrollbar-track,::-webkit-scrollbar-corner{
    background:rgba(0,0,0,0);
}
::-webkit-scrollbar-thumb{
    background:rgba(0,0,0,.2);
    border-radius:4px;
}
::-webkit-scrollbar-thumb:hover{
    background:rgba(0,0,0,.3);
}
```
