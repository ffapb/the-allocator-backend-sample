# the-allocator-backend-sample
Sample backend for [the-allocator](https://github.com/shadiakiki1986/the-allocator)

# Usage
1. Run `the-allocator` with the local `the-allocator-config.json` mounted in `www`
 * `docker run -d -p 6543:80 -v the-allocator-config.json:/code/the-allocator/www/the-allocator-config.json shadiakiki1986/the-allocator`
2. Run this backend
 * `docker run -d -p 6544:80 shadiakiki1986/the-allocator-backend-sample`
3. Open `the-allocator` in a browser. The `EADS` should be detected
