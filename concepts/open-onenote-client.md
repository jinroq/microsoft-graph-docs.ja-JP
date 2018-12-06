---
title: OneNote クライアントを開く
description: 'ページまたはノートブックの **links** プロパティを使用して、OneNote アプリケーションで特定のぺージまたはノートブックを開きます。 '
ms.openlocfilehash: c82507243488777e557b18e599edb86b2ac15622
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092472"
---
# <a name="open-the-onenote-client"></a><span data-ttu-id="045de-103">OneNote クライアントを開く</span><span class="sxs-lookup"><span data-stu-id="045de-103">Open the OneNote client</span></span>

<span data-ttu-id="045de-104">ページまたはノートブックの **links** プロパティを使用して、OneNote アプリケーションで特定のぺージまたはノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="045de-104">You can use the **links** property of a page or notebook to open a OneNote application to a particular page or notebook.</span></span> 

<span data-ttu-id="045de-105">**links** プロパティは 2 つの URL を含む JSON オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="045de-105">The **links** property is a JSON object that contains two URLs.</span></span> <span data-ttu-id="045de-106">これらの URL は、OneNote クライアント アプリケーションまたは OneNote Online のページまたはノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="045de-106">The URLs will open the page or notebook in the OneNote client application or in OneNote Online.</span></span>

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

- <span data-ttu-id="045de-107">**oneNoteClientUrl**</span><span class="sxs-lookup"><span data-stu-id="045de-107">**oneNoteClientUrl**</span></span> 

    - <span data-ttu-id="045de-108">OneNote クライアントがデバイスにインストールされている場合は、そのクライアントを開きます。</span><span class="sxs-lookup"><span data-stu-id="045de-108">Opens the OneNote client if it is already installed on the device.</span></span> <span data-ttu-id="045de-109">この URL には、*onenote* プレフィックスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="045de-109">This URL includes the *onenote* prefix.</span></span>
    - <span data-ttu-id="045de-110">言語固有のバージョンがデバイスにインストールされている場合は、そのバージョンを開きます。</span><span class="sxs-lookup"><span data-stu-id="045de-110">Opens the language-specific version if one is installed on the device.</span></span> <span data-ttu-id="045de-111">それ以外の場合は、プラットフォームの言語の設定を使用します。</span><span class="sxs-lookup"><span data-stu-id="045de-111">Otherwise, uses the platform language setting.</span></span>

- <span data-ttu-id="045de-112">**oneNoteWebUrl**</span><span class="sxs-lookup"><span data-stu-id="045de-112">**oneNoteWebUrl**</span></span> 

    - <span data-ttu-id="045de-113">デバイスの既定のブラウザーが OneNote Online をサポートしている場合は、OneNote Online を開きます。</span><span class="sxs-lookup"><span data-stu-id="045de-113">Opens OneNote Online if the default browser on the device supports it.</span></span> 
    - <span data-ttu-id="045de-114">ブラウザーの言語設定を使用します。</span><span class="sxs-lookup"><span data-stu-id="045de-114">Uses the browser language setting.</span></span>


<span data-ttu-id="045de-115">OneNote API は、次の操作の HTTP 応答で **links** プロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="045de-115">The OneNote API returns the **links** property in the HTTP response for the following operations:</span></span>

- <span data-ttu-id="045de-116">[`POST pages`](/graph/api/section-post-pages?view=graph-rest-1.0) 要求を送信してページを作成する。</span><span class="sxs-lookup"><span data-stu-id="045de-116">Create a page by sending a [`POST pages`](/graph/api/section-post-pages?view=graph-rest-1.0) request.</span></span>

- <span data-ttu-id="045de-117">[`POST notebooks`](/graph/api/onenote-post-notebooks?view=graph-rest-1.0) 要求を送信してノートブックを作成する。</span><span class="sxs-lookup"><span data-stu-id="045de-117">Create a notebook by sending a [`POST notebooks`](/graph/api/onenote-post-notebooks?view=graph-rest-1.0) request.</span></span>

- <span data-ttu-id="045de-118">[`GET pages`](/graph/api/page-get?view=graph-rest-1.0) または [`GET pages/{id}`](/graph/api/page-get?view=graph-rest-1.0) 要求を送信してページ メタデータを取得する。</span><span class="sxs-lookup"><span data-stu-id="045de-118">Get page metadata by sending a [`GET pages`](/graph/api/page-get?view=graph-rest-1.0) or [`GET pages/{id}`](/graph/api/page-get?view=graph-rest-1.0) request.</span></span>

- <span data-ttu-id="045de-119">[`GET notebooks`](/graph/api/notebook-get?view=graph-rest-1.0) または [`GET notebooks/{id}`](/graph/api/notebook-get?view=graph-rest-1.0) 要求を送信してノートブック メタデータを取得する。</span><span class="sxs-lookup"><span data-stu-id="045de-119">Get notebook metadata by sending a [`GET notebooks`](/graph/api/notebook-get?view=graph-rest-1.0) or [`GET notebooks/{id}`](/graph/api/notebook-get?view=graph-rest-1.0) request.</span></span>

