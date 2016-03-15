###HTML/CSS����

**1��ʲô�Ǻ���ģ�ͣ�**

����ҳ�У�һ��Ԫ��ռ�пռ�Ĵ�С�ɼ������ֹ��ɣ����а���Ԫ�ص����ݣ�content����Ԫ�ص��ڱ߾ࣨpadding����Ԫ�صı߿�border����Ԫ�ص���߾ࣨmargin���ĸ����֡����ĸ�����ռ�еĿռ��У��еĲ��ֿ�����ʾ��Ӧ�����ݣ����еĲ���ֻ�����ָ����ڵ����������4������һ�𹹳���css��Ԫ�صĺ�ģ�͡�

**2������Ԫ������Щ���鼶Ԫ������Щ����(void)Ԫ������Щ��**

����Ԫ�أ�a��b��span��img��input��strong��select��label��em��button��textarea

�鼶Ԫ�أ�div��ul��li��dl��dt��dd��p��h1-h6��blockquote

��Ԫ�أ���ϵû�����ݵ�HTMLԪ�أ����磺br��meta��hr��link��input��img

**3��CSSʵ�ִ�ֱˮƽ����**

һ����������⣬ʵ�ַ����кܶ��֣�����������һ��ʵ�֣�

HTML�ṹ��

```html
<div class="wrapper">
     <div class="content"></div>
</div>
```

CSS��

```css
.wrapper{position:relative;}
.content{
	background-color:#6699FF;
	width:200px;
	height:200px;
	position: absolute;        //��Ԫ����Ҫ��Զ�λ
	top: 50%;
	left: 50%;
	margin-top:-100px ;   //����֮һ��height��width
	margin-left: -100px;
}
```

**4������һ��src��href������**

href��ָ��������Դ����λ�ã������͵�ǰԪ�أ�ê�㣩��ǰ�ĵ������ӣ�֮������ӣ����ڳ����ӡ�

src��ָ���ⲿ��Դ��λ�ã�ָ������ݽ���Ƕ�뵽�ĵ��е�ǰ��ǩ����λ�ã�������src��Դʱ�Ὣ��ָ�����Դ���ز�Ӧ�õ��ĵ��ڣ�����js�ű���imgͼƬ��frame��Ԫ�ء����������������Ԫ��ʱ������ͣ������Դ�����غʹ���ֱ��������Դ���ء����롢ִ����ϣ�ͼƬ�Ϳ�ܵ�Ԫ��Ҳ��ˣ������ڽ���ָ����ԴǶ�뵱ǰ��ǩ�ڡ���Ҳ��Ϊʲô��js�ű����ڵײ�������ͷ����

**5��ʲô��CSS Hack?**

һ����˵����Բ�ͬ�������д��ͬ��CSS,���� CSS Hack��

IE�����Hackһ���ַ�Ϊ���֣�����Hack�����Լ�Hack��ѡ���Hack����ϸ�ο�CSS�ĵ���css�ĵ��������磺

*1������Hack*

```html
<!--[if IE]>
  <style>
		.test{color:red;}
  </style>
<![endif]-->
```

*2������Hack*

```css
.test{
color:#090\9; /* For IE8+ */
*color:#f00;  /* For IE7 and earlier */
_color:#ff0;  /* For IE6 and earlier */
}
```

*3��ѡ���Hack*

```css
* html .test{color:#090;}       /* For IE6 and earlier */
* + html .test{color:#ff0;}     /* For IE7 */
```

**6������ͬ�����첽������**

ͬ��������ģʽ���첽�Ƿ�����ģʽ��

ͬ������ָһ��������ִ��ĳ�������ʱ������������Ҫһ��ʱ����ܷ�����Ϣ����ô������̽���һֱ�ȴ���ȥ��ֱ���յ�������Ϣ�ż���ִ����ȥ��

�첽��ָ���̲���Ҫһֱ����ȥ�����Ǽ���ִ������Ĳ����������������̵�״̬��������Ϣ����ʱϵͳ��֪ͨ���̽��д��������������ִ�е�Ч�ʡ�

**7��px��em������**

px��em���ǳ��ȵ�λ�������ǣ�px��ֵ�ǹ̶��ģ�ָ���Ƕ��پ��Ƕ��٣�����Ƚ����ס�em��ֵ���ǹ̶��ģ�����em��̳и���Ԫ�ص������С��

