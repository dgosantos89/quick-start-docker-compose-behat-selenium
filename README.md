# quick-start-docker-compose-behat-selenium
Example of use docker-compose and behat to test

# requirements
- docker + docker-compose => [recommended docker toolbox](https://www.docker.com/products/docker-toolbox)
- 5GB disk space

## generate dependencies
docker-compose -f docker-compose.vendor.yml up

## run tests
docker-compose -f docker-compose.yml -f docker-compose.testing.yml up -d
## wait results
docker wait quickstartdockercomposebehatselenium_tests-wordpress_1
## see results
docker logs quickstartdockercomposebehatselenium_tests-wordpress_1
