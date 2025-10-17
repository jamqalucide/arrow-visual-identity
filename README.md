# phnxq

message queue. simple.

```bash
docker run -p 6000:6000 phnxq/phnxq:latest
```

```python
import phnxq

q = phnxq.connect("localhost:6000")
q.push("tasks", {"action": "send_email"})

msg = q.pop("tasks")
print(msg)
```

that's it.

no kafka complexity. no rabbitmq config hell. just works.

[github](https://github.com/queue-systems/phnxq) • MIT

# PR Update: 2025-10-17 - fix/update-1767
