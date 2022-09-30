1. Install typescript: npm i -g typescript
2. Generate the tsconfig.json file using tsc --init
3. Configure the tscconfig.json file and create a src directory to store all the .ts files
4. Command to compile the .ts file is tsc


1. npm init
2. Install express: npm i --save express
3. Need to install Typescript as well Express types to take advantage of typescript: npm i --save-dev typescript @types/express
4. Executing typescript file in node using ts-node which we need to install npm i --save-dev ts-node
5. Run the .ts file using the following command npx ts-node src/index.ts
6. If we want to avoid running the above command we can also configure the package.json file to include the "start" keyword and then running the following command will be sufficient npm run start
7. Then we need to make the tsconfig.json file so that it checks the types otherwise it will be a .js kind of environment only
8. Create the endpoints in routes.ts. But we cannot use this unless we import them in index.ts which is the application server


9. To create a table use dynamodb.ts : npx ts-node src/api/dynamodb.ts
10. Load the data from .json file into the table
    - Run npm install @aws-sdk/client-dynamodb
    - Run npm install @aws-sdk/util-dynamodb
    - Run npx ts-node src/api/loadData.ts


TO RUN :npm run start:watch
11. View the contents of your aws dynamodb scan --table-name CustomerLeads4 --endpoint-url http://localhost:8000


java -Djava.library.path=./DynamoDBLocal_lib -jar DynamoDBLocal.jar -sharedDb