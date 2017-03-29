# dom基本操作

### 1.元素获取方法
#### a.获取单个元素
        document.getElementById("idName");
        document.querySelector("与css选择器格式一致");
#### b.获取多个元素
        document.getElementsByTagName("标签名");
        document.getElementsByName("表单元素的name");
        document.getElementsByClassName("");动态的，实时的
        document.querySelectorAll("");静态的，非实时的

### 2.创建元素、文本
        document.createElement("div");创建元素
        document.createTextNode("hello world");创建文本节点

### 3.移除元素
        ele.remove();移除包括element本身的全部,()内为空
        parentNode.removeChild("childNode");移除其中的childnode

### 4.插入到文档
        parentNode.appendChild(需要插入的node/newNode);插入到parentNode内后面
        parentNode.insertBefore(newNode,positionNode);插入到positionNode节点前面

### 5.替换子元素
        parentNode.replaceChild(newNode,oldNode);

### 6.克隆节点
        ele.cloneNode(boolean);boolean为true时深度克隆，包括节点内部的子节点，()内为false或为空的时候，为浅层克隆

### 7.属性操作
        ele.setAttribute(name,value);设置属性
        ele.getAttribute(name);获取属性
        ele.removeAttribute(name);移除属性