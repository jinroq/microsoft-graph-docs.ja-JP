# <a name="list-memberof"></a><span data-ttu-id="ae2b5-101">memberOf を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ae2b5-101">List memberOf</span></span>

<span data-ttu-id="ae2b5-102">ユーザーがダイレクト メンバーになっている[グループ](../resources/group.md)と[ディレクトリ ロール](../resources/directoryrole.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="ae2b5-102">Get [groups](../resources/group.md) and [directory roles](../resources/directoryrole.md) that the user is a direct member of.</span></span> 

## <a name="permissions"></a><span data-ttu-id="ae2b5-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ae2b5-103">Permissions</span></span>
<span data-ttu-id="ae2b5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae2b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ae2b5-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae2b5-106">Permission type</span></span>      | <span data-ttu-id="ae2b5-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae2b5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae2b5-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae2b5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ae2b5-109">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ae2b5-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ae2b5-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae2b5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae2b5-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae2b5-111">Not supported.</span></span>    |
|<span data-ttu-id="ae2b5-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae2b5-112">Application</span></span> | <span data-ttu-id="ae2b5-113">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae2b5-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae2b5-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae2b5-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ae2b5-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ae2b5-115">Optional query parameters</span></span>
<span data-ttu-id="ae2b5-p102">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。$filter はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae2b5-p102">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response. $filter is not supported.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="ae2b5-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae2b5-118">Request headers</span></span>
| <span data-ttu-id="ae2b5-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae2b5-119">Header</span></span>       | <span data-ttu-id="ae2b5-120">値</span><span class="sxs-lookup"><span data-stu-id="ae2b5-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ae2b5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae2b5-121">Authorization</span></span>  | <span data-ttu-id="ae2b5-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ae2b5-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ae2b5-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ae2b5-124">Accept</span></span>  | <span data-ttu-id="ae2b5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ae2b5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae2b5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ae2b5-126">Request body</span></span>
<span data-ttu-id="ae2b5-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ae2b5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae2b5-128">応答</span><span class="sxs-lookup"><span data-stu-id="ae2b5-128">Response</span></span>

<span data-ttu-id="ae2b5-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ae2b5-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ae2b5-130">例</span><span class="sxs-lookup"><span data-stu-id="ae2b5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae2b5-131">要求</span><span class="sxs-lookup"><span data-stu-id="ae2b5-131">Request</span></span>
<span data-ttu-id="ae2b5-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ae2b5-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/memberOf
```
##### <a name="response"></a><span data-ttu-id="ae2b5-133">応答</span><span class="sxs-lookup"><span data-stu-id="ae2b5-133">Response</span></span>
<span data-ttu-id="ae2b5-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ae2b5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
