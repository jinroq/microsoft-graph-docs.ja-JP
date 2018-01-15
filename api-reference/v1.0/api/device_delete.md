# <a name="delete-device"></a><span data-ttu-id="1505c-101">デバイスを削除する</span><span class="sxs-lookup"><span data-stu-id="1505c-101">Delete device</span></span>

<span data-ttu-id="1505c-102">登録されているデバイスを削除します。</span><span class="sxs-lookup"><span data-stu-id="1505c-102">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="1505c-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1505c-103">Permissions</span></span>
<span data-ttu-id="1505c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1505c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="1505c-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1505c-106">Permission type</span></span>      | <span data-ttu-id="1505c-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1505c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1505c-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1505c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1505c-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1505c-109">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="1505c-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1505c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1505c-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1505c-111">Not supported.</span></span>    |
|<span data-ttu-id="1505c-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1505c-112">Application</span></span> | <span data-ttu-id="1505c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1505c-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1505c-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1505c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="1505c-115">注:要求内の"id"は、"deviceId"プロパティではなく、デバイスの id プロパティです。</span><span class="sxs-lookup"><span data-stu-id="1505c-115">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1505c-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1505c-116">Request headers</span></span>
| <span data-ttu-id="1505c-117">名前</span><span class="sxs-lookup"><span data-stu-id="1505c-117">Name</span></span>       | <span data-ttu-id="1505c-118">型</span><span class="sxs-lookup"><span data-stu-id="1505c-118">Type</span></span> | <span data-ttu-id="1505c-119">説明</span><span class="sxs-lookup"><span data-stu-id="1505c-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1505c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1505c-120">Authorization</span></span>  | <span data-ttu-id="1505c-121">string</span><span class="sxs-lookup"><span data-stu-id="1505c-121">string</span></span>  | <span data-ttu-id="1505c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1505c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1505c-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="1505c-124">Request body</span></span>
<span data-ttu-id="1505c-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1505c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1505c-126">応答</span><span class="sxs-lookup"><span data-stu-id="1505c-126">Response</span></span>

<span data-ttu-id="1505c-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1505c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1505c-129">例</span><span class="sxs-lookup"><span data-stu-id="1505c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1505c-130">要求</span><span class="sxs-lookup"><span data-stu-id="1505c-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="1505c-131">応答</span><span class="sxs-lookup"><span data-stu-id="1505c-131">Response</span></span>

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
