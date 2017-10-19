# <a name="open-the-onenote-client"></a><span data-ttu-id="9a89e-101">OneNote クライアントを開く</span><span class="sxs-lookup"><span data-stu-id="9a89e-101">Open the OneNote clients</span></span>

<span data-ttu-id="9a89e-102">ページまたはノートブックの **links** プロパティを使用して、OneNote アプリケーションで特定のぺージまたはノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="9a89e-102">You can use the **links** property of a page or notebook to open OneNote to the particular page or notebook.</span></span> 

<span data-ttu-id="9a89e-103">**links** プロパティは 2 つの URL を含む JSON オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="9a89e-103">The **links** property is a JSON object that contains two URLs:</span></span> <span data-ttu-id="9a89e-104">これらの URL は、OneNote クライアント アプリケーションまたは OneNote Online のページまたはノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="9a89e-104">The URLs will open the page or notebook in the native OneNote client application or in OneNote Online.</span></span>

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

- <span data-ttu-id="9a89e-105">**oneNoteClientUrl** - デバイスに既にインストールされている場合は、OneNote クライアントを開きます。</span><span class="sxs-lookup"><span data-stu-id="9a89e-105">Opens the native client if it is already installed on the device.</span></span> <span data-ttu-id="9a89e-106">この URL には、*onenote* プレフィックスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9a89e-106">This URL includes the *onenote* prefix.</span></span>
<span data-ttu-id="9a89e-107">言語固有のバージョンがデバイスにインストールされている場合は、そのバージョンを開きます。</span><span class="sxs-lookup"><span data-stu-id="9a89e-107">Opens the language-specific version if one is installed on the device.</span></span> <span data-ttu-id="9a89e-108">それ以外の場合は、プラットフォームの言語設定を使用します。</span><span class="sxs-lookup"><span data-stu-id="9a89e-108">Otherwise, uses the platform language setting.</span></span>
- <span data-ttu-id="9a89e-109">**oneNoteWebUrl** - デバイスの既定のブラウザーが OneNote Online をサポートしている場合は、OneNote Online を開きます。</span><span class="sxs-lookup"><span data-stu-id="9a89e-109">Opens OneNote Online if the default browser on the device supports OneNote Online.</span></span> <span data-ttu-id="9a89e-110">ブラウザーの言語設定を使用します。</span><span class="sxs-lookup"><span data-stu-id="9a89e-110">Uses the browser language setting.</span></span>


<span data-ttu-id="9a89e-111">OneNote API は、次の操作の HTTP 応答で **links** プロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="9a89e-111">The OneNote API returns the **links** property in the HTTP response for the following operations:</span></span>

- <span data-ttu-id="9a89e-112">[`POST pages`](../api-reference/v1.0/api/section_post_pages.md) 要求を送信してページを作成する</span><span class="sxs-lookup"><span data-stu-id="9a89e-112">Create a page by sending a [`POST pages`](../api-reference/v1.0/api/section_post_pages.md) request</span></span>
- <span data-ttu-id="9a89e-113">[`POST notebooks`](../api-reference/v1.0/api/onenote_post_notebooks.md) 要求を送信してノートブックを作成する</span><span class="sxs-lookup"><span data-stu-id="9a89e-113">Create a notebook by sending a  request</span></span>
- <span data-ttu-id="9a89e-114">[`GET pages`](../api-reference/v1.0/api/page_get.md) または [`GET pages/{id}`](../api-reference/v1.0/api/page_get.md) 要求を送信してページ メタデータを取得する</span><span class="sxs-lookup"><span data-stu-id="9a89e-114">Get page metadata by sending a [`GET pages`](../api-reference/v1.0/api/page_get.md) or [`GET pages/{id}`](../api-reference/v1.0/api/page_get.md) request</span></span>
- <span data-ttu-id="9a89e-115">[`GET notebooks`](../api-reference/v1.0/api/notebook_get.md) または [`GET notebooks/{id}`](../api-reference/v1.0/api/notebook_get.md) 要求を送信してノートブック メタデータを取得する</span><span class="sxs-lookup"><span data-stu-id="9a89e-115">Get notebook metadata by sending a [`GET notebooks`](../api-reference/v1.0/api/notebook_get.md) or [`GET notebooks/{id}`](../api-reference/v1.0/api/notebook_get.md) request</span></span>

<span data-ttu-id="9a89e-116">次の例では、応答の状態コードを確認し、JSON を解析して URL を抽出し、OneNote クライアントを開く方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="9a89e-116">The following examples show how to check the status code of the response, parse the JSON to extract the URLs, and then open the client.</span></span>

## <a name="ios-example"></a><span data-ttu-id="9a89e-117">iOS の例</span><span class="sxs-lookup"><span data-stu-id="9a89e-117">iOS example</span></span>

