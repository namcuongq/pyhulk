# pyhulk
## Worker

### Example Use

[embedmd]:# (example/basic/server.go go)
```py
def task(job):
  print(job)
  
number_worker = 10
worker = Worker(task,number_worker)

for i in 10:
  worker.add_job(i)
  
worker.wait_and_stop()
```
