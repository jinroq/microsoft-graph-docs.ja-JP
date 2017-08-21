# <a name="list-devices"></a><span data-ttu-id="d433f-101">デバイスを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d433f-101">List devices</span></span>

<span data-ttu-id="d433f-102">組織に登録されているデバイス オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="d433f-102">Retrieve a list of device objects registered in the organization.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d433f-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="d433f-103">Prerequisites</span></span>
<span data-ttu-id="d433f-104">この API を実行するには、次のいずれかの**スコープ**が必要です。*Device.ReadWrite.All* または *Directory.Read.All* または *Directory.ReadWrite.All* または *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="d433f-104">One of the following **scopes** is required to execute this API: *Device.ReadWrite.All* or *Directory.Read.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="d433f-105">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d433f-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d433f-106">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d433f-106">Optional query parameters</span></span>
<span data-ttu-id="d433f-107">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d433f-107">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d433f-108">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d433f-108">Request headers</span></span>
| <span data-ttu-id="d433f-109">名前</span><span class="sxs-lookup"><span data-stu-id="d433f-109">Name</span></span>       | <span data-ttu-id="d433f-110">型</span><span class="sxs-lookup"><span data-stu-id="d433f-110">Type</span></span> | <span data-ttu-id="d433f-111">説明</span><span class="sxs-lookup"><span data-stu-id="d433f-111">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d433f-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="d433f-112">Authorization</span></span>  | <span data-ttu-id="d433f-113">string</span><span class="sxs-lookup"><span data-stu-id="d433f-113">string</span></span>  | <span data-ttu-id="d433f-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d433f-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d433f-116">要求本文</span><span class="sxs-lookup"><span data-stu-id="d433f-116">Request body</span></span>
<span data-ttu-id="d433f-117">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d433f-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d433f-118">応答</span><span class="sxs-lookup"><span data-stu-id="d433f-118">Response</span></span>

<span data-ttu-id="d433f-119">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [device](../resources/device.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d433f-119">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d433f-120">例</span><span class="sxs-lookup"><span data-stu-id="d433f-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d433f-121">要求</span><span class="sxs-lookup"><span data-stu-id="d433f-121">Request</span></span>
<span data-ttu-id="d433f-122">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d433f-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices
```

##### <a name="response"></a><span data-ttu-id="d433f-123">応答</span><span class="sxs-lookup"><span data-stu-id="d433f-123">Response</span></span>
<span data-ttu-id="d433f-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d433f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "accountEnabled":false,
      "alternativeSecurityIds":
      [
        {
          "type":2,
          "key":"Y3YxN2E1MWFlYw==",
          "identityProvider": null
        }
      ],
      "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
      "displayName":"Test device",
      "id": "id-value",
      "operatingSystem":"linux",
      "operatingSystemVersion":"1"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List devices",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
