Anotações importantes da documentação

Where should this code live?

If your background is in plain old PHP (with no use of modern frameworks), you’re probably used to putting code under the Web server’s document root (in a place such as /var/www). With Django, you don’t do that. It’s not a good idea to put any of this Python code within your Web server’s document root, because it risks the possibility that people may be able to view your code over the Web. That’s not good for security.

Put your code in some directory outside of the document root, such as /home/mycode.

python manage.py runserver 0:80