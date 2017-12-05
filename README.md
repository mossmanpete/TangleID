# TangleID

# Get started

- Create a `.env` file, and specify `OFF_TANGLE_USERS_LINK` and `HOST_API`

```
OFF_TANGLE_USERS_LINK=https://tangleidentity.firebaseio.com/users.json
HOST_API=http://node0.puyuma.org/tangleid_backend/api/
```

```
$> npm install
```

For dev:

```
$> npm run dev
```

For production build:

```
$> npm run build && npm start
```

# Directory structure

# Dev note

- [ ] Users Page(Temporary landing page): `/` or `/users`
  - [x] Fetch offtangle user list
  - [x] use login api to check

- [ ] User Page: `/users/:id`
  - [ ] Make claim of specified user
    - [ ] use new claim api: [doc](https://hackmd.io/s/HJyzQvF1z)
  - [ ] List claims of specified user
    - [ ] use get all claims api: [doc](https://hackmd.io/s/Sku7aPFkM#)

- [ ] New User Page: `/users/new`
  - prepare
    - [ ] retrieve key pairs
    - [ ] create uuid
  - [ ] Create new user
    - [ ] send previous as body to new user api([doc](https://hackmd.io/s/BkB03arJz))