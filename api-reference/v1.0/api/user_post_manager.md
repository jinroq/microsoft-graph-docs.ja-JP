# <a name="assign-a-manager"></a><span data-ttu-id="f5458-101">上司を割り当てる</span><span class="sxs-lookup"><span data-stu-id="f5458-101">Assign a manager</span></span>

<span data-ttu-id="f5458-102">この API を使用して、ユーザーの上司を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="f5458-102">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="f5458-103">注:直属の部下を割り当てることはできません。代わりにこの API を使用します。</span><span class="sxs-lookup"><span data-stu-id="f5458-103">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5458-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f5458-104">Permissions</span></span>
<span data-ttu-id="f5458-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f5458-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f5458-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f5458-107">Permission type</span></span>      | <span data-ttu-id="f5458-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f5458-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5458-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f5458-109">Delegated (work or school account)</span></span> | <span data-ttu-id="f5458-110">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f5458-110">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f5458-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f5458-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5458-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5458-112">Not supported.</span></span>    |
|<span data-ttu-id="f5458-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f5458-113">Application</span></span> | <span data-ttu-id="f5458-114">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5458-114">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5458-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f5458-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="f5458-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f5458-116">Request headers</span></span>
| <span data-ttu-id="f5458-117">名前</span><span class="sxs-lookup"><span data-stu-id="f5458-117">Name</span></span>       | <span data-ttu-id="f5458-118">型</span><span class="sxs-lookup"><span data-stu-id="f5458-118">Type</span></span> | <span data-ttu-id="f5458-119">説明</span><span class="sxs-lookup"><span data-stu-id="f5458-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f5458-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5458-120">Authorization</span></span>  | <span data-ttu-id="f5458-121">string</span><span class="sxs-lookup"><span data-stu-id="f5458-121">string</span></span>  | <span data-ttu-id="f5458-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f5458-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5458-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="f5458-124">Request body</span></span>
<span data-ttu-id="f5458-125">要求本文で、追加する [directoryObject](../resources/directoryobject.md) または[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f5458-125">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="f5458-126">応答</span><span class="sxs-lookup"><span data-stu-id="f5458-126">Response</span></span>

<span data-ttu-id="f5458-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="f5458-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5458-129">例</span><span class="sxs-lookup"><span data-stu-id="f5458-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f5458-130">要求</span><span class="sxs-lookup"><span data-stu-id="f5458-130">Request</span></span>
<span data-ttu-id="f5458-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f5458-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
PUT https://graph.microsoft.com/v1.0/users/{id}/manager/$ref
Content-type: application/json
Content-length: xxx

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="f5458-132">要求本文で、追加する[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f5458-132">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="f5458-133">応答</span><span class="sxs-lookup"><span data-stu-id="f5458-133">Response</span></span>
<span data-ttu-id="f5458-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f5458-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
