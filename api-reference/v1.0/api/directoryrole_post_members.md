# <a name="add-directory-role-member"></a><span data-ttu-id="5dfee-101">ディレクトリ ロールのメンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="5dfee-101">Add directory role member</span></span>

<span data-ttu-id="5dfee-102">この API を使用して、新しいディレクトリ ロールのメンバーを作成します。</span><span class="sxs-lookup"><span data-stu-id="5dfee-102">Use this API to create a new directory role member.</span></span>

## <a name="permissions"></a><span data-ttu-id="5dfee-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5dfee-103">Permissions</span></span>
<span data-ttu-id="5dfee-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5dfee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5dfee-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5dfee-106">Permission type</span></span>      | <span data-ttu-id="5dfee-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5dfee-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5dfee-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5dfee-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5dfee-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5dfee-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5dfee-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5dfee-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5dfee-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5dfee-111">Not supported.</span></span>    |
|<span data-ttu-id="5dfee-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5dfee-112">Application</span></span> | <span data-ttu-id="5dfee-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5dfee-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5dfee-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5dfee-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="5dfee-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5dfee-115">Request headers</span></span>
| <span data-ttu-id="5dfee-116">名前</span><span class="sxs-lookup"><span data-stu-id="5dfee-116">Name</span></span>       | <span data-ttu-id="5dfee-117">型</span><span class="sxs-lookup"><span data-stu-id="5dfee-117">Type</span></span> | <span data-ttu-id="5dfee-118">説明</span><span class="sxs-lookup"><span data-stu-id="5dfee-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5dfee-119">承認</span><span class="sxs-lookup"><span data-stu-id="5dfee-119">Authorization</span></span>  | <span data-ttu-id="5dfee-120">文字列</span><span class="sxs-lookup"><span data-stu-id="5dfee-120">string</span></span>  | <span data-ttu-id="5dfee-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5dfee-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5dfee-123">コンテンツ タイプ</span><span class="sxs-lookup"><span data-stu-id="5dfee-123">Content-Type</span></span>  | <span data-ttu-id="5dfee-124">文字列</span><span class="sxs-lookup"><span data-stu-id="5dfee-124">string</span></span>  | <span data-ttu-id="5dfee-125">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="5dfee-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5dfee-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="5dfee-126">Request body</span></span>
<span data-ttu-id="5dfee-127">要求本文で、追加する [directoryObject](../resources/directoryobject.md) または[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5dfee-127">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="5dfee-128">応答</span><span class="sxs-lookup"><span data-stu-id="5dfee-128">Response</span></span>

<span data-ttu-id="5dfee-129">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="5dfee-129">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5dfee-130">例</span><span class="sxs-lookup"><span data-stu-id="5dfee-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5dfee-131">要求</span><span class="sxs-lookup"><span data-stu-id="5dfee-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/{id}/members/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```

##### <a name="response"></a><span data-ttu-id="5dfee-132">応答</span><span class="sxs-lookup"><span data-stu-id="5dfee-132">Response</span></span>
<span data-ttu-id="5dfee-133">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="5dfee-133">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain

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