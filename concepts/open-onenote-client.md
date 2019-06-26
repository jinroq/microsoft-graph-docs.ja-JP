---
title: OneNote クライアントを開く
description: 'ページまたはノートブックの **links** プロパティを使用して、OneNote アプリケーションで特定のぺージまたはノートブックを開きます。 '
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: b4ad078443bd6d85c46a6e23552ddc730c725b51
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236287"
---
# <a name="open-the-onenote-client"></a>OneNote クライアントを開く

ページまたはノートブックの **links** プロパティを使用して、OneNote アプリケーションで特定のぺージまたはノートブックを開きます。 

**links** プロパティは 2 つの URL を含む JSON オブジェクトです。 Url は、OneNote クライアントアプリケーションまたは web 上の OneNote でページまたはノートブックを開きます。

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
    - Opens the language-specific version if one is installed on the device. Otherwise, uses the platform language setting.

- **oneNoteWebUrl** 

    - デバイスの既定のブラウザーが OneNote をサポートしている場合、その web 上で OneNote を開きます。 
    - ブラウザーの言語設定を使用します。


OneNote API は、次の操作の HTTP 応答で **links** プロパティを返します。

- [`POST pages`](/graph/api/section-post-pages?view=graph-rest-1.0) 要求を送信してページを作成する。

- [`POST notebooks`](/graph/api/onenote-post-notebooks?view=graph-rest-1.0) 要求を送信してノートブックを作成する。

- [`GET pages`](/graph/api/page-get?view=graph-rest-1.0) または [`GET pages/{id}`](/graph/api/page-get?view=graph-rest-1.0) 要求を送信してページ メタデータを取得する。

- [`GET notebooks`](/graph/api/notebook-get?view=graph-rest-1.0) または [`GET notebooks/{id}`](/graph/api/notebook-get?view=graph-rest-1.0) 要求を送信してノートブック メタデータを取得する。

次の例では、応答の状態コードを確認し、JSON を解析して URL を抽出し、OneNote クライアントを開く方法を示しています。

## <a name="ios-example"></a>iOS の例

次の例では、JSON 応答から OneNote クライアントの URL を取得します。 AFNetworking ライブラリ (https://afnetworking.com/)) を使用して、2 つの URL を抽出します。 この例では、`created` は、応答値を格納するために使用される **ONSCPSStandardResponse** オブジェクトへのポインターであり、`responseObject` は解析された JSON を保持します。

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

応答から URL を解析した後は、次のコードを使用して OneNote を開くことができるようになります。 を`oneNoteClientUrl`使用して、インストールされ`oneNoteWebURL`ている onenote クライアントを開くか、web 上の onenote を開きます。

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

Response プロパティを使用すると、次の例に示すように、アプリから web 上の OneNote を開くことができます。

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
