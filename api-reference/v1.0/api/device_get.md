# <a name="get-device"></a><span data-ttu-id="3b86a-101">デバイスを取得する</span><span class="sxs-lookup"><span data-stu-id="3b86a-101">Get device</span></span>

<span data-ttu-id="3b86a-102">デバイス オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="3b86a-102">Get the properties and relationships of a device object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3b86a-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="3b86a-103">Prerequisites</span></span>
<span data-ttu-id="3b86a-104">この API を実行するには、次のいずれかの**スコープ**が必要です。*Device.ReadWrite.All* または *Directory.Read.All* または *Directory.ReadWrite.All* または *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="3b86a-104">One of the following **scopes** is required to execute this API: *Device.ReadWrite.All* or *Directory.Read.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="3b86a-105">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3b86a-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
> <span data-ttu-id="3b86a-106">注:要求内の"id"は、"deviceId"プロパティではなく、デバイスの id プロパティです。</span><span class="sxs-lookup"><span data-stu-id="3b86a-106">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="3b86a-107">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3b86a-107">Optional query parameters</span></span>
<span data-ttu-id="3b86a-108">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3b86a-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3b86a-109">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3b86a-109">Request headers</span></span>
| <span data-ttu-id="3b86a-110">名前</span><span class="sxs-lookup"><span data-stu-id="3b86a-110">Name</span></span>       | <span data-ttu-id="3b86a-111">型</span><span class="sxs-lookup"><span data-stu-id="3b86a-111">Type</span></span> | <span data-ttu-id="3b86a-112">説明</span><span class="sxs-lookup"><span data-stu-id="3b86a-112">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3b86a-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b86a-113">Authorization</span></span>  | <span data-ttu-id="3b86a-114">string</span><span class="sxs-lookup"><span data-stu-id="3b86a-114">string</span></span>  | <span data-ttu-id="3b86a-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3b86a-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b86a-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="3b86a-117">Request body</span></span>
<span data-ttu-id="3b86a-118">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3b86a-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b86a-119">応答</span><span class="sxs-lookup"><span data-stu-id="3b86a-119">Response</span></span>

<span data-ttu-id="3b86a-120">成功した場合、このメソッドは`200 OK`応答コードと、応答本文で[デバイス](../resources/device.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3b86a-120">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3b86a-121">例</span><span class="sxs-lookup"><span data-stu-id="3b86a-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b86a-122">要求</span><span class="sxs-lookup"><span data-stu-id="3b86a-122">Request</span></span>
<span data-ttu-id="3b86a-123">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3b86a-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="3b86a-124">応答</span><span class="sxs-lookup"><span data-stu-id="3b86a-124">Response</span></span>
<span data-ttu-id="3b86a-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3b86a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "accountEnabled":false,
  "alternativeSecurityIds":
  [
    {
      "type": 2,
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
