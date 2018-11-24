# <a name="list-tabs-in-channel"></a><span data-ttu-id="b088d-101">チャネルの一覧] タブ</span><span class="sxs-lookup"><span data-stu-id="b088d-101">List tabs in channel</span></span>



<span data-ttu-id="b088d-102">[チーム](../resources/team.md)内で指定された[チャネル](../resources/channel.md)で[のタブ](../resources/teamstab.md)のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="b088d-102">Retrieve the list of [tabs](../resources/teamstab.md) in the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="b088d-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b088d-103">Permissions</span></span>
<span data-ttu-id="b088d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b088d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b088d-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b088d-106">Permission type</span></span>      | <span data-ttu-id="b088d-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b088d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b088d-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b088d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b088d-109">Group.ReadWrite.All、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b088d-109">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="b088d-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b088d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b088d-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b088d-111">Not supported.</span></span>    |
| <span data-ttu-id="b088d-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b088d-112">Application</span></span>                            | <span data-ttu-id="b088d-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b088d-113">Group.Read.All, Group.ReadWrite.All</span></span>         |

## <a name="http-request"></a><span data-ttu-id="b088d-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b088d-114">HTTP request</span></span>

```http
GET /teams/{id}/channels/{id}/tabs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b088d-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b088d-115">Optional query parameters</span></span>

<span data-ttu-id="b088d-116">このメソッドは、$filter、$select をサポートしていて、$ は、応答をカスタマイズするために[OData クエリ パラメーター](../../../concepts/query_parameters.md)を展開します。</span><span class="sxs-lookup"><span data-stu-id="b088d-116">This method supports the $filter, $select, and $expand [OData query parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b088d-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b088d-117">Request headers</span></span>
| <span data-ttu-id="b088d-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b088d-118">Header</span></span>       | <span data-ttu-id="b088d-119">値</span><span class="sxs-lookup"><span data-stu-id="b088d-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b088d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b088d-120">Authorization</span></span>  | <span data-ttu-id="b088d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b088d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b088d-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="b088d-123">Request body</span></span>
<span data-ttu-id="b088d-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b088d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b088d-125">応答</span><span class="sxs-lookup"><span data-stu-id="b088d-125">Response</span></span>
<span data-ttu-id="b088d-126">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[タブ](../resources/teamstab.md)のオブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="b088d-126">If successful, this method returns a `200 OK` response code and collection of [tabs](../resources/teamstab.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b088d-127">例</span><span class="sxs-lookup"><span data-stu-id="b088d-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b088d-128">要求</span><span class="sxs-lookup"><span data-stu-id="b088d-128">Request</span></span>
<span data-ttu-id="b088d-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b088d-129">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs
```

#### <a name="response"></a><span data-ttu-id="b088d-130">応答</span><span class="sxs-lookup"><span data-stu-id="b088d-130">Response</span></span>
<span data-ttu-id="b088d-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b088d-131">The following is an example of the response.</span></span>
><span data-ttu-id="b088d-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b088d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 Success
Content-type: application/json

{
  "value": [
    {
      "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
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
    },
    {
      "id": "b5d5f001-0471-49a5-aac4-04ef96683be0",
      "name": "My Trello Tab",
      "teamsAppId": "23134c6b-5e4b-439c-8f70-3ded1df20805",
      "configuration": null,
      "sortOrderIndex": 21,
      "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3a3709b35c-a0ba-467c-8001-0f66895fb9d3?label=My%20Trello%Tab"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List all tabs in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
