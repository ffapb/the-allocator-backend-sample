# the-allocator-backend-sample
Sample backend for [the-allocator](https://github.com/shadiakiki1986/the-allocator)

# Usage
1. Either build or pull `the-allocator` image
 * Check `the-allocator` [usage](https://github.com/shadiakiki1986/the-allocator#Usage)
2. Run `docker-compose up --force-recreate -d` (check `docker-compose.yml`). What this does is:
 * Run `the-allocator` with the local `the-allocator-config.json` mounted in `www`
 * Run this backend
  * Could be done with docker: `docker run --rm --name the-allocator-backend-sample -p 6544:80 -v $(pwd)/www:/usr/share/nginx/html:ro nginx:alpine`
3. Open `the-allocator` in a browser. The `EADS` should be detected