<span data-ttu-id="045de-120">次の例では、応答の状態コードを確認し、JSON を解析して URL を抽出し、OneNote クライアントを開く方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="045de-120">The following examples show how to check the status code of the response, parse the JSON to extract the URLs, and then open the OneNote client.</span></span>

## <a name="ios-example"></a><span data-ttu-id="045de-121">iOS の例</span><span class="sxs-lookup"><span data-stu-id="045de-121">iOS example</span></span>

<span data-ttu-id="045de-122">次の例では、JSON 応答から OneNote クライアントの URL を取得します。</span><span class="sxs-lookup"><span data-stu-id="045de-122">The following example gets the OneNote client URLs from the JSON response.</span></span> <span data-ttu-id="045de-123">AFNetworking ライブラリ (https://afnetworking.com/)) を使用して、2 つの URL を抽出します。</span><span class="sxs-lookup"><span data-stu-id="045de-123">It uses the AFNetworking library (https://afnetworking.com/) to extract the two URLs.</span></span> <span data-ttu-id="045de-124">この例では、`created` は、応答値を格納するために使用される **ONSCPSStandardResponse** オブジェクトへのポインターであり、`responseObject` は解析された JSON を保持します。</span><span class="sxs-lookup"><span data-stu-id="045de-124">In the example, `created` is a pointer to the **ONSCPSStandardResponse** object used to store the response values, and `responseObject` holds the parsed JSON.</span></span>

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

<span data-ttu-id="045de-125">応答から URL を解析した後は、次のコードを使用して OneNote を開くことができるようになります。</span><span class="sxs-lookup"><span data-stu-id="045de-125">After you parse the URLs from the response, you can open OneNote by using the following code.</span></span> <span data-ttu-id="045de-126">インストール済みの OneNote クライアントを開くには `oneNoteClientUrl`、OneNote Online を開くには `oneNoteWebURL` を使用します。</span><span class="sxs-lookup"><span data-stu-id="045de-126">Use `oneNoteClientUrl` to open the installed OneNote client or `oneNoteWebURL` to open OneNote Online.</span></span>

```objc
NSURL *url = [NSURL URLWithString:standardResponse.oneNoteWebUrl];
[[UIApplication sharedApplication] openURL:url];
```

## <a name="android-example"></a><span data-ttu-id="045de-127">Android の例</span><span class="sxs-lookup"><span data-stu-id="045de-127">Android example</span></span>

<span data-ttu-id="045de-128">まず成功状態コードを確認し、次に JSON を解析します。</span><span class="sxs-lookup"><span data-stu-id="045de-128">First, check for the success status code, and then parse the JSON.</span></span> <span data-ttu-id="045de-129">この例では POST 要求が送信されていることを前提としているので、`201 Created` 状態コードが確認されます。</span><span class="sxs-lookup"><span data-stu-id="045de-129">The example assumes a POST request was sent, so it checks for a `201 Created` status code.</span></span> <span data-ttu-id="045de-130">`GET` 要求を行った場合は、代わりに `200` 状態コードを確認します。</span><span class="sxs-lookup"><span data-stu-id="045de-130">If you made a `GET` request, check for a `200` status code instead.</span></span>

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

<span data-ttu-id="045de-131">次の例に示すように、応答プロパティを使用すると、アプリで OneNote Online を開くことができます。</span><span class="sxs-lookup"><span data-stu-id="045de-131">Using the response properties, your app can open OneNote Online, as shown in the following example.</span></span>

```java 
if (response.getResponseCode() == 201) {
    Uri uriUrl = Uri.parse(response.getOneNoteWebUrl);  
    Intent launchBrowser = new Intent(Intent.ACTION_VIEW, uriUrl); 
    startActivity(launchBrowser);
}
```

<br/>

<span data-ttu-id="045de-132">または、アプリで Android デバイスの OneNote クライアントを開くことができます。</span><span class="sxs-lookup"><span data-stu-id="045de-132">Or your app can open the OneNote client on an Android device.</span></span> <span data-ttu-id="045de-133">`oneNoteClientUrl` プロパティを使用するときには、Intent を開始する前に、中かっこ `{ }` で GUID 文字列を囲む必要があります。</span><span class="sxs-lookup"><span data-stu-id="045de-133">When using the `oneNoteClientUrl` property, you must surround the GUID strings with braces `{ }` before starting the Intent.</span></span> <span data-ttu-id="045de-134">次の例に方法を示します。</span><span class="sxs-lookup"><span data-stu-id="045de-134">The following example shows how to do that.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="045de-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="045de-135">See also</span></span>

- [<span data-ttu-id="045de-136">OneNote コンテンツと構造を取得する</span><span class="sxs-lookup"><span data-stu-id="045de-136">Get OneNote content and structure</span></span>](onenote-get-content.md)
- [<span data-ttu-id="045de-137">OneNote ページの作成</span><span class="sxs-lookup"><span data-stu-id="045de-137">Create OneNote pages</span></span>](onenote-create-page.md)