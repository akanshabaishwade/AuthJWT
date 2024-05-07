# AuthJWT

## API Endpoints

- `POST /register/`: Register a new user.
- `POST /login/`: Login and get JWT tokens.

## Dummy User for Testing

You can use the following dummy user for testing:

- Email: `test_user@example.com`
- Password: `test_password`
- json: `{
    "email": "test_user@example.com",
    "password": "test_password"
}`

## How to Test

You can test the APIs using tools like Postman or curl. Here's how you can test the registration and login APIs using the dummy user:

1. **Registration:**
   - **Method:** POST
   - **URL:** `http://127.0.0.1:8000/register/`
   - **Body:** JSON data with email and password
   - **Expected Response:** User created successfully (status 201) or validation errors (status 400)
   - ![image](https://github.com/akanshabaishwade/AuthJWT/assets/85228361/df8f0a74-dc71-4b7c-a4e6-77a780221a38)


2. **Login:**
   - **Method:** POST
   - **URL:** `http://127.0.0.1:8000/login/`
   - **Body:** JSON data with email and password
   - **Expected Response:** JWT tokens (status 200) or Invalid credentials (status 401)
   - ![image](https://github.com/akanshabaishwade/AuthJWT/assets/85228361/fa561aba-b817-4a7b-a304-0e8756dc7706)
  
3. **Manohar Sir's Question Solution**
```python
nums = [1, 2, 3, 4, 5, 1, 2, 3, 9]
count = {}
unique = []

for i in nums:
    if i not in unique:
        unique.append(i)

    if i in count:
        count[i] += 1
    else:
        count[i] = 1

print(count)
print(unique)

