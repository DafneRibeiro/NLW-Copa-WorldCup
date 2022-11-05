# Daily Log 


## 05/11/2022

Started setting up my backend
Installed typescript as a Dev dependency ```npm i typescript -D``` and ```npx tsc --init```. 
And changed the target in the file tsconfig to `es2020` 

Installed Fastify `npm i fastify`
Installed tsx `npm i tsx -D` to help me compiling and executing straight away so I don't need to do it manually. 
I also add a dev in script in my file .json ` "dev": "tsx src/server.ts"` so when I run the command `npm run dev` my server starts. 
Also add watch to the dev script so my server updates itself when I change something.

Set up the first route for /pools/count


Started setting up Prisma to start the requests for the Database.

Installed Prisma `npm i prisma -D` and Prisma client `npm i @prisma/client` to connect DB with my application.
Executed with the flag `npx prisma init --datasource-provider SQlite` to use SQlite other wise it will use what Prisma uses as Default.

Created a Model for my Pool with id, title, code and createdAt and used  `npx prisma migrate dev` to create a statement SQL 

Opened prisma Studio and created a Pool in my Database so I could use it.
And doing that I was able to do a async function to access this data, and get the counts.

### Diagram ERD

Installed `npm i prisma-erd-generator @mermaid-js/mermaid-cli -D` mermaid is used to generate diagram through codes.
In my schema.prisma I created a generator:

generator erd {
  provider = "prisma-erd-generator"
}

and used `npx prisma generate` and this created a ERD.svg file for my diagram.

To finish setting up my Backend, I installed the library `npm i @fastify/cors` and set up on my server.ts

Updated Readme.