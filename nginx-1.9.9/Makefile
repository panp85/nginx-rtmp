
default:	build

clean:
	rm -rf Makefile objs

build:
	$(MAKE) -f objs/Makefile
	$(MAKE) -f objs/Makefile manpage

install:
	$(MAKE) -f objs/Makefile install

upgrade:
	/mnt/w3/panpan/player/nginx-1.9.9/nginx-pp-git/nginx-rtmp/nginx-1.9.9/test/sbin/nginx -t

	kill -USR2 `cat /mnt/w3/panpan/player/nginx-1.9.9/nginx-pp-git/nginx-rtmp/nginx-1.9.9/test/logs/nginx.pid`
	sleep 1
	test -f /mnt/w3/panpan/player/nginx-1.9.9/nginx-pp-git/nginx-rtmp/nginx-1.9.9/test/logs/nginx.pid.oldbin

	kill -QUIT `cat /mnt/w3/panpan/player/nginx-1.9.9/nginx-pp-git/nginx-rtmp/nginx-1.9.9/test/logs/nginx.pid.oldbin`
