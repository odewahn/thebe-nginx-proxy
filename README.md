This is an nginx proxy that will serve a static site and a Jupyter Notebook backend for thebe from the same domain.

You should start jupyter on port 8888:

```
jupyter notebook --NotebookApp.allow_origin='*' --no-browser --port 8888 --ip=*
```

Start the nginx proxy on localhost:

```
nginx -c /Users/odewahn/Desktop/nginx-proxy/nginx.conf
```

Go to localhost:9000 and be able to run the thebe code widgets.
