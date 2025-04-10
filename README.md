# golang-tryout
# json.Marshal
Purpose:
Converts (or "serializes") a Go value (typically a struct or map) into a JSON-formatted byte slice.

When to Use It:

When you want to obtain a JSON string (or byte slice) that you can store, log, or further manipulate before sending it somewhere.

It's ideal when you don't need to write directly to an output stream, but instead want to capture the JSON output in a variable.

#  json.Encode and json.Decode

Purpose:

json.Encode writes JSON directly to an io.Writer.

json.Decode reads JSON from an io.Reader and decodes it into a Go value.

When to Use Them:

Encode:
When you're working with streams or output destinations like HTTP responses, files, or network connections. For example, you can write JSON directly to the HTTP response writer in a web server.

Decode:
When you receive JSON data from a stream (like an HTTP request body or a file) and want to convert it directly into a Go struct or map.