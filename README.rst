Flaskr
======

Ứng dụng blog cơ bản được tích hợp trong Flask `tutorial`_.

.. _tutorial: https://flask.palletsprojects.com/tutorial/


Install
---- 
::

    # clone the repository
    $ git clone https://github.com/MaiThuyNguyen369/FLASK_PROJECT.git
    $ cd FLASK_PROJECT

Tạo môi trường và kích hoạt nó: ::

    $ python3 -m venv .venv
    $ . .venv/bin/activate

Hoặc với Windows cmd:::

    $ py -3 -m venv .venv
    $ .venv\Scripts\activate.bat

Cài đặt Flaskr::

    $ pip install -e .

Hoặc nếu đang sử dụng nhánh main, hãy cài đặt Flask từ nguồn trước khi cài đặt Flaskr:
::
    $ pip install -e ../..
    $ pip install -e .


Run
---

.. code-block:: text

    $ flask --app flaskr init-db
    $ flask --app flaskr run --debugger

Mở http://127.0.0.1:5000 trong trình duyệt.


Test
----

::

    $ pip install '.[test]'
    $ pytest

Run with coverage report::

    $ coverage run -m pytest
    $ coverage report
    $ coverage html  # Mở htmlcov/index.html trong trình duyệt