<span data-ttu-id="9a89e-118">次の例では、JSON 応答から OneNote クライアントの URL を取得します。</span><span class="sxs-lookup"><span data-stu-id="9a89e-118">The following example gets the OneNote client URLs from the JSON response.</span></span> <span data-ttu-id="9a89e-119">AFNetworking ライブラリ (http://afnetworking.com/) を使用して 2 つの URL を抽出します。</span><span class="sxs-lookup"><span data-stu-id="9a89e-119">It uses the AFNetworking library (http://afnetworking.com/) to extract the two URLs.</span></span> <span data-ttu-id="9a89e-120">この例では、`created` は、応答値を格納するために使用される ONSCPSStandardResponse オブジェクトへのポインターであり、`responseObject` は解析された JSON を保持します。</span><span class="sxs-lookup"><span data-stu-id="9a89e-120">The following example gets the OneNote client URLs from the JSON response. It uses the AFNetworking library (http://afnetworking.com/) to extract the two URLs. In the example, created`created` is a pointer to the ONSCPSStandardResponse object used to store the response values, and responseObject`responseObject` holds the parsed JSON.</span></span>

```objectivec
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

<span data-ttu-id="9a89e-121">応答から URL を解析した後は、次のコードを使用して OneNote を開くことができるようになります。</span><span class="sxs-lookup"><span data-stu-id="9a89e-121">After you parse the URLs from the response, you can open OneNote by using the following code.</span></span> <span data-ttu-id="9a89e-122">インストール済みの OneNote クライアントを開くには `oneNoteClientUrl`、OneNote Online を開くには `oneNoteWebURL` を使用します。</span><span class="sxs-lookup"><span data-stu-id="9a89e-122">Use `oneNoteClientUrl` to open the installed OneNote client or `oneNoteWebURL` to open OneNote Online.</span></span>

```objectivec
NSURL *url = [NSURL URLWithString:standardResponse.oneNoteWebUrl];
[[UIApplication sharedApplication] openURL:url];
```

## <a name="android-example"></a><span data-ttu-id="9a89e-123">Android の例</span><span class="sxs-lookup"><span data-stu-id="9a89e-123">Android example</span></span>

<span data-ttu-id="9a89e-124">まず成功状態コードを確認し、次に JSON を解析します。</span><span class="sxs-lookup"><span data-stu-id="9a89e-124">First, check for the success status code and then parse the JSON.</span></span> <span data-ttu-id="9a89e-125">この例では POST 要求が送信されていることを前提としているので、`201 Created` 状態コードが確認されます。</span><span class="sxs-lookup"><span data-stu-id="9a89e-125">The example assumes a POST request was sent, so it checks for a `201 Created` status code.</span></span> <span data-ttu-id="9a89e-126">`GET` 要求を行った場合は、代わりに `200` 状態コードを確認します。</span><span class="sxs-lookup"><span data-stu-id="9a89e-126">If you made a `GET` request, check for a `200` status code instead.</span></span>

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

<span data-ttu-id="9a89e-127">次の例に示すように、応答プロパティを使用すると、アプリで OneNote Online を開くことができます。</span><span class="sxs-lookup"><span data-stu-id="9a89e-127">Using the response properties, your app can open OneNote Online, as shown in the following example.</span></span>

```java 
if (response.getResponseCode() == 201) {
    Uri uriUrl = Uri.parse(response.getOneNoteWebUrl);  
    Intent launchBrowser = new Intent(Intent.ACTION_VIEW, uriUrl); 
    startActivity(launchBrowser);
}
```
 
<span data-ttu-id="9a89e-128">または、アプリで Android デバイスの OneNote クライアントを開くことができます。</span><span class="sxs-lookup"><span data-stu-id="9a89e-128">Or your app can open the native OneNote client on an Android device.</span></span> <span data-ttu-id="9a89e-129">`oneNoteClientUrl` プロパティを使用するときには、Intent を開始する前に、中かっこ `{ }` で GUID 文字列を囲む必要があります。</span><span class="sxs-lookup"><span data-stu-id="9a89e-129">When using the oneNoteClientUrl`oneNoteClientUrl` property, you must surround the GUID strings with braces `{ }` before starting the Intent.</span></span> <span data-ttu-id="9a89e-130">次の例に方法を示します。</span><span class="sxs-lookup"><span data-stu-id="9a89e-130">The following example shows how to do that.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="9a89e-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="9a89e-131">See also</span></span>

- [<span data-ttu-id="9a89e-132">OneNote コンテンツと構造を取得する</span><span class="sxs-lookup"><span data-stu-id="9a89e-132">Get Onenote content and structure</span></span>](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-get-content)
- [<span data-ttu-id="9a89e-133">OneNote ページの作成</span><span class="sxs-lookup"><span data-stu-id="9a89e-133">Create OneNote pages</span></span>](../api-reference/v1.0/api/section_post_pages.md)