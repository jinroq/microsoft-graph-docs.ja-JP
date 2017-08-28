# <a name="update-device"></a><span data-ttu-id="bab09-101">デバイスを更新する</span><span class="sxs-lookup"><span data-stu-id="bab09-101">Update device</span></span>

<span data-ttu-id="bab09-102">登録済みデバイスのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bab09-102">Update the properties of a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="bab09-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bab09-103">Permissions</span></span>
<span data-ttu-id="bab09-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bab09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="bab09-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bab09-106">Permission type</span></span>      | <span data-ttu-id="bab09-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bab09-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bab09-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bab09-108">Delegated (work or school account)</span></span> | <span data-ttu-id="bab09-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bab09-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bab09-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bab09-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bab09-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bab09-111">Not supported.</span></span>    |
|<span data-ttu-id="bab09-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bab09-112">Application</span></span> | <span data-ttu-id="bab09-113">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bab09-113">Device.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bab09-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bab09-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```
> <span data-ttu-id="bab09-115">注:要求内の"id"は、"deviceId"プロパティではなく、デバイスの id プロパティです。</span><span class="sxs-lookup"><span data-stu-id="bab09-115">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bab09-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bab09-116">Request headers</span></span>
| <span data-ttu-id="bab09-117">名前</span><span class="sxs-lookup"><span data-stu-id="bab09-117">Name</span></span>       | <span data-ttu-id="bab09-118">型</span><span class="sxs-lookup"><span data-stu-id="bab09-118">Type</span></span> | <span data-ttu-id="bab09-119">説明</span><span class="sxs-lookup"><span data-stu-id="bab09-119">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bab09-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bab09-120">Authorization</span></span>  | <span data-ttu-id="bab09-121">string</span><span class="sxs-lookup"><span data-stu-id="bab09-121">string</span></span>  | <span data-ttu-id="bab09-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bab09-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bab09-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="bab09-124">Request body</span></span>
<span data-ttu-id="bab09-125">要求本文で、更新する[デバイス](../resources/device.md) プロパティの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="bab09-125">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span>

## <a name="response"></a><span data-ttu-id="bab09-126">応答</span><span class="sxs-lookup"><span data-stu-id="bab09-126">Response</span></span>

<span data-ttu-id="bab09-127">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="bab09-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bab09-128">例</span><span class="sxs-lookup"><span data-stu-id="bab09-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bab09-129">要求</span><span class="sxs-lookup"><span data-stu-id="bab09-129">Request</span></span>
<span data-ttu-id="bab09-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bab09-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_device"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/devices/{id}
Content-type: application/json

{
  "accountEnabled": true
}
```
##### <a name="response"></a><span data-ttu-id="bab09-131">応答</span><span class="sxs-lookup"><span data-stu-id="bab09-131">Response</span></span>
<span data-ttu-id="bab09-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bab09-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```
