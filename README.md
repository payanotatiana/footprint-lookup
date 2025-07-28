# footprint-lookup
pip install googlesearch-python
from googlesearch import search

# List of identifiers you want to trace
identifiers = [
    "Tatiianaax0",
    "Tatianastar100@gmail.com",
    "Payanotatiana@gmail.com",
    "9144267373"
]

# Search each identifier on Google and print the results
for item in identifiers:
    print(f"\n🔍 Searching for: {item}")
    query = f'"{item}"'
    try:
        for url in search(query, num_results=10):
            print(url)
    except Exception as e:
        print(f"Error searching {item}: {e}")
