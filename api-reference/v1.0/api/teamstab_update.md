# <a name="update-tab"></a><span data-ttu-id="c2b0d-101">[更新] タブ</span><span class="sxs-lookup"><span data-stu-id="c2b0d-101">Update tab</span></span>



<span data-ttu-id="c2b0d-102">指定した[タブ](../resources/teamstab.md)のプロパティを更新します。タブのコンテンツを構成するのには、これを使用できます。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-102">Update the properties of the specified [tab](../resources/teamstab.md). This can be used to configure the content of the tab.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2b0d-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c2b0d-103">Permissions</span></span>
<span data-ttu-id="c2b0d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="c2b0d-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c2b0d-106">Permission type</span></span>      | <span data-ttu-id="c2b0d-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2b0d-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c2b0d-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2b0d-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c2b0d-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c2b0d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2b0d-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-111">Not supported.</span></span>    |
|<span data-ttu-id="c2b0d-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c2b0d-112">Application</span></span>                            | <span data-ttu-id="c2b0d-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2b0d-113">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c2b0d-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c2b0d-114">HTTP request</span></span>
```http
PATCH /teams/{id}/channels/{id}/tabs/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c2b0d-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c2b0d-115">Request headers</span></span>
| <span data-ttu-id="c2b0d-116">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c2b0d-116">Header</span></span>       | <span data-ttu-id="c2b0d-117">値</span><span class="sxs-lookup"><span data-stu-id="c2b0d-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c2b0d-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2b0d-118">Authorization</span></span>  | <span data-ttu-id="c2b0d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c2b0d-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c2b0d-121">Content-Type</span></span>  | <span data-ttu-id="c2b0d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c2b0d-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c2b0d-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="c2b0d-123">Request body</span></span>
<span data-ttu-id="c2b0d-124">要求の本文には、 [tab](../resources/teamstab.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-124">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c2b0d-125">応答</span><span class="sxs-lookup"><span data-stu-id="c2b0d-125">Response</span></span>

<span data-ttu-id="c2b0d-126">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c2b0d-127">例</span><span class="sxs-lookup"><span data-stu-id="c2b0d-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c2b0d-128">要求</span><span class="sxs-lookup"><span data-stu-id="c2b0d-128">Request</span></span>
<span data-ttu-id="c2b0d-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-129">The following is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
Content-type: application/json
Content-length: 211

{
  "name": "My Contoso Tab - updated"
}
```
#### <a name="response"></a><span data-ttu-id="c2b0d-130">応答</span><span class="sxs-lookup"><span data-stu-id="c2b0d-130">Response</span></span>
```http
HTTP/1.1 200 Success
Content-type: application/json

{
  "id": "tabId",
  "name": "My Contoso Tab - updated",
  "teamsAppId": "06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "sortOrderIndex": 20,
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```

## <a name="see-also"></a><span data-ttu-id="c2b0d-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="c2b0d-131">See also</span></span>

[<span data-ttu-id="c2b0d-132">組み込みタブのタイプを設定します。</span><span class="sxs-lookup"><span data-stu-id="c2b0d-132">Configuring the built-in tab types</span></span>](../../../concepts/teams-configuring-builtin-tabs.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tab in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
