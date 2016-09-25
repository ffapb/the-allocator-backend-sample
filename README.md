# the-allocator-backend-sample
Sample backend for [the-allocator](https://github.com/shadiakiki1986/the-allocator)

# Usage
1. Run `the-allocator` with the local `the-allocator-config.json` mounted in `www`
 * `docker run -d -p 6543:80 -v the-allocator-config.json:/usr/share/nginx/html/the-allocator-config.json shadiakiki1986/the-allocator`
2. Run this backend
 * `docker run --name the-allocator-backend-sample -d -p 6544:80 -v www:/usr/share/nginx/html:ro nginx:alpine`
3. Open `the-allocator` in a browser. The `EADS` should be detected
