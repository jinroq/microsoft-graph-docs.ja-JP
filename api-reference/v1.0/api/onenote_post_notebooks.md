# <a name="create-notebook"></a><span data-ttu-id="4331b-101">ノートブックを作成する</span><span class="sxs-lookup"><span data-stu-id="4331b-101">Create notebook</span></span>

<span data-ttu-id="4331b-102">新しい OneNote [ノートブック](../resources/notebook.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="4331b-102">Create a new OneNote [notebook](../resources/notebook.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="4331b-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4331b-103">Permissions</span></span>
<span data-ttu-id="4331b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4331b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4331b-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4331b-106">Permission type</span></span>      | <span data-ttu-id="4331b-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4331b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4331b-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4331b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4331b-109">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4331b-109">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="4331b-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4331b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4331b-111">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4331b-111">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="4331b-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4331b-112">Application</span></span> | <span data-ttu-id="4331b-113">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4331b-113">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4331b-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4331b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks
POST /users/{id | userPrincipalName}/onenote/notebooks
POST /groups/{id}/onenote/notebooks
POST /sites/{id}/onenote/notebooks
```
## <a name="request-headers"></a><span data-ttu-id="4331b-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4331b-115">Request headers</span></span>
| <span data-ttu-id="4331b-116">名前</span><span class="sxs-lookup"><span data-stu-id="4331b-116">Name</span></span>       | <span data-ttu-id="4331b-117">型</span><span class="sxs-lookup"><span data-stu-id="4331b-117">Type</span></span> | <span data-ttu-id="4331b-118">説明</span><span class="sxs-lookup"><span data-stu-id="4331b-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4331b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="4331b-119">Authorization</span></span>  | <span data-ttu-id="4331b-120">string</span><span class="sxs-lookup"><span data-stu-id="4331b-120">string</span></span>  | <span data-ttu-id="4331b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4331b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4331b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4331b-123">Content-Type</span></span> | <span data-ttu-id="4331b-124">string</span><span class="sxs-lookup"><span data-stu-id="4331b-124">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="4331b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="4331b-125">Request body</span></span>
<span data-ttu-id="4331b-126">要求本文で、ノートブックの名前を入力します。</span><span class="sxs-lookup"><span data-stu-id="4331b-126">In the request body, supply a name for the notebook.</span></span> 

<span data-ttu-id="4331b-p103">ノートブック名は一意にする必要があります。名前は 128 文字以内で、次の文字は使用できません:  ?\*\/:<>|'"</span><span class="sxs-lookup"><span data-stu-id="4331b-p103">Notebook names must be unique. The name cannot contain more than 128 characters or contain the following characters:  ?\*\/:<>|'"</span></span>

## <a name="response"></a><span data-ttu-id="4331b-129">応答</span><span class="sxs-lookup"><span data-stu-id="4331b-129">Response</span></span>

<span data-ttu-id="4331b-130">成功した場合、このメソッドは応答本文で `201 Created` 応答コードと新しい [notebook](../resources/notebook.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4331b-130">If successful, this method returns a `201 Created` response code and the new [notebook](../resources/notebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4331b-131">例</span><span class="sxs-lookup"><span data-stu-id="4331b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4331b-132">要求</span><span class="sxs-lookup"><span data-stu-id="4331b-132">Request</span></span>
<span data-ttu-id="4331b-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4331b-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_notebook_from_onenote"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks
Content-type: application/json
Content-length: 30

{
  "displayName": "Notebook name"
}
```

##### <a name="response"></a><span data-ttu-id="4331b-134">応答</span><span class="sxs-lookup"><span data-stu-id="4331b-134">Response</span></span>
<span data-ttu-id="4331b-p104">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4331b-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 284

{
  "isDefault": true,
  "userRole": {
  },
  "isShared": true,
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
