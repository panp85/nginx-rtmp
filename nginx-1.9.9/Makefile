
default:	build

clean:
	rm -rf Makefile objs

build:
	$(MAKE) -f objs/Makefile
	$(MAKE) -f objs/Makefile manpage

install:
	$(MAKE) -f objs/Makefile install

upgrade:
	/home/panpan/rk/nginx/nginx-1.9.9/test/sbin/nginx -t

	kill -USR2 `cat /home/panpan/rk/nginx/nginx-1.9.9/test/logs/nginx.pid`
	sleep 1
	test -f /home/panpan/rk/nginx/nginx-1.9.9/test/logs/nginx.pid.oldbin

	kill -QUIT `cat /home/panpan/rk/nginx/nginx-1.9.9/test/logs/nginx.pid.oldbin`
