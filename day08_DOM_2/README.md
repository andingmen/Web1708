

# ��� #

1. �ڵ�����
2. �ڵ����
3. �¼�(����)


# �������� #


## �ڵ����� ##

```
box.attributes;      // �ڵ�����������
box.getAttribute('data-index')  // ��ȡԪ�ؽڵ����Ե�ֵ

box.setAttribute('data-index',2); // ���ýڵ������
box.removeAttribute('title') // �Ƴ��ڵ�����
```


### ��ҳ���� ###

css ��ʽ���� css �ļ���
```
<link id="link" href="css/css1.css" rel="stylesheet" type="text/css" />


<dl id="message">
	<form>
		<dt>
			<strong>���Ի������ύ��</strong>
			<input type="button" value="Ƥ��1" data-css="css1" />
			<input type="button" value="Ƥ��2" data-css="css2" />
		</dt>
		<dd>����������<input class="text" type="text" /></dd>
		<dd>�������룺<input class="text" type="password" /></dd>
		<dd>�������ԣ�<textarea></textarea></dd>
		<dd class="center"><input class="btn" type="submit" value="�ύ" /></dd>
	</form>
</dl>

```


style CSS������ʽ����ֵ
��ȡ��������ʽ�����ԣ�����Ҫʹ��currentStyle��IE���У�
```
//var style = window.getComputedStyle("Ԫ��", "α��");
var dom = document.getElementById("test");
style = window.getComputedStyle(dom , ":after");
```
//����������Եڶ���α�಻֧��
className CSSԪ�ص��� (������ʹ��class)


### ������ ###


```
<style>
	#progress{
		position: relative;
		margin: auto;
		top: 200px;
		display: block;
		width: 200px;
		height: 20px;
		border-style: dotted;
		border-width: thin;
		border-color: darkgreen;
	}
	#filldiv{
		position:absolute;
		top: 0px;
		left: 0px;
		width: 0px;
		height: 20px;
		background: blue;
	}
	#percent{
		position: absolute;
		top: 0px;
		left: 200px;
		
	}
</style>


<div id="progress">
	<div id="filldiv"></div>
	<span id="percent">0</span>
</div>

```


## �ڵ�������� ##

DOM ���������Բ��ҽڵ㣬Ҳ���Դ����ڵ㡢���ƽڵ㡢����ڵ㡢ɾ���ڵ���滻�ڵ�

```
createElement() //����һ��Ԫ�ؽڵ�
createTextNode()  //����һ���ı��ڵ�
box.appendChild(node)  //��node�ڵ���뵽box���ڲ�����λ��
box.insertBefore(newNode, existNode)  //��newNode�ڵ���뵽exsitNode��ǰ��
box.removeChild(node) // ��box���Ƴ��ڵ�
box.replaceChild(p,h1); // h1�滻��p

box.cloneNode(true) // ��¡�ڵ�

```

### ��ӱ�� ###


```
	<style>
		table{margin-top:20px;width:100%;border:1px solid #ddd;border-collapse: collapse;}
		td{padding:5px 15px;border:1px solid #ddd;}

		/*css3���б�ɫ*/
		/*table tr:nth-child(odd){
			background-color:#efefef;
		}*/
		.odd{background-color:#fc0;}
	</style>


�У�<input type="text" id="row"> �У�<input type="text" id="col"><button>���ɱ��</button>
```


### ����и��� ###

node.cloneNode(true);

����Ϊ true���������Ҫ��¡�ڵ㼰�����ԣ��Լ����
����Ϊ false�������ֻ��Ҫ��¡�ڵ㼰����

### �����ж�ɫ ###

```
		// i ����Ӧ �к� �� �к�
		// 2*2
		// i:   �к�  �к�
		// 0     0    0
		// 1     0    1
		// 2     1    0
		// 3     1    1

    // oDiv = document.createElement("div");
	// oDiv.className = "block";
	// // ��һ������Ŀ�� + ��϶
	// oDiv.style.left = (200 + 20) + "px";

	// gameBox.appendChild(oDiv);

```


��θı䷽�����ɫ��
	
```
oDiv.style.background = "#ff0000";
```

ff(16) = 1111 1111(2) = 2^8 - 1 = 256

---------
��β����������ɫ��

---------
��������λ�õ���ɫ

��ѭ�����ж�����λ�ã����ó�һ���µ������ɫ����


---------
�� div Ԫ������ӵ���¼�������


---------
����ˣ� ���´�������(���µ��ú���)

�������װ�ɺ���

---------
������չ

���3�β�����
����˵ļ�����ʾ





















## �¼����� ##


### �����˵� ###

�¼����� event

event.target // ��ǰʱ�䴥���Ľڵ�


# ��ҵ #
1. ����Ч��
    ![](hw1.jpg)

2. �����˵�

3. �����ж�ɫ ��С��Ϸ��

����չ�� ���ʱ�༭

