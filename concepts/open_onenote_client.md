# <a name="open-the-onenote-client"></a>OneNote クライアントを開く

ページまたはノートブックの **links** プロパティを使用して、OneNote アプリケーションで特定のぺージまたはノートブックを開きます。 

**links** プロパティは 2 つの URL を含む JSON オブジェクトです。 これらの URL は、OneNote クライアント アプリケーションまたは OneNote Online のページまたはノートブックを開きます。

```json
{ 
    "links": {
        "oneNoteClientUrl": {
            "href": "onenote:https://..."
        },
        "oneNoteWebUrl": {
            "href": "https://..."
        }
    }
}
```

- **oneNoteClientUrl** 

    - OneNote クライアントがデバイスにインストールされている場合は、そのクライアントを開きます。 この URL には、*onenote* プレフィックスが含まれています。
    - 言語固有のバージョンがデバイスにインストールされている場合は、そのバージョンを開きます。 それ以外の場合は、プラットフォームの言語の設定を使用します。

- **oneNoteWebUrl** 

    - デバイスの既定のブラウザーが OneNote Online をサポートしている場合は、OneNote Online を開きます。 
    - ブラウザーの言語設定を使用します。


OneNote API は、次の操作の HTTP 応答で **links** プロパティを返します。

- [`POST pages`](../api-reference/v1.0/api/section_post_pages.md) 要求を送信してページを作成する。

- [`POST notebooks`](../api-reference/v1.0/api/onenote_post_notebooks.md) 要求を送信してノートブックを作成する。

- [`GET pages`](../api-reference/v1.0/api/page_get.md) または [`GET pages/{id}`](../api-reference/v1.0/api/page_get.md) 要求を送信してページ メタデータを取得する。

- [`GET notebooks`](../api-reference/v1.0/api/notebook_get.md) または [`GET notebooks/{id}`](../api-reference/v1.0/api/notebook_get.md) 要求を送信してノートブック メタデータを取得する。

次の例では、応答の状態コードを確認し、JSON を解析して URL を抽出し、OneNote クライアントを開く方法を示しています。

## <a name="ios-example"></a>iOS の例

