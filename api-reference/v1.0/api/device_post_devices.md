# <a name="create-device"></a><span data-ttu-id="40128-101">デバイスを作成する</span><span class="sxs-lookup"><span data-stu-id="40128-101">Create device</span></span>

<span data-ttu-id="40128-102">新しいデバイスを作成し、組織に登録します。</span><span class="sxs-lookup"><span data-stu-id="40128-102">Create and register a new device in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="40128-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="40128-103">Permissions</span></span>
<span data-ttu-id="40128-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="40128-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="40128-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="40128-106">Permission type</span></span>      | <span data-ttu-id="40128-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="40128-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40128-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="40128-108">Delegated (work or school account)</span></span> | <span data-ttu-id="40128-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="40128-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="40128-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="40128-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40128-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40128-111">Not supported.</span></span>    |
|<span data-ttu-id="40128-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="40128-112">Application</span></span> | <span data-ttu-id="40128-113">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40128-113">Device.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="40128-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="40128-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="40128-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40128-115">Request headers</span></span>
| <span data-ttu-id="40128-116">名前</span><span class="sxs-lookup"><span data-stu-id="40128-116">Name</span></span>       | <span data-ttu-id="40128-117">型</span><span class="sxs-lookup"><span data-stu-id="40128-117">Type</span></span> | <span data-ttu-id="40128-118">説明</span><span class="sxs-lookup"><span data-stu-id="40128-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="40128-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="40128-119">Authorization</span></span>  | <span data-ttu-id="40128-120">string</span><span class="sxs-lookup"><span data-stu-id="40128-120">string</span></span>  | <span data-ttu-id="40128-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="40128-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="40128-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="40128-123">Content-type</span></span> | <span data-ttu-id="40128-124">string</span><span class="sxs-lookup"><span data-stu-id="40128-124">string</span></span> | <span data-ttu-id="40128-125">application/json</span><span class="sxs-lookup"><span data-stu-id="40128-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="40128-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="40128-126">Request body</span></span>
<span data-ttu-id="40128-127">要求本文で、[デバイス](../resources/device.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="40128-127">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="40128-128">応答</span><span class="sxs-lookup"><span data-stu-id="40128-128">Response</span></span>

<span data-ttu-id="40128-129">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で[デバイス](../resources/device.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="40128-129">If successful, this method returns `201, Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40128-130">例</span><span class="sxs-lookup"><span data-stu-id="40128-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="40128-131">要求</span><span class="sxs-lookup"><span data-stu-id="40128-131">Request</span></span>
<span data-ttu-id="40128-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="40128-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_device_from_devices"
}-->
```http
POST https://graph.microsoft.com/v1.0/devices
Content-type: application/json

{
  "accountEnabled":false,
  "alternativeSecurityIds":
  [
    {
      "type":2,
      "key":"Y3YxN2E1MWFlYw=="
    }
  ],
  "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
  "displayName":"Test device",
  "operatingSystem":"linux",
  "operatingSystemVersion":"1"
}
```
<span data-ttu-id="40128-133">要求本文で、[デバイス](../resources/device.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="40128-133">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="40128-134">応答</span><span class="sxs-lookup"><span data-stu-id="40128-134">Response</span></span>
<span data-ttu-id="40128-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="40128-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "accountEnabled":false,
  "alternativeSecurityIds":
  [
    {
      "type":2,
      "key":"Y3YxN2E1MWFlYw=="
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
  "description": "Create device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
