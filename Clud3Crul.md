Upload** file with the standard [IPFS API](https://docs.ipfs.tech/reference/kubo/rpc/#api-v0-add) and get the CID:

```cil
curl -X POST 'https://<GATEWAY_HOST>/api/v0/add?pin=true' --header 'Authorization: Bearer <YOUR_W3AUTH_TOKEN>' --form 'path=@"<FILE_PATH>"'
```

**Pin** the CID with the standard [IPFS Pinning Service API](https://ipfs.github.io/pinning-services-api-spec/#operation/addPin):

```clike
curl -X POST 'https://pin.cloud3.cc' \
--header 'Authorization: Bearer <YOUR_W3AUTH_TOKEN>' \
--data-raw '{
    "cid": "<FILE_CID>",
    "name": "<FILE_NAME>"
}'
```
