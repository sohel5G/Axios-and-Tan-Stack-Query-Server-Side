----------------------------------
Deploy to vercel 
----------------------------------
1. npm i -g vercel
2. create vercel.json file 
```JavaScript
{
    "version": 2,
    "builds": [
        {
            "src": "./index.js",
            "use": "@vercel/node"
        }
    ],
    "routes": [
        {
            "src": "/(.*)",
            "dest": "/",
            "methods": ["GET", "POST", "PUT", "PATCH", "DELETE", "OPTIONS"]
        }
    ]
}
```
3. vercel (in the command)
4. set Environment Variable
5. vercel --prod
6. finally get the url and replace it on the frontend side


