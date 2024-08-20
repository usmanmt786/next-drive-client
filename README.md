<img src="https://github.com/user-attachments/assets/cf92e206-0cee-4f38-abfd-959c27ac3232"
height="100px"
/>

# NEXT DRIVE CLIENT

Upload and other utility functions for Clients using `NEXT DRIVE` as file server.



## Install
```
npm install nextdrive-client
```

## Usage
```ts
import {NextDriveUploader} from 'nextdrive-client';

const uploader = new NextDriveUploader({
    rootUrl:"http://localhost:4000",
    apiKey: process.ev.API_KEY,
});

```
### Upload Files
```ts
const response = await uploader.upload({
    folder: "products",
    files: [File]
});
```


### Delete Files
```ts
const response = await uploader.delete({
    folder: "products",
    files: [string]
});

```