次の例では、JSON 応答から OneNote クライアントの URL を取得します。 AFNetworking ライブラリ (http://afnetworking.com/)) を使用して、2 つの URL を抽出します。 この例では、`created` は、応答値を格納するために使用される **ONSCPSStandardResponse** オブジェクトへのポインターであり、`responseObject` は解析された JSON を保持します。

```objc
    /* Import the JSON library */
    #import "AFURLRequestSerialization.h"

    - (void)connectionDidFinishLoading:(NSURLConnection *)connection {
            if(delegate) {
                  int status = [returnResponse statusCode];
                  ONSCPSStandardResponse *standardResponse = nil;
                  if (status == 201) {
                        ONSCPSCreateSuccessResponse *created = 
                              [[ONSCPSCreateSuccessResponse alloc] init];
                        created.httpStatusCode = status;
                        NSError *jsonError;
                        NSDictionary *responseObject = 
                              [NSJSONSerialization JSONObjectWithData:returnData options:0 error:&jsonError];
                        if(responseObject && !jsonError) {
                              created.oneNoteClientUrl = ((NSDictionary *)
                                    ((NSDictionary *)responseObject[@"links"])[@"oneNoteClientUrl"])[@"href"];
                              created.oneNoteWebUrl = ((NSDictionary *)
                                    ((NSDictionary *)responseObject[@"links"])[@"oneNoteWebUrl"])[@"href"];
                        }
                  standardResponse = created;
                  }
                  else {
                        ONSCPSStandardErrorResponse *error = [[ONSCPSStandardErrorResponse alloc] init];
                        error.httpStatusCode = status;
                        error.message = [[NSString alloc] initWithData:returnData 
                              encoding:NSUTF8StringEncoding];
                        standardResponse = error;
                  }
                  // Send the response back to the client.
                  if (standardResponse) {
                        [delegate exampleServiceActionDidCompleteWithResponse: standardResponse];
                  }
            }
      }
``` 

<br/>

応答から URL を解析した後は、次のコードを使用して OneNote を開くことができるようになります。 インストール済みの OneNote クライアントを開くには `oneNoteClientUrl`、OneNote Online を開くには `oneNoteWebURL` を使用します。

```objc
NSURL *url = [NSURL URLWithString:standardResponse.oneNoteWebUrl];
[[UIApplication sharedApplication] openURL:url];
```

## <a name="android-example"></a>Android の例

まず成功状態コードを確認し、次に JSON を解析します。 この例では POST 要求が送信されていることを前提としているので、`201 Created` 状態コードが確認されます。 `GET` 要求を行った場合は、代わりに `200` 状態コードを確認します。

```java
public ApiResponse getResponse() throws Exception {
    /* Get the HTTP response code and message from the connection object */
    int responseCode = mUrlConnection.getResponseCode();
    String responseMessage = mUrlConnection.getResponseMessage();
    String responseBody = null;

    /* Get the response if the new page was created successfully. */
    if ( responseCode == 201) {
        InputStream is = mUrlConnection.getInputStream();

        /* Verify that this byte array is big enough. */
        byte[] b1 = new byte[1024];
        StringBuffer buffer = new StringBuffer();

        /* Copy the body of the response into the new string. */
        /* Make sure the buffer is big enough. */
        while ( is.read(b1) != -1)
            buffer.append(new String(b1));

      /* When the returned data is complete, close the connection 
         and convert the byte array into a string. */
        mUrlConnection.disconnect();
        responseBody =  buffer.toString();
    }

    /* Create a new JSON object, and an object to hold the response URLs. */
    JSONObject responseObject = null;
    ApiResponse response = new ApiResponse();
    try {

        /* Store and verify the HTTP response code. */
        response.setResponseCode(responseCode);
        response.setResponseMessage(responseMessage);
        if ( responseCode == 201) {

            /* Retrieve the two URLs from the links property. */
            responseObject = new JSONObject(responseBody);
            String clientUrl = responseObject.getJSONObject(
                "links").getJSONObject("oneNoteClientUrl").getString("href");
            String webUrl = responseObject.getJSONObject(
                "links").getJSONObject("oneNoteWebUrl").getString("href");
            response.setOneNoteClientUrl(clientUrl);
            response.setOneNoteWebUrl(webUrl);
        }
    } catch (JSONException ex) {

        /* If the JSON was malformed or incomplete... */
        String msg = ex.getMessage();
        msg = msg;
    }
    return response;
}
```

<br/>

次の例に示すように、応答プロパティを使用すると、アプリで OneNote Online を開くことができます。

```java 
if (response.getResponseCode() == 201) {
    Uri uriUrl = Uri.parse(response.getOneNoteWebUrl);  
    Intent launchBrowser = new Intent(Intent.ACTION_VIEW, uriUrl); 
    startActivity(launchBrowser);
}
```

<br/>

または、アプリで Android デバイスの OneNote クライアントを開くことができます。 `oneNoteClientUrl` プロパティを使用するときには、Intent を開始する前に、中かっこ `{ }` で GUID 文字列を囲む必要があります。 次の例に方法を示します。

```java 
if (response.getResponseCode() == 201) {

    // Get the URL from the OneNote API JSON response.
    String onenoteClientUrl = obtainClientLinkFromJSONResponse();
    String androidClientUrl = 
        onenoteClientUrl.replaceAll(
            "=([0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12})&",
            "={$1}&");

    // Open the URL: Open the newly created OneNote page.
    Uri uriUrl = Uri.parse(androidClientUrl);  
    Intent launchBrowser = new Intent(Intent.ACTION_VIEW, uriUrl); 
    startActivity(launchBrowser);
}
```

## <a name="see-also"></a>関連項目

- [OneNote コンテンツと構造を取得する](onenote-get-content.md)
- [OneNote ページを作成する](onenote-create-page.md)