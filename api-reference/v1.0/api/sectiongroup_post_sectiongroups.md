# <a name="create-sectiongroup"></a><span data-ttu-id="d6621-101">sectionGroup を作成する</span><span class="sxs-lookup"><span data-stu-id="d6621-101">Create sectionGroup</span></span>

<span data-ttu-id="d6621-102">指定されたセクション グループに新しい[セクション グループ](../resources/sectiongroup.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="d6621-102">Create a new [section group](../resources/sectiongroup.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="d6621-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d6621-103">Permissions</span></span>
<span data-ttu-id="d6621-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d6621-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d6621-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d6621-106">Permission type</span></span>      | <span data-ttu-id="d6621-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d6621-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6621-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d6621-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d6621-109">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6621-109">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="d6621-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d6621-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6621-111">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6621-111">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="d6621-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d6621-112">Application</span></span> | <span data-ttu-id="d6621-113">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6621-113">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6621-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d6621-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
POST /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
POST /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="d6621-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d6621-115">Request headers</span></span>
| <span data-ttu-id="d6621-116">名前</span><span class="sxs-lookup"><span data-stu-id="d6621-116">Name</span></span>       | <span data-ttu-id="d6621-117">型</span><span class="sxs-lookup"><span data-stu-id="d6621-117">Type</span></span> | <span data-ttu-id="d6621-118">説明</span><span class="sxs-lookup"><span data-stu-id="d6621-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d6621-119">承認</span><span class="sxs-lookup"><span data-stu-id="d6621-119">Authorization</span></span>  | <span data-ttu-id="d6621-120">文字列</span><span class="sxs-lookup"><span data-stu-id="d6621-120">string</span></span>  | <span data-ttu-id="d6621-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d6621-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d6621-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d6621-123">Content-Type</span></span> | <span data-ttu-id="d6621-124">string</span><span class="sxs-lookup"><span data-stu-id="d6621-124">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="d6621-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d6621-125">Request body</span></span>
<span data-ttu-id="d6621-126">要求本文でセクション グループ名を指定します。</span><span class="sxs-lookup"><span data-stu-id="d6621-126">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="d6621-p103">同じ階層レベルのセクション グループには一意の名前が必要です。名前は 50 文字以内で、次の文字は使用できません: ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="d6621-p103">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="d6621-129">応答</span><span class="sxs-lookup"><span data-stu-id="d6621-129">Response</span></span>

<span data-ttu-id="d6621-130">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [sectionGroup](../resources/sectiongroup.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d6621-130">If successful, this method returns a `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6621-131">例</span><span class="sxs-lookup"><span data-stu-id="d6621-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d6621-132">要求</span><span class="sxs-lookup"><span data-stu-id="d6621-132">Request</span></span>
<span data-ttu-id="d6621-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d6621-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_sectiongroup_from_sectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}/sectionGroups
Content-type: application/json
Content-length: 30

{
  "displayName": "Section group name"
}
```
##### <a name="response"></a><span data-ttu-id="d6621-134">応答</span><span class="sxs-lookup"><span data-stu-id="d6621-134">Response</span></span>
<span data-ttu-id="d6621-p104">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d6621-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectionGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

{
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "displayName": "name-value",  
  "createdBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "lastModifiedBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create SectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->