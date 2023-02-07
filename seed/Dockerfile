FROM mongo:4.4.6

COPY users.json /users.json
COPY contacts.json /contacts.json
COPY galerias.json /galerias.json
COPY polaroids.json /polaroids.json
COPY services.json /services.json

CMD mongoimport --collection users --uri mongodb://root:example@mongodb:27017/carwash_db?authSource=admin --type json --drop --file /users.json --jsonArray && \
    mongoimport --collection contacts --uri mongodb://root:example@mongodb:27017/carwash_db?authSource=admin --type json --drop --file /contacts.json --jsonArray && \
    mongoimport --collection galerias --uri mongodb://root:example@mongodb:27017/carwash_db?authSource=admin --type json --drop --file /galerias.json --jsonArray && \
    mongoimport --collection polaroids --uri mongodb://root:example@mongodb:27017/carwash_db?authSource=admin --type json --drop --file /polaroids.json --jsonArray && \
    mongoimport --collection services --uri mongodb://root:example@mongodb:27017/carwash_db?authSource=admin --type json --drop --file /services.json --jsonArray