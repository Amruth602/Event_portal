# Event Registration Portal

Advanced event registration portal for universities using:

- HTML
- CSS
- JavaScript
- Node.js
- Express.js
- MongoDB

## Features

### Admin
- Login
- View all users
- View registrations
- Manage event status
- Approve/reject vendor locations

### Vendor
- Register/login
- Add location with address
- Create events
- View own events and locations

### User
- Register/login
- Browse events
- Register for events
- Duplicate registration prevention

## Important Rule
Duplicate email registration for same event is blocked using:

```js
registrationSchema.index({ eventId: 1, email: 1 }, { unique: true });