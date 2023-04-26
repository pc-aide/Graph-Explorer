# batch

---

## beta ou v1.0
1. beta give more attributes vs v1.0

---

## sample
1. Method : Post
2. ApiVersion : beta
3. URL : `https://graph.microsoft.com/beta/$batch`
4. Request body
````json
{
    "requests": [
        {
            "id": "1",
            "method": "GET",
            "url": "/me"
        },
        {
            "id": "2",
            "method": "GET",
            "url": "/users"
        }
    ]
}
````
