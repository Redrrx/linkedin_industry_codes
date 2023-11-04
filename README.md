# linkedin_industry_codes
Linkedin industry codes V2 JSON 


open the file 

```python
with open('industry_data.json', 'r') as f:
    all_industry_data = json.load(f)
```

basic function to return the industry for the code.

```python
def get_industry_label(industry_id):
    return next((item['label'] for item in all_industry_data if item['id'] == industry_id), None)
```
