# THRIFT_STORE_PROJECT
A Flask-based thrift store platform with role-based access (admin, buyer, donor). Features include product management (add, edit, delete), shopping cart with session tracking, dynamic admin dashboard, contact form with email integration, and MySQL database support. Lightweight, extendable, and easy to use.


Thrift Store Web Application

Overview
This project is a **Thrift Store Web Application** developed using **Flask**. It serves as an online platform for buying, selling, and managing thrift products. The app supports **role-based access** (admin, buyer, donor), product management, shopping cart functionality, contact form handling, and session management. It uses **MySQL** as the backend database and offers smooth user experience through dynamic routing and page rendering with Flask. 

Admins can manage product inventory, while buyers can browse products, add them to their carts, and place orders. The project is lightweight, easy to deploy, and extendable for future enhancements.

---

Features
- **Role-based Authentication:** Admins, buyers, and donors with login/logout functionality using **Flask-Login**.
- **Admin Dashboard:** Manage products (add, edit, delete) through the admin interface.
- **Shopping Cart:** Users can add products to the cart, update quantities, and view total price.
- **Product Management:** Each product has dedicated details with support for image uploads.
- **Contact Form with Email Notifications:** Messages are saved in the database and emailed to the admin using **Flask-Mail**.
- **Session Management:** Cart contents and user states are maintained through sessions.
- **Dynamic Pages:** Product pages are rendered based on their slug, enhancing SEO and user experience.

---

Technologies Used
- **Backend:** Flask, Flask-SQLAlchemy, Flask-Login, Flask-Mail  
- **Database:** MySQL  
- **Frontend:** Jinja2 templates, HTML, CSS  
- **Session Management:** Flask session  
- **Email Integration:** Flask-Mail with Gmail SMTP  

---

Requirements
Below is the list of the required modules and their versions used in the project. To install them, run:

```bash
pip install -r requirements.txt
```

### **`requirements.txt`**
```
blinker==1.8.2
click==8.1.7
colorama==0.4.6
Flask==3.0.3
Flask-Login==0.6.3
Flask-MySQL==1.5.2
Flask-SQLAlchemy==3.1.1
greenlet==3.1.1
itsdangerous==2.2.0
Jinja2==3.1.4
MarkupSafe==3.0.2
mysql-connector-python==9.1.0
PyMySQL==1.1.1
SQLAlchemy==2.0.36
typing_extensions==4.12.2
Werkzeug==3.0.4
```

---

## **Setup and Installation**
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/thrift-store.git
   cd thrift-store
   ```

2. Create and activate a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up the **MySQL database**:
   - Create a new MySQL database named `thrift_store`.
   - Update the database configuration in the `config.json` file.

5. Run the Flask application:
   ```bash
   python main.py
   ```

6. Open the browser and go to `http://127.0.0.1:5000/` to access the application.

---

Project Structure
```
THRIFT_STORE/
│
├── static/               # CSS, JS, and images
├── templates/            # HTML templates
├── config/               # Configuration files (e.g., config.json)
├── main.py               # Main Flask application file
├── requirements.txt      # Project dependencies
├── README.md             # Project description
```

---

Usage
1. **Login as Admin:**  
   Use the credentials specified in `config.json` to log in as admin and manage the store's products.
2. **Browse Products:**  
   Users can view all products listed in the store.
3. **Add to Cart:**  
   Users can add products to their cart and proceed to checkout.
4. **Contact Admin:**  
   Users can submit inquiries via the contact form.

---

Contributing
Feel free to fork this repository and submit pull requests. Any contributions to improve the project are welcome.

---

License
This project is licensed under the MIT License. See the `LICENSE` file for more details.

---

Acknowledgements
- **Flask**: Lightweight and flexible web framework
- **MySQL**: Relational database management system  
- **Flask-Mail**: Easy email integration for Flask  
- **SQLAlchemy**: ORM for smooth database interaction

---
