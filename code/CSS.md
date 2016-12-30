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
- 快递四色条纹
```stylesheet
background: linear-gradient(315deg,#95c5f7 0, #95c5f7 12.5%, #fff 0, #fff 25%, #f3a1a1 0, #f3a1a1 37.5%, #fff 0, #fff 50%, #95c5f7 0, #95c5f7 62.5%, #fff 0, #fff 75%,#f3a1a1 0, #f3a1a1 87.5%, #fff 0);
background-size: 1.27279220613rem 1.27279220613rem;
```
