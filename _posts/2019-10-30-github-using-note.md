---
layout: post
title: Ӣ�ﱳ�����ĵ����2
date: 2019-10-30
categories: blog
tags: [����ѧϰ,��֪]
description: some tips I gets from the study of reciting English words��
---


---
layout: post
title: githubʹ��note
date: 2019-10-30
categories: blog
tags: [github,�������]
description: some tips I gets from the study of reciting English words��
---

# �������
��վ��һ��������������Լ���Ŀ�����ߣ�����folk���˵Ĵ��룬������֧ branch���Լ������޸ģ�pull�ύ������Է�ͬ����İ汾����merge������İ汾�ںϽ�������
1.��Ҫע���˺�
2.�����Լ��Ŀ⣬public����private������public�Ĳ���������ɾ�̬ҳ�棬�������࣬��Github Page
## ����������fork/clone/push/pull
[github��fork,clone,push,pull request�ļ���� - cvper's world ! - CSDN����](https://blog.csdn.net/cvper/article/details/79035664)

## �ͻ��˹����� Github Desktop
> Github Desktop :�ٷ�����
> 
ֻ�ǰ汾�����ܣ�clone������folk�󽫿����ص����ԡ������޸���Ҫ�Լ�ʹ��IDE�����޸ĵ��ԡ� 
����ļ����ݱ仯����������Github Desktop��pull�ύ���Լ�����

## Github Page����д����Jekyll����

Jekyll����һ���򵥡�����չ�ľ�̬վ�����������ı�����֧��md��ʽ��github page �ڲ�֧��jekyll������ֻҪͨ����������վ���ϴ���github���У�Ȼ���趨���setting�����ɡ�
> http://jekyllcn.com/
> 
��װ����
1. ruby�Ѱ�װ
2. ruby �����н�ȥ��
> gem install jekyll bundler
3. cd ����Ŀ¼������վ,����������
> jekyll new myblog
> cd myblog
> bundle exec jekyll serve
4. ��������д� http://localhost:4000 ��ַ
```
����� $ jekyll serve ���� $ jekyll serve �Cwatch�����ܺ�jekyll serve��ͬ�����ǿ����ڷ���������������޸����ݲ���ͬ�����¡���˵���ǣ������ٴ���������Ϳ���ˢ����������޸Ĺ������ݡ�
```

## ʹ�����еĲ���ģ�� : cnfeatΪ��
��public�����ҳ��setting�У���pages��ѡ������ѡ��
���ñ����Ѿ�д�õ�ģ�棬ʹ��md�ļ��������ÿ�ղ���
>cnfeat��GitHub��ַ��https://github.com/cnfeat/blog.io
>��ؽ��ܣ�[��δһ���������͡�������Github Pages��Hexo�̳� - ����](https://www.jianshu.com/p/05289a4bc8b2)
### ��ʼ����
1. ��github�����folk���������Լ���Ŀ��setting���������Ŀ��
2. ���Լ�folk��Ĺ��̣���clone���ͻ����Զ�����������
3. ��desktop�ͻ����д򿪿�repository���Ҽ����򿪱����ļ��У�
4. �޸�cmake�ļ�����Ϊ�Լ�Ҫ������
> cmake����:showna.cnfeat.com
5. �޸ĺ���desktop�ͻ��ˣ�changes�·�����commit�ύ��Ȼ�����ұߵ�pushing���Ž��޸��ϴ�����ӳ����ҳ��
6. .����ҳ�ϣ����setting���ҵ�GitHub Pages��ѡ���֧�����⣬
7. �����յ��ʼ������ʲ�����ַ�����ɡ�
```
�ʼ����ݣ�
The page build completed successfully, but returned the following warning for the `master` branch:
Your site's DNS settings are using a custom subdomain, showna.cnfeat.com, that's set up as an A record. We recommend you change this to a CNAME record pointing at showna-wei.github.io
.����
```
> ������ַ:http://showna.cnfeat.com/ 

#### �ɰ汾��jekyll-site ���±���

* ִ�У�bundle exec jekyll serve
* ��ʾ����Could not locate Gemfile or .bundle/ directory��
* siteĿ¼���½��ļ���Gemfile��������� [Ruby x Jekyll ���ص��Ի����](https://szhshp.org/tech/2015/11/14/localjekyllenv.html)
* ִ�У� Bundle install


 
### ���²���

���Ĳ��ͻ�����Ϣ����[������ַ](https://www.jianshu.com/p/05289a4bc8b2)

* �������ּ�������Ϣ��_config.yml
* ���˽���ҳ�棺about.md
* ������ҳ�棺milestone.md
* ����ģ�壺blog.io/_posts/2015-03-02-how-to-write.md

�޸���
���Ӳ��ģ�
* ��blog.io�ļ��������½�md�ļ���ǰ����̶���prefix
```
---
layout: post
title: Ӣ�ﱳ�����ĵ����
date: 2019-10-30
categories: blog
tags: [����ѧϰ,��֪]
description: some tips I gets from the study of reciting English words��
---

�����ǲ������ġ�
```
> ������Ϣ����Ҫ���±�������ϴ�����Ȼ�ܶ���Ϣ�����£���
> ruby �����н���Ŀ¼ �����У�bundle exec jekyll serve -watch

[jekyll ���� - һЩ�е�û�� - CSDN����](https://blog.csdn.net/uselym/article/details/73608638)


