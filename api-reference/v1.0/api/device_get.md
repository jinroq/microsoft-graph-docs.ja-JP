# <a name="get-device"></a><span data-ttu-id="07436-101">デバイスを取得する</span><span class="sxs-lookup"><span data-stu-id="07436-101">Get device</span></span>

<span data-ttu-id="07436-102">デバイス オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="07436-102">Get the properties and relationships of a device object.</span></span>
## <a name="permissions"></a><span data-ttu-id="07436-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="07436-103">Permissions</span></span>
<span data-ttu-id="07436-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="07436-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="07436-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="07436-106">Permission type</span></span>      | <span data-ttu-id="07436-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="07436-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07436-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="07436-108">Delegated (work or school account)</span></span> | <span data-ttu-id="07436-109">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="07436-109">One of the following scopes is required to execute this API: Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="07436-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="07436-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07436-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07436-111">Not supported.</span></span>    |
|<span data-ttu-id="07436-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="07436-112">Application</span></span> | <span data-ttu-id="07436-113">Device.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07436-113">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="07436-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="07436-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
> <span data-ttu-id="07436-115">注:要求内の"id"は、"deviceId"プロパティではなく、デバイスの id プロパティです。</span><span class="sxs-lookup"><span data-stu-id="07436-115">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="07436-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="07436-116">Optional query parameters</span></span>
<span data-ttu-id="07436-117">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="07436-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="07436-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="07436-118">Request headers</span></span>
| <span data-ttu-id="07436-119">名前</span><span class="sxs-lookup"><span data-stu-id="07436-119">Name</span></span>       | <span data-ttu-id="07436-120">型</span><span class="sxs-lookup"><span data-stu-id="07436-120">Type</span></span> | <span data-ttu-id="07436-121">説明</span><span class="sxs-lookup"><span data-stu-id="07436-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="07436-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="07436-122">Authorization</span></span>  | <span data-ttu-id="07436-123">string</span><span class="sxs-lookup"><span data-stu-id="07436-123">string</span></span>  | <span data-ttu-id="07436-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="07436-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07436-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="07436-126">Request body</span></span>
<span data-ttu-id="07436-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="07436-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07436-128">応答</span><span class="sxs-lookup"><span data-stu-id="07436-128">Response</span></span>

<span data-ttu-id="07436-129">成功した場合、このメソッドは`200 OK`応答コードと、応答本文で[デバイス](../resources/device.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="07436-129">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="07436-130">例</span><span class="sxs-lookup"><span data-stu-id="07436-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07436-131">要求</span><span class="sxs-lookup"><span data-stu-id="07436-131">Request</span></span>
<span data-ttu-id="07436-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="07436-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="07436-133">応答</span><span class="sxs-lookup"><span data-stu-id="07436-133">Response</span></span>
<span data-ttu-id="07436-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="07436-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