�������Ĭ������߶���16px������δ�������������������: 1em=16px����ô12px=0.75em, 10px=0.625em

**8��ʲô�����Ž����ͽ�����ǿ��**

*������ǿ progressive enhancement��*

��ԵͰ汾��������й���ҳ�棬��֤������Ĺ��ܣ�Ȼ������Ը߼����������Ч���������ȸĽ���׷�ӹ��ܴﵽ���õ��û����顣

*���Ž��� graceful degradation��*

һ��ʼ�͹��������Ĺ��ܣ�Ȼ������ԵͰ汾��������м��ݡ�

����

a. ���Ž����ǴӸ��ӵ���״��ʼ������ͼ�����û�����Ĺ���

b. ������ǿ���Ǵ�һ���ǳ������ģ��ܹ������õİ汾��ʼ�����������䣬����Ӧδ����������Ҫ

c. ����������˥������ζ�����ؿ�����������ǿ����ζ�ų�ǰ����ͬʱ��֤��������ڰ�ȫ�ش�

**9����������ں˷ֱ���ʲô?**

IE: trident�ں�

Firefox��gecko�ں�

Safari��webkit�ں�

Opera����ǰ��presto�ںˣ�Opera���Ѹ���Google Chrome��Blink�ں�

Chrome��Blink(����webkit��Google��Opera Software��ͬ����)

###JavaScript����

**1��������ӡ��Ƴ����ƶ������ơ������Ͳ��ҽڵ㣿**

1�������½ڵ�

```javascript
createDocumentFragment() //����һ��DOMƬ��
createElement() //����һ�������Ԫ��
createTextNode() //����һ���ı��ڵ�
```

2����ӡ��Ƴ����滻������

```javascript
appendChild() //���
removeChild() //�Ƴ�
replaceChild() //�滻
insertBefore() //����
```

3������

```
getElementsByTagName() //ͨ����ǩ����
getElementsByName() //ͨ��Ԫ�ص�Name���Ե�ֵ
getElementById() //ͨ��Ԫ��Id��Ψһ��
```

**2��ʵ��һ������clone�����Զ�JavaScript�е�5����Ҫ���������ͣ�����Number��String��Object��Array��Boolean������ֵ���ơ�**

```javascript
/**
 * �����¡
 * ֧�ֻ����������ͼ�����
 * �ݹ鷽��
 */
function clone(obj) {
    var o;
    switch (typeof obj) {
        case "undefined":
            break;
        case "string":
            o = obj + "";
            break;
        case "number":
            o = obj - 0;
            break;
        case "boolean":
            o = obj;
            break;
        case "object": // object ��Ϊ������� ����Object�������飨Array��
            if (obj === null) {
                o = null;
            } else {
                if (Object.prototype.toString.call(obj).slice(8, -1) === "Array") {
                    o = [];
                    for (var i = 0; i < obj.length; i++) {
                        o.push(clone(obj[i]));
                    }
                } else {
                    o = {};
                    for (var k in obj) {
                        o[k] = clone(obj[k]);
                    }
                }
            }
            break;
        default:
            o = obj;
            break;
    }
    return o;
}
```

**3���������һ�����������ظ���Ԫ�أ�**

*����һ��*

```javascript
var arr1 =[1,2,2,2,3,3,3,4,5,6],
    arr2 = [];
for(var i = 0,len = arr1.length; i< len; i++){
    if(arr2.indexOf(arr1[i]) < 0){
        arr2.push(arr1[i]);
    }
}
document.write(arr2); // 1,2,3,4,5,6
```

**4����ʵ��һ����ҳ��ĳ���ڵ����ҷ�����������ʹ��ԭ��JS����**

**5����Javascript��ʲô��α���飿��ν�α����ת��Ϊ��׼���飿**

α���飨�����飩���޷�ֱ�ӵ������鷽��������length������ʲô�������Ϊ�����Կ��Զ�������������������������ǡ����͵��Ǻ�����argument���������������getElementsByTagName,document.childNodes֮���,���Ƕ�����NodeList��������α���顣����ʹ��Array.prototype.slice.call(fakeArray)������ת��Ϊ������Array����

```javascript
function log(){
      var args = Array.prototype.slice.call(arguments);  
//Ϊ��ʹ��unshift���鷽������argumentת��Ϊ����������
      args.unshift('(app)');

      console.log.apply(console, args);
};
```

**6��Javascript��callee��caller�����ã�**

caller�Ƿ���һ���Ժ��������ã��ú��������˵�ǰ������

callee�Ƿ������ڱ�ִ�е�function������Ҳ������ָ����function��������ġ�

**7��������һ��cookies��sessionStorage��localStorage������**

sessionStorage���ڱ��ش洢һ���Ự��session���е����ݣ���Щ����ֻ����ͬһ���Ự�е�ҳ����ܷ��ʲ��ҵ��Ự����������Ҳ��֮���١����sessionStorage����һ�ֳ־û��ı��ش洢�������ǻỰ����Ĵ洢����localStorage���ڳ־û��ı��ش洢����������ɾ�����ݣ�������������Զ������ڵġ�

*web storage��cookie������*

Web Storage�ĸ����cookie���ƣ�����������Ϊ�˸��������洢��Ƶġ�Cookie�Ĵ�С�����޵ģ�����ÿ��������һ���µ�ҳ���ʱ��Cookie���ᱻ���͹�ȥ�������������˷��˴�������cookie����Ҫָ�������򣬲����Կ�����á�

����֮�⣬Web Storageӵ��setItem,getItem,removeItem,clear�ȷ���������cookie��Ҫǰ�˿������Լ���װsetCookie��getCookie������CookieҲ�ǲ����Ի�ȱ�ģ�Cookie������������������н�������ΪHTTP�淶��һ���ֶ����� ����Web Storage������Ϊ���ڱ��ء��洢�����ݶ�����

**8����д�����������**

���ڿ����㷨����ϸ˵�������Բο���һ����ʦ�����¿�������

���������򡱵�˼��ܼ򵥣������������ֻ��Ҫ������

��1�������ݼ�֮�У�ѡ��һ��Ԫ����Ϊ����׼����pivot����
��2������С�ڡ���׼����Ԫ�أ����Ƶ�����׼������ߣ����д��ڡ���׼����Ԫ�أ����Ƶ�����׼�����ұߡ�
��3���ԡ���׼����ߺ��ұߵ������Ӽ��������ظ���һ���͵ڶ�����ֱ�������Ӽ�ֻʣ��һ��Ԫ��Ϊֹ��

**9��ͳ���ַ�����aaaabbbccccddfgh������ĸ������ͳ�������ĸ����**

```javascript
var str = "aaaabbbccccddfgh";
var obj  = {};
for(var i=0;i<str.length;i++){
    var v = str.charAt(i);
    if(obj[v] && obj[v].value == v){
        obj[v].count = ++ obj[v].count;
    }else{
        obj[v] = {};
        obj[v].count = 1;
        obj[v].value = v;
    }
}
for(key in obj){
    document.write(obj[key].value +'='+obj[key].count+' '); // a=4  b=3  c=4  d=2  f=1  g=1  h=1 
}
```

**10��дһ��function������ַ���ǰ��Ŀո񡣣����������������**

```javascript
function trim(str) {
    if (str && typeof str === "string") {
        return str.replace(/(^\s*)|(\s*)$/g,""); //ȥ��ǰ��հ׷�
    }
}
```

###����

**1��һ��������HTTP������������һ�����̣�**

�������̣�

a. ��������

b. ����TCP��3������

c. ����TCP���Ӻ���http����

d. ����������Ӧhttp����������õ�html����

e. ���������html���룬������html�����е���Դ

f. �������ҳ�������Ⱦ���ָ��û�

2����ǰ�˹���ʦ���ְλ������ô�����ģ�

a. ǰ�����������û��ĳ���Ա��ǰ�˵������������ò�Ʒ�� 90�ֽ����� 100 �֣���������

b. ������Ŀ�����ٸ��������ʵ��Ч��ͼ����ȷ��1px��

c. ���Ŷӳ�Ա��UI��ƣ���Ʒ����Ĺ�ͨ��

d. ���õ�ҳ��ṹ��ҳ���ع����û����飻

e. ����hack�����ݡ�д�������Ĵ����ʽ��

f. ��Է��������Ż���ӵ������ǰ�˼�����