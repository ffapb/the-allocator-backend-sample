# the-allocator-backend-sample
Sample backend for [the-allocator](https://github.com/shadiakiki1986/the-allocator)

# Usage
1. Run `the-allocator` with the local `the-allocator-config.json` mounted in `www`
 * Check `the-allocator` [usage](https://github.com/shadiakiki1986/the-allocator#Usage)
2. Run this backend
 * With docker: `docker run --rm --name the-allocator-backend-sample -p 6544:80 -v $(pwd)/www:/usr/share/nginx/html:ro nginx:alpine`
 * With docker-compose:
  * `docker-compose up --force-recreate -d`
  * check `docker-compose.yml`
3. Open `the-allocator` in a browser. The `EADS` should be detected
