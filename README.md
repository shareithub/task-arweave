# AFTER COMPLETE TASK , SAVE THE SCREENSHOOT & UPLOAD IN YOUR FOLDER

# TASK U CAN JOIN HERE : https://openbuild.xyz/u/ArweaveOasis

# ***QUIZ 1***

# Where does Arweave store files?

The transaction object can contain files smaller than 12MiB

Files bigger than 12MiB have a separate storage location


# How does Arweave's consensus algorithm ensure permanent storage?

By incentivizing miner nodes to share data

By requiring miner nodes to prove access to random chunks of uploaded data


# What data can you store on Arweave?

Single page applications

Image and text

Music and Videos

# What features does Arweave have?

Global replication

Censorship resistance

# What is Arweave?

Immutable object storage

Like Bitcoin for storage

A layer1 network


# What responsibilities do miner nodes have?

Data replication

Data storage

# ***QUIZ 2***


# What are Arweave’s pros compared to popular blockchain networks?

The protocol handles storage and replication

Cheap permanent storage

# What are Arweave's pros compared to cloud storage?

Strong provenance guarantees

One-time payment


# What are the properties of bundled transactions?

They can have custom tags

They can be paid with fiat currency

They are relatively fast

# What are the properties of L1 transactions?

They can have custom tags

They can transfer AR tokens

They are relatively slow

# What are the Arweave transaction types?

Bundled transactions

L1 transactions


# How does Arweave ensure continuous payment for its storage?

Its token economics are based on future storage cost estimates

It has a storage endowment to save tokens for later

# How can you remove data from Arweave?

You can’t enforce removal

By sending a do-not-store request

# What are parts of the SPoRA consensus algorithm?

Proving access to random chunks of uploaded data

Computing a hash



# ***QUIZ 3***


# Which Arweave wallets are well suited for DApp frontends?

Arweave.app

ArConnect

# Can you use Ledger as a cold wallet for Arweave?

Yes, there is a plugin for AR.


# How do bundling services improve Arweave?

They enable non-Arweave signatures

They enable non-AR token payments

They enable fiat payments

# Can you use the same wallet address on the frontend and backend?

Yes, you can import the key file exported from your backend in your wallet app

Yes, you can export a key file from a wallet app and load it in the backend



# Why do you need a reusable wallet address to upload big files?

To mark your uploads with your personal signature, to proof you uploaded it first

To charge the wallet with tokens for the upload payments


# How do you pay for a bundled transaction?

Depends on the bundling service


# When would you upload a file via a bundled transaction?

You require high TPS

You’re file is under 100 KiB, so it’s a free upload


# Can you upload files directly from the browser?

Yes, you can use JavaScript SDKs in the browser and Node.js

# How do you store small files on Arweave?

You don’t need any tokens to upload files under 100KiB

You upload them via a bundling service




# ***QUIZ 4***


# How do you access the plain manifest JSON?

With the /raw endpoint of a gateway node


# What properties does a path manifest support?

An index key that resolves the empty path

A list of keys that point to transaction IDs

A wildcard key that resolves missing paths


# How do gateways simulate directory structures?

With JSON path manifests.

# Why do gateways isolate transactions with subdomains?

To prevent browser data access between transactions

# What’s the primary difference between Bitcoin and Arweave transactions?

Arweave transactions can contain links to files of arbitrary size.


# What information do you need to access a file on Arweave?

The hostname of a gateway

A transaction ID




# ***QUIZ 5***

# Which properties are part of Arweave transactions?

last_tx

data_root

signature

tags

# How does Arweave incentivize gateway nodes?

The money from ArNS name sales is used to pay gateway operators.


# Are ArNS names mutable?

Yes, ArNS names let you change their target transaction ID


# Does Arweave support naming transactions?

Yes, with ArNS.



# Where can you store files on Arweave?

Outside the transaction, if it’s smaller than 12MiB

Outside the transaction, if it’s bigger than 12MiB

Inside the transaction, if it’s smaller than 12MiB


# How do you search transactions on Arweave?

With the GraphQL endpoint of the gateway nodes.




# ***QUIZ 6***


# How can using relative URLs in your website lead to permanent links?

While the URLs are relative to the TXID they belong to, this ID never changes.



# How do you use the rel filter in a Eleventy template?

{{ post.url | rel }}

# Does Eleventy need any special configuration to work with Arweave?

Yes, it needs a filter to rewrite relative URLs, so they work with the TXID Arweave websites start with.


# Why is a static website generator the perfect tool to create websites for Arweave?

Arweave gateways can’t render HTML and build-time rendering solves this issue.


# Does Arweave treat websites different from other data?

Yes, if you add the correct tags, gateways will deliver the data as website to a browser.


# What is the goal of Arweave?

To provide the world with permanent, immutable storage.


# ***QUIZ 7***


# Where can you find the immutable TXID of an ArNS page?

In the X-Arns-Resolved-Id header field.

# Are ArNS names linked to a gateway?

No, you can access every ArNS name from every gateway.


# Are ArNS names immutable?

No, you can change their target TXIDs.

# What enables users to access multiple files with one TXID?

A JSON path manifest that maps paths to TXIDs.



# How does Arweave change the content of a TXID after you uploaded a new version of a file?

It doesn’t, the new upload will get a new TXID.


# Why can you deploy a website with a randomly generated wallet?

Arweave bundling services subsidize uploads under 100 KiB.



# ***QUIZ 8***



# Why do you need custom tags?

To tell the gateways what type of file is in the transaction body.

To improve the discoverability of your uploaded files.



# Why is the storage utility split into two files?

For efficiency, because the writing functionality requires many libraries and readers don’t need them.


# Where in this project do you write data to Arweave?

In the browser, when creating and updating articles.

In Node.js, to deploy the DApp.



# What can SPAs do that static websites can’t?

Enable complex user interactions.

Include data that isn’t available at build time.


# Why are SPAs a good fit for Arweave?

Clint-side rendering scales better as server don’t have to execute any logic.

As gateways only deliver static files, code must run on the client.


# What are the properties of SPAs?

They execute and rener inside the browser.

They are platform independent.

You can use them without installation.





# ***QUIZ 9***



# Why should you define your bundle chunks manually?

It reduces storage costs by using chunks that are already on Arweave.

Chunk uploads under 100 KiB are free.

# Why should you test your DApp with a regular web server before uploading it to Arweave?

Web servers behave more similarly to Arweave gateways than dev servers, which include hot reloading and other features.


# Why should you lazy-load some routes of your DApp?

Because not all functionality is used by all users.

# How do you retrieve the article content?

With the TXID and the gateway’s data endpoint.


# Can you filter GraphQL queries by the content of the transaction body?

No because transaction bodies can have an arbitrary size and format.

# How does your blog update articles if data on Arweave is immutable?

It creates a transaction with a new article version and only displays the latest versions.


# ***QUIZ 10***


# Under which URL scheme is your DApp available after you point an ArNS name to its TXID?

https://<ARNS_NAME>.<GATEWAY_HOSTNAME>/



# What’s the undername of the root record of an ArNS name?

@



# Why do you need the ANT process ID to update your ArNS name?

The ANT process controls the ArNS name.




# Why do you have to set a base in the Vite configuration?

To ensure Vite generates relative URLs.



# How does the deployment script detect changed files?

The script can diff the current file names with the ones in the path manifest of the previous deployment.

The file names contain hashes that change when their content changes.


# Why do you need Turbo Credits?

To upload files to Arweave that are bigger than 100 KiB.

