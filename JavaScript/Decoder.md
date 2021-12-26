# Decoder
A Text[Decoder].prototype.decode() is a method that returns a [[DOMString]] after processing a stream.

####### [Parameters](https://developer.mozilla.org/en-US/docs/Web/API/TextDecoder/decode#parameters "Permalink to Parameters")

`buffer` (optional)

Is either an [ArrayBuffer] or an [ArrayBufferView] containing the text to decode. We get this reading from the lichess API and reading from the stream from the response.

`options` (optional)

Is a [TextDecodeOptions] dictionary with the property:

`stream`

A boolean flag indicating that additional data will follow in subsequent calls to decode(). Set to true if processing the data in chunks, and false for the final chunk or if the data is not chunked. It defaults to false.
