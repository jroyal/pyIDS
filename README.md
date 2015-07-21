# pyIDS
Python wrapper for IDS(IBM Bluemix Devops Services)

---

### What this is?

This is an attempt by me to create a helpful python wrapper for the IDS track and plan dashboards for my own uses. You can use it if you like, and feel free to add to it if you want to help.

### What this is not?

This is not in anyway official IBM software. I'm writing this on my own time for kicks and giggles in an attempt to learn something new. Assuming this works for you and you still want to use it lets move on.

---

## Installation

```bash
pip install pyIDS
```

## Example Usage

```python
from pyIDS import IDS

client = IDS("https://hub.jazz.net/ccm10", "user", "pass")

workitem = client.get_work_item_by_id("16219")

my_workitems = client.get_work_items_by_owner("James Royal")

print workitem.id
print workitem.description
print workitem.priority
```
