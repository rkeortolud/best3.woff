![HandyUI](https://raw.githubusercontent.com/herokufree/HandyUI/30e2c62/docs/banner.png)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

# HandyUI

# backup-system
- The REST Server runs on port 4000
- Tested on Apple Silicon M2 and Raspberry Pi 4
- [Live demo](https://herokufree.github.io/HandyUI/)

# ChessCrypt

```bash
git clone https://github.com/herokufree/HandyUI.git
cd HandyUI
npm install
```

# todo_go

```bash
node server.js
```

or with nodemon:

```bash
npx nodemon server.js
```

Server starts on `http://localhost:4000`

# idonethis-perl

Set up `.env`:
```
MONGO_URI=mongodb://localhost:27017/handyui
PORT=4000
JWT_SECRET=your_secret_here
NODE_ENV=development
```

# sweeui-basic

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | /api/items | List all items |
| POST | /api/items | Create item |
| GET | /api/items/:id | Get item by id |
| PUT | /api/items/:id | Update item |
| DELETE | /api/items/:id | Delete item |
| GET | /api/users | List all users |
| POST | /api/users/login | Login user |
| POST | /api/users/register | Register user |

# hecto

```javascript
const mongoose = require('mongoose')

const ItemSchema = new mongoose.Schema({
  title: { type: String, required: true },
  done: { type: Boolean, default: false },
  priority: { type: Number, default: 2 },
  tags: [{ type: String }],
  createdAt: { type: Date, default: Date.now },
  updatedAt: { type: Date, default: Date.now }
})

module.exports = mongoose.model('Item', ItemSchema)
```

# twilio-python

```bash
# Install MongoDB on ARM (Ubuntu/Debian)
wget -qO - https://www.mongodb.org/static/pgp/server-6.0.asc | sudo apt-key add -
echo "deb [ arch=arm64 ] https://repo.mongodb.org/apt/ubuntu focal/mongodb-org/6.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-6.0.list
sudo apt-get update
sudo apt-get install -y mongodb-org
sudo systemctl start mongod
sudo systemctl enable mongod
```

# rate_throttle

```bash
# Verify MongoDB is running
sudo systemctl status mongod

# Connect to mongo shell
mongosh

# Create database
use handyui

# Create test document
db.items.insertOne({ title: "test", done: false, priority: 1 })
db.items.find()
```

# messagit-store

```bash
npm test
```

Coverage report in `coverage/lcov-report/index.html`.

Run specific test suite:
```bash
npm test -- --testPathPattern=items
npm test -- --coverage
```

# stuffsamdrinks

```javascript
const request = require('supertest')
const app = require('../server')

describe('GET /api/items', () => {
  it('should return 200 and array', async () => {
    const res = await request(app).get('/api/items')
    expect(res.statusCode).toBe(200)
    expect(Array.isArray(res.body)).toBe(true)
  })
})
```

# streamlit-hello

- Node.js 20+
- MongoDB 6.0+
- mongoose, express, dotenv, jsonwebtoken, bcryptjs
- jest, supertest (dev)
- nodemon (dev)

# cosign

Deploy to Railway or Render:
```bash
# Railway
railway init
railway up

# or Render — connect GitHub repo, set env vars in dashboard
```
