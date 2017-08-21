# <a name="delete-device"></a><span data-ttu-id="10d29-101">デバイスを削除する</span><span class="sxs-lookup"><span data-stu-id="10d29-101">Delete device</span></span>

<span data-ttu-id="10d29-102">登録されているデバイスを削除します。</span><span class="sxs-lookup"><span data-stu-id="10d29-102">Delete a registered device.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10d29-103">前提条件</span><span class="sxs-lookup"><span data-stu-id="10d29-103">Prerequisites</span></span>
<span data-ttu-id="10d29-104">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Directory.AccessAsUser.All*、*Device.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="10d29-104">One of the following **scopes** is required to execute this API: *Directory.AccessAsUser.All*, *Device.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="10d29-105">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="10d29-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="10d29-106">注:要求内の"id"は、"deviceId"プロパティではなく、デバイスの id プロパティです。</span><span class="sxs-lookup"><span data-stu-id="10d29-106">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10d29-107">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="10d29-107">Request headers</span></span>
| <span data-ttu-id="10d29-108">名前</span><span class="sxs-lookup"><span data-stu-id="10d29-108">Name</span></span>       | <span data-ttu-id="10d29-109">型</span><span class="sxs-lookup"><span data-stu-id="10d29-109">Type</span></span> | <span data-ttu-id="10d29-110">説明</span><span class="sxs-lookup"><span data-stu-id="10d29-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="10d29-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="10d29-111">Authorization</span></span>  | <span data-ttu-id="10d29-112">string</span><span class="sxs-lookup"><span data-stu-id="10d29-112">string</span></span>  | <span data-ttu-id="10d29-p101">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="10d29-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10d29-115">要求本文</span><span class="sxs-lookup"><span data-stu-id="10d29-115">Request body</span></span>
<span data-ttu-id="10d29-116">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="10d29-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10d29-117">応答</span><span class="sxs-lookup"><span data-stu-id="10d29-117">Response</span></span>

<span data-ttu-id="10d29-p102">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="10d29-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10d29-120">例</span><span class="sxs-lookup"><span data-stu-id="10d29-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="10d29-121">要求</span><span class="sxs-lookup"><span data-stu-id="10d29-121">Request</span></span>
<span data-ttu-id="10d29-122">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="10d29-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="10d29-123">応答</span><span class="sxs-lookup"><span data-stu-id="10d29-123">Response</span></span>
<span data-ttu-id="10d29-124">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="10d29-124">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
