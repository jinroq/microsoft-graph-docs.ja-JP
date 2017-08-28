# <a name="create-registereduser"></a><span data-ttu-id="4d123-101">RegisteredUser を作成する</span><span class="sxs-lookup"><span data-stu-id="4d123-101">Create registeredUser</span></span>

<span data-ttu-id="4d123-102">デバイスの登録済みユーザーを追加します。</span><span class="sxs-lookup"><span data-stu-id="4d123-102">Add a registered user for the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d123-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4d123-103">Permissions</span></span>
<span data-ttu-id="4d123-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d123-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="4d123-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4d123-106">Permission type</span></span>      | <span data-ttu-id="4d123-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4d123-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d123-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4d123-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4d123-109">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4d123-109">Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4d123-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4d123-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d123-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d123-111">Not supported.</span></span>    |
|<span data-ttu-id="4d123-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4d123-112">Application</span></span> | <span data-ttu-id="4d123-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d123-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d123-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4d123-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredUsers

```
## <a name="request-headers"></a><span data-ttu-id="4d123-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4d123-115">Request headers</span></span>
| <span data-ttu-id="4d123-116">名前</span><span class="sxs-lookup"><span data-stu-id="4d123-116">Name</span></span>       | <span data-ttu-id="4d123-117">型</span><span class="sxs-lookup"><span data-stu-id="4d123-117">Type</span></span> | <span data-ttu-id="4d123-118">説明</span><span class="sxs-lookup"><span data-stu-id="4d123-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4d123-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d123-119">Authorization</span></span>  | <span data-ttu-id="4d123-120">string</span><span class="sxs-lookup"><span data-stu-id="4d123-120">string</span></span>  | <span data-ttu-id="4d123-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4d123-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d123-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="4d123-123">Request body</span></span>
<span data-ttu-id="4d123-124">要求本文で、[directoryObject](../resources/directoryobject.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4d123-124">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4d123-125">応答</span><span class="sxs-lookup"><span data-stu-id="4d123-125">Response</span></span>

<span data-ttu-id="4d123-126">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4d123-126">If successful, this method returns `201, Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d123-127">例</span><span class="sxs-lookup"><span data-stu-id="4d123-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4d123-128">要求</span><span class="sxs-lookup"><span data-stu-id="4d123-128">Request</span></span>
<span data-ttu-id="4d123-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4d123-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="4d123-130">要求本文で、[directoryObject](../resources/directoryobject.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4d123-130">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4d123-131">応答</span><span class="sxs-lookup"><span data-stu-id="4d123-131">Response</span></span>
<span data-ttu-id="4d123-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4d123-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "directoryObject": {
    "id": "id-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create registeredUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->