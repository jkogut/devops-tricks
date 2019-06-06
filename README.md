# devops-tricks


# [Ansible, Docker, Curl, HTTP] get hhtp status code from containers to be sure about working host resolution 

```js
 $ ansible --inventory-file="inventory.ini" gitlab-runners -a "docker run pstauffer/curl:latest curl -s -o /dev/null -w '%{http_code}' http://google.com" -b
 ```

 