# Flask CRUD API

This is a simple Flask-based CRUD (Create, Read, Update, Delete) API for managing stores and their items, including item prices.

## Features
- Add new stores
- Update store details
- Add items to a store
- Update item prices
- Retrieve store and item details
- Delete stores and items

## Installation

Make sure you have Python installed. Then, install Flask using pip:

```bash
pip install flask
```

## Running the Application

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/flask-crud-api.git
   cd flask-crud-api
   ```

2. Run the Flask application:
   ```bash
   flask run
   ```

   By default, the API will be available at: `http://127.0.0.1:5000/`

## API Endpoints

### Stores

- **Get all stores**: `GET /stores`
- **Get a specific store**: `GET /stores/<store_id>`
- **Create a store**: `POST /stores`
  ```json
  {
    "name": "Store Name"
  }
  ```
- **Update a store**: `PUT /stores/<store_id>`
  ```json
  {
    "name": "Updated Store Name"
  }
  ```
- **Delete a store**: `DELETE /stores/<store_id>`

### Items

- **Get all items in a store**: `GET /stores/<store_id>/items`
- **Add an item to a store**: `POST /stores/<store_id>/items`
  ```json
  {
    "name": "Item Name",
    "price": 10.99
  }
  ```
- **Update an item price**: `PUT /stores/<store_id>/items/<item_id>`
  ```json
  {
    "price": 12.99
  }
  ```
- **Delete an item**: `DELETE /stores/<store_id>/items/<item_id>`

## Contributing
Feel free to fork the repository and submit pull requests.

## License
This project is licensed under the MIT License.

