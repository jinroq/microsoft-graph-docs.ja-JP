# <a name="list-members"></a><span data-ttu-id="bb783-101">メンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="bb783-101">List members</span></span>

<span data-ttu-id="bb783-p101">ディレクトリ ロールに割り当てられているユーザーの一覧を取得します。ディレクトリに割り当てることができるのはユーザーのみです。</span><span class="sxs-lookup"><span data-stu-id="bb783-p101">Retrieve a list of the users that are assigned to the directory role.  Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="bb783-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bb783-104">Permissions</span></span>
<span data-ttu-id="bb783-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb783-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="bb783-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bb783-107">Permission type</span></span>      | <span data-ttu-id="bb783-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bb783-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb783-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bb783-109">Delegated (work or school account)</span></span> | <span data-ttu-id="bb783-110">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bb783-110">One of the following scopes is required to execute this API: Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bb783-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bb783-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb783-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb783-112">Not supported.</span></span>    |
|<span data-ttu-id="bb783-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bb783-113">Application</span></span> | <span data-ttu-id="bb783-114">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb783-114">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb783-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bb783-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bb783-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="bb783-116">Optional query parameters</span></span>
<span data-ttu-id="bb783-117">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="bb783-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bb783-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bb783-118">Request headers</span></span>
| <span data-ttu-id="bb783-119">名前</span><span class="sxs-lookup"><span data-stu-id="bb783-119">Name</span></span>       | <span data-ttu-id="bb783-120">型</span><span class="sxs-lookup"><span data-stu-id="bb783-120">Type</span></span> | <span data-ttu-id="bb783-121">説明</span><span class="sxs-lookup"><span data-stu-id="bb783-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bb783-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb783-122">Authorization</span></span>  | <span data-ttu-id="bb783-123">string</span><span class="sxs-lookup"><span data-stu-id="bb783-123">string</span></span>  | <span data-ttu-id="bb783-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bb783-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb783-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="bb783-126">Request body</span></span>
<span data-ttu-id="bb783-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bb783-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb783-128">応答</span><span class="sxs-lookup"><span data-stu-id="bb783-128">Response</span></span>

<span data-ttu-id="bb783-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="bb783-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bb783-130">例</span><span class="sxs-lookup"><span data-stu-id="bb783-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb783-131">要求</span><span class="sxs-lookup"><span data-stu-id="bb783-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles/{id}/members
```
##### <a name="response"></a><span data-ttu-id="bb783-132">応答</span><span class="sxs-lookup"><span data-stu-id="bb783-132">Response</span></span>
<span data-ttu-id="bb783-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bb783-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "businessPhones":["000-000-0000"],
      "displayName":"First Last",
      "givenName":"First",
      "jobTitle":null,
      "mail":"first@example.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Last",
      "userPrincipalName":"first@example.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->