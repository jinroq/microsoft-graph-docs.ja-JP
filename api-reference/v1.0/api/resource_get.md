# <a name="get-resource"></a><span data-ttu-id="2a10d-101">リソースを取得する</span><span class="sxs-lookup"><span data-stu-id="2a10d-101">Get resource</span></span>

<span data-ttu-id="2a10d-102">ファイルまたは画像の[リソース](../resources/resource.md) オブジェクトのバイナリ データを取得します。</span><span class="sxs-lookup"><span data-stu-id="2a10d-102">Retrieve the binary data of a file or image [resource](../resources/resource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2a10d-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2a10d-103">Permissions</span></span>
<span data-ttu-id="2a10d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a10d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2a10d-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2a10d-106">Permission type</span></span>      | <span data-ttu-id="2a10d-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2a10d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a10d-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2a10d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="2a10d-109">Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a10d-109">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="2a10d-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2a10d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a10d-111">Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a10d-111">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="2a10d-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2a10d-112">Application</span></span> | <span data-ttu-id="2a10d-113">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a10d-113">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a10d-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2a10d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="2a10d-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2a10d-115">Request headers</span></span>
| <span data-ttu-id="2a10d-116">名前</span><span class="sxs-lookup"><span data-stu-id="2a10d-116">Name</span></span>       | <span data-ttu-id="2a10d-117">型</span><span class="sxs-lookup"><span data-stu-id="2a10d-117">Type</span></span> | <span data-ttu-id="2a10d-118">説明</span><span class="sxs-lookup"><span data-stu-id="2a10d-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2a10d-119">承認</span><span class="sxs-lookup"><span data-stu-id="2a10d-119">Authorization</span></span>  | <span data-ttu-id="2a10d-120">文字列</span><span class="sxs-lookup"><span data-stu-id="2a10d-120">string</span></span>  | <span data-ttu-id="2a10d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2a10d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a10d-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="2a10d-123">Request body</span></span>
<span data-ttu-id="2a10d-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2a10d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a10d-125">応答</span><span class="sxs-lookup"><span data-stu-id="2a10d-125">Response</span></span>

<span data-ttu-id="2a10d-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で画像またはファイルのバイナリ データを返します。</span><span class="sxs-lookup"><span data-stu-id="2a10d-126">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="2a10d-127">注:残りのページのコンテンツと同様、画像を取得するには承認が必要となるため、ブラウザーでは画像は直接表示されません。</span><span class="sxs-lookup"><span data-stu-id="2a10d-127">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="2a10d-128">例</span><span class="sxs-lookup"><span data-stu-id="2a10d-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2a10d-129">要求</span><span class="sxs-lookup"><span data-stu-id="2a10d-129">Request</span></span>
<span data-ttu-id="2a10d-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2a10d-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/resources/{id}/content
```
##### <a name="response"></a><span data-ttu-id="2a10d-131">応答</span><span class="sxs-lookup"><span data-stu-id="2a10d-131">Response</span></span>
<span data-ttu-id="2a10d-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="2a10d-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Edm.Stream"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

...binary data...
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
