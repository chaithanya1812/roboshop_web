FROM mongo

LABEL projectName=roboShop \
      env=dev
      
COPY catalouge_schema.js /docker-entrypoint-initdb.d/catalouge_schema.js
COPY user_schema.js  /docker-entrypoint-initdb.d/user.js
