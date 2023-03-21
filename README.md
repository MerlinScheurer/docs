# Tube Archivist Documentation

This is a work in progress, porting the old wiki to a more flexible documentation framework.


## Development Environment

To just make simple changes, edit the markdown files within *mkdocs/docs* direclty.

To setup a local development server:

Install mkdocs with pip:
```
pip3 install mkdocs mkdocs-material
```

From the AUR:
```
yay -S mkdocs mkdocs-material
```

More details: [User Guide](https://www.mkdocs.org/user-guide/installation/)

Run the server from the *mkdocs* folder with:
```
mkdocs serve
```

And the site - with live reload enabled - should be available on [localhost:8000](http://localhost:8000/).

## Production environment
Build the Docker image:
```
docker build -t bbilly1/tubearchivist-docs .
```

Run the image:
```
docker run -p 80:80 bbilly1/tubearchivist-docs
```
