import * as sdk from "appwrite";

// Init SDK
let client = new sdk.Client();

let storage = new sdk.Storage(client);

client
    .setProject('5df5acd0d48c2') // Your project ID
;

let promise = storage.getFileView('[FILE_ID]');

promise.then(function (response) {
    console.log(response);
}, function (error) {
    console.log(error);
});