# the-allocator-backend-sample
Sample backend for [the-allocator](https://github.com/shadiakiki1986/the-allocator)

# Usage
1. Either build or pull `the-allocator` image
 * Check `the-allocator` [usage](https://github.com/shadiakiki1986/the-allocator#Usage)
2. Copy `config/the-allocator-config-sample.json` to `config/the-allocator-config.json` and edit if needed
* if the development server is not `localhost`, replace `localhost` with the IP of your host as seen from the browser
3. check `docker-compose.yml`
* if the volume binding in the `docker-compose.yml` is kept to use the development folder, make sure to run `make install` in the dev folder. 
4. Run `docker-compose up --force-recreate -d` (check `docker-compose.yml`). What this does is:
 * Run `the-allocator` with the local `the-allocator-config.json` mounted in `www`
 * Run this backend
  * Could be done with docker: `docker run --rm --name the-allocator-backend-sample -p 6544:80 -v $(pwd)/www:/usr/share/nginx/html:ro nginx:alpine`
5. Open http://localhost:6543 in a browser. The `EADS` should be detected
