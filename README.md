# zos
�����ַ��

http://zos-wwccss.alaudacn.me/

��������֪��Ȼ֮�Ĺ���Ա�ʺź����붼�ǣ�admin 123456 ��֪�ĺ�̨��ַ��http://localhost/chanzhi/admin.php

��������

ZOS���ൺ�����촴����Ƽ����޹�˾����ά�����ൺ�����촴������Ϊ������ҵ�ṩרҵ�Ĺ����ߡ������Ⱥ��Կ�Դ�ķ�ʽ������������Ŀ�����������֪��ҵ�Ż�ϵͳ��Ȼ֮Эͬ����ϵͳ��

ZOS�ı���

�ڿ���ά���⼸�Դ����Ĺ����У�����������һ���Ƚϼ��ֵ����������ο��ټ������û���װ�ɹ���Ϊ���������˸��ֵĳ��ԣ������а�������windows��һ����װ����linux��һ����װ����rpm��,deb���ȵȡ�

�������ǳ���ʹ������ṩova��ʽ��������񡣵������������Ǹ���linux���а汾���ǳ����Ӵ������ľ�����������Ҫ�����ף������ڷ��к����ء�Ϊ�����ǳ����˸��ַ��а汾������ѡ���˸���LFS(linux from scratch)���б��롣

���°汾��ZOS�Ǹ���LFS 7.6����ġ��ڻ�����LFS���棬�����ֽ��BLFS������apache, mariadb, php, vim�ȳ����ķ���͹��ߣ������������ǵ����Դ���������

ZOS�ص�

ZOS��Ҫ������ҵ�ڲ���������ּ��Ϊ���ֹ�������ṩһ�ֹ�װ�ķ��з�������Ӧ��Խ��Խ���ӵ��ն˳�����
ZOS���ǹ�������ϵͳ��Ҳ�����������а汾�ľ���汾��������linux from scratch 7.6���б���ġ�
ZOS����һ��ͨ�÷��а汾����Ҫ������apache, php, mysql, openssh, cron, vim, rzsz, phpmyadmin������ͷ���
ZOS�����˴����ľ��������docker����ֻ��175M����ʹ��ubuntu����������ͬ���Ĺ��ܵľ���ﵽ��460��M��
ZOS�����˼򵥵İ�������(pkg)������ʵ�ּ򵥵��б���ѯ���鿴����װ��ɾ���Ȳ�����
���ʹ��

docker pull index.alauda.cn/wwccss/zos:1.1
docker run --name zos -d -p 80:80 zos /bin/start
Ȼ��ʹ�����������������ip���������Ϳ��Կ����ˡ�
�˻�˵��

��������֪��Ȼ֮�Ĺ���Ա�ʺź����붼�ǣ�admin 123456 ��֪�ĺ�̨��ַ��http://localhost/chanzhi/admin.php

�ĵ�

ȥ���ʱ�����Լ�����һ��docker������������վ( http://www.docker.org.cn )��������docker�Ļ��������ֲᡣ���Զ�docker�л������˽⡣������������ʱ����Ҫ�����ļ������⣺

����þ�����Ϊ�����˳��������кܶ෽���ˡ�������ѡ�������� tail -f һ���ļ���ȡ�ɵķ�ʽ��ʵ�֡�
��ν��Լ�����ZOS����Ϊ���񣬱�����Ϊ�ܸ��ӣ�����ʵ���Ǻܼ��ˡ���Ҫ�ο��˺�ñ��һƪ���� http://developerblog.redhat.com/2014/05/15/practical-introduction-to-docker-containers/

* ֧��Markdown��ʽ ��������
user-logo whopawho   ������ 24 ��ǰ
�㶨��ԭ������Ҫ��url�;���tag

sudo docker run --name='zos' -d -p 80:80 index.alauda.cn/wwccss/zos:1.1 /bin/start
 user-logo whopawho   ������ 24 ��ǰ
~$ sudo docker run --name zos -d -p 80:80 zos /bin/start
Unable to find image 'zos:latest' locally
����ʱ����ʾ�Ҳ�������

 user-logo whopawho   ������ 24 ��ǰ
��һ�����������ԡ������ڹ��ڻ��Ƿǳ�����ģ�
