���ذ�װ
English German Russian

ƽ̨֧��
V2Ray ������ƽ̨�п��ã�

Windows 7 ��֮��汾��x86 / amd64����
Mac OS X 10.10 Yosemite ��֮��汾��amd64����
Linux 2.6.23 ��֮��汾��x86 / amd64 / arm / arm64 / mips64 / mips����
������������ Debian 7 / 8��Ubuntu 12.04 / 14.04 �������汾��CentOS 6 / 7��Arch Linux��
FreeBSD (x86 / amd64)��
OpenBSD (x86 / amd64)��
Dragonfly BSD (amd64)��
Ӳ��Ҫ��
���� 32MB �����ڴ棬�Ƽ� 64MB ����ࡣ

���� V2Ray
Ԥ�����ѹ�������������¼���վ���ҵ���

Github Release: github.com/v2ray/v2ray-core
Github ����: v2ray.com/download
ѹ������Ϊ zip ��ʽ���ҵ���Ӧƽ̨��ѹ���������ؽ�ѹ����ʹ�á�

��֤��װ��
V2Ray �ṩ������֤��ʽ��

��װ�� zip �ļ��� SHA1 ժҪ��������ҳ��� metadata.txt �ļ��п����ҵ���
�����г���v2ray �� v2ray.exe���� gpg ǩ�����ļ�λ�ڰ�װ���е� v2ray.sig �� v2ray.exe.sig��ǩ����Կ�����ڴ�������ҵ���
Windows �� Mac OS ��װ��ʽ
ͨ��������ʽ���ص�ѹ��������ѹ֮��ɿ��� v2ray �� v2ray.exe��ֱ�����м��ɡ�

Linux ��װ�ű�
V2Ray �ṩ��һ���� Linux �е��Զ�����װ�ű�������ű����Զ������û�а�װ�� V2Ray�����û�У�����������İ�װ�����ã����֮ǰ��װ�� V2Ray����ֻ���� V2Ray �����Ƴ�������������á�

����ָ��������� su �����£�������ǣ��������� sudo su��

���������ָ�����ز���װ V2Ray���� yum �� apt-get ���õ�����£��˽ű����Զ���װ unzip �� daemon������������ǰ�װ V2Ray �ı�Ҫ����������ʹ�õ�ϵͳ��֧�� yum �� apt-get�������а�װ unzip �� daemon

bash <(curl -L -s https://install.direct/go.sh)
�˽ű����Զ���װ�����ļ���

/usr/bin/v2ray/v2ray��V2Ray ����
/usr/bin/v2ray/v2ctl��V2Ray ���ߣ�
/etc/v2ray/config.json�������ļ���
/usr/bin/v2ray/geoip.dat��IP �����ļ�
/usr/bin/v2ray/geosite.dat�����������ļ�
�˽ű��������Զ����нű����Զ����нű�����ϵͳ����֮���Զ����� V2Ray��Ŀǰ�Զ����нű�ֻ֧�ִ��� Systemd ��ϵͳ���Լ� Debian / Ubuntu ȫϵ�С�

���нű�λ��ϵͳ������λ�ã�

/etc/systemd/system/v2ray.service: Systemd
/etc/init.d/v2ray: SysV
�ű�������ɺ�����Ҫ��

�༭ /etc/v2ray/config.json �ļ�����������Ҫ�Ĵ���ʽ��
���� service v2ray start ������ V2Ray ���̣�
֮�����ʹ�� service v2ray start|stop|status|reload|restart|force-reload ���� V2Ray �����С�
go.sh ����
go.sh ֧�����²����������ֶ���װʱ����ʵ�����������

-p �� --proxy: ʹ�ô�������������� V2Ray ���ļ�����ʽ�� curl ���ܵĲ���һ�£����� "socks5://127.0.0.1:1080" �� "http://127.0.0.1:3128"��
-f �� --force: ǿ�ư�װ����Ĭ������£������ǰϵͳ���������°汾�� V2Ray��go.sh ���ڼ��֮����˳��������Ҫǿ����װһ�飬����Ҫָ���ò�����
--version: ָ����Ҫ��װ�İ汾������ "v1.13"��Ĭ��ֵΪ���°汾��
--local: ʹ��һ�������ļ����а�װ��������Ѿ�������ĳ���汾�� V2Ray�����ͨ���������ָ��һ���ļ�·�������а�װ��
ʾ����

ʹ�õ�ַΪ 127.0.0.1:1080 �� SOCKS �������ز���װ���°汾��./go.sh -p socks5://127.0.0.1:1080
��װ���ص� v1.13 �汾��./go.sh --version v1.13 --local /path/to/v2ray.zip
Docker
V2Ray �ṩ������Ԥ����� Docker image��

v2ray/official: �������·����İ汾��ÿ�ܸ����°汾���£�
v2ray/dev: ���������µĴ��������ɵĳ����ļ�����������£�
���� image ���ļ��ṹ��ͬ��

/etc/v2ray/config.json: �����ļ�
/usr/bin/v2ray/v2ray: V2Ray ������
/usr/bin/v2ray/v2ctl: V2Ray ��������
/usr/bin/v2ray/geoip.dat: IP �����ļ�
/usr/bin/v2ray/geosite:dat: ���������ļ