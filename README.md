# textfsms

Example to use TFSM

```
import io
import textfsm

# Update file locations
template = open('calix/show_ont_detail', 'r').read()
text = open('calix/show_ont_detail_example', 'r').read()

fsm = textfsm.TextFSM(io.StringIO(template))
parsed_text = fsm.ParseText(text)


for item in parsed_text:
    print(item)
```
