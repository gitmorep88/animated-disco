# animated-discohttp://track.coldnightstudio.com/campaigns/fh2897g0tlabd/track-url/pw322k467rff3/37bfd8d50da3d51d6d417716b335f652ee771818YOUR_API_KEY_HERE
FILE_PATH=CSV_FILE_PATH
curl -X POST -H 'Content-Type: application/json' -H "Authorization: Bearer $API_KEY" -d'{
  "data": {
    "type": "importer",
    "attributes": {
      "file": { "data": "'"$(base64 $FILE_PATH)"'", "filename": "$FILE_PATH" }
    }
  }
}' https://withpersona.com/api/v1API_KEY=YOUR_API_KEY_HERE
LIST_ID=YOUR_LIST_ID_HERE
FILE_PATH=CSV_FILE_PATH

curl -X POST -H 'Content-Type: application/json' -H "Authorization: Bearer $API_KEY" -d'{
  "data": {
    "type": "importer",
    "attributes": {
      "list-id": "'"${LIST_ID}"'",
      "file": { "data": "'"$(base64 $FILE_PATH)"'", "filename": "$FILE_PATH" }
    }
  }
}' https://withpersona.com/api/v1/importer/API_KEY=YOUR_API_KEY_HERE
FILE_PATH=CSV_FILE_PATH
curl -X POST -H 'Content-Type: application/json' -H "Authorization: Bearer $API_KEY" -d'{
  "data": {
    "type": "importer",
    "attributes": {
      "file": { "data": "'"$(base64 $FILE_PATH)"'", "filename": "$FILE_PATH" }
    }
  }
}' https://withpersona.com/api/v1/importer/accountsinquiry.created	Initial status.
pending	inquiry.started	Your customer submits a document or begins a verification.
completed / failed	inquiry.completed
