# devops-tricks


* [Ansible, Docker, Curl, HTTP] get http status code from containers to ensure working host resolution 

```js
 $ ansible --inventory-file="inventory.ini" gitlab-runners -a "docker run pstauffer/curl:latest curl -s -o /dev/null -w '%{http_code}' http://google.com" -b
 ```


