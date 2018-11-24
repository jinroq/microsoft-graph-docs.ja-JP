# <a name="get-tab"></a><span data-ttu-id="5f47a-101">タブを取得します。</span><span class="sxs-lookup"><span data-stu-id="5f47a-101">Get tab</span></span>



<span data-ttu-id="5f47a-102">プロパティと、指定した[タブ](../resources/teamstab.md)の関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="5f47a-102">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="5f47a-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5f47a-103">Permissions</span></span>
<span data-ttu-id="5f47a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5f47a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5f47a-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5f47a-106">Permission type</span></span>      | <span data-ttu-id="5f47a-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5f47a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f47a-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5f47a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5f47a-109">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f47a-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5f47a-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5f47a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f47a-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f47a-111">Not supported.</span></span>    |
|<span data-ttu-id="5f47a-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5f47a-112">Application</span></span> | <span data-ttu-id="5f47a-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f47a-113">Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="5f47a-114">現在、[委任されたアクセス許可](../../../concepts/permissions_reference.md)をのみがこの操作に対してサポートされています。</span><span class="sxs-lookup"><span data-stu-id="5f47a-114">Currently, only [delegated permissions](../../../concepts/permissions_reference.md) are supported for this operation.</span></span>

## <a name="http-request"></a><span data-ttu-id="5f47a-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5f47a-115">HTTP request</span></span>
```http
GET /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5f47a-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5f47a-116">Optional query parameters</span></span>

<span data-ttu-id="5f47a-117">このメソッドは、$select をサポートし、$ は、応答をカスタマイズするために[OData クエリ パラメーター](../../../concepts/query_parameters.md)を展開します。</span><span class="sxs-lookup"><span data-stu-id="5f47a-117">This method supports the $select, and $expand [OData query parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f47a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5f47a-118">Request headers</span></span>
| <span data-ttu-id="5f47a-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5f47a-119">Header</span></span>       | <span data-ttu-id="5f47a-120">値</span><span class="sxs-lookup"><span data-stu-id="5f47a-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5f47a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f47a-121">Authorization</span></span>  | <span data-ttu-id="5f47a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5f47a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5f47a-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="5f47a-124">Request body</span></span>
<span data-ttu-id="5f47a-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5f47a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f47a-126">応答</span><span class="sxs-lookup"><span data-stu-id="5f47a-126">Response</span></span>

<span data-ttu-id="5f47a-127">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の[tab](../resources/teamstab.md)オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="5f47a-127">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5f47a-128">例</span><span class="sxs-lookup"><span data-stu-id="5f47a-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5f47a-129">要求</span><span class="sxs-lookup"><span data-stu-id="5f47a-129">Request</span></span>
<span data-ttu-id="5f47a-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5f47a-130">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="5f47a-131">応答</span><span class="sxs-lookup"><span data-stu-id="5f47a-131">Response</span></span>
<span data-ttu-id="5f47a-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5f47a-132">The following is an example of the response.</span></span> 

><span data-ttu-id="5f47a-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5f47a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get a channel tab",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
