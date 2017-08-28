# <a name="get-permission"></a><span data-ttu-id="57274-101">アクセス許可を取得する</span><span class="sxs-lookup"><span data-stu-id="57274-101">Get permission</span></span>

<span data-ttu-id="57274-102">アクセス許可オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="57274-102">Retrieve the properties and relationships of permission object.</span></span>

## <a name="permissions"></a><span data-ttu-id="57274-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="57274-103">Permissions</span></span>
<span data-ttu-id="57274-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="57274-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="57274-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="57274-106">Permission type</span></span>      | <span data-ttu-id="57274-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="57274-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57274-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="57274-108">Delegated (work or school account)</span></span> | <span data-ttu-id="57274-109">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57274-109">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="57274-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="57274-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57274-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57274-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="57274-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="57274-112">Application</span></span> | <span data-ttu-id="57274-113">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57274-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="57274-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="57274-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{item-id}/permissions/{perm-id}
GET /me/drive/root:/{path}:/permissions/{perm-id}
GET /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
GET /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="57274-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="57274-115">Optional query parameters</span></span>
<span data-ttu-id="57274-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="57274-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="57274-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="57274-117">Request body</span></span>
<span data-ttu-id="57274-118">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="57274-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57274-119">応答</span><span class="sxs-lookup"><span data-stu-id="57274-119">Response</span></span>

<span data-ttu-id="57274-120">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Permission](../resources/permission.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="57274-120">If successful, this method returns a `200 OK` response code and [Permission](../resources/permission.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57274-121">例</span><span class="sxs-lookup"><span data-stu-id="57274-121">Example</span></span>

##### <a name="request"></a><span data-ttu-id="57274-122">要求</span><span class="sxs-lookup"><span data-stu-id="57274-122">Request</span></span>

<span data-ttu-id="57274-123">以下は、ルート フォルダーのアクセス許可にアクセスするための要求の例です。</span><span class="sxs-lookup"><span data-stu-id="57274-123">Here is an example of the request to access a permission on the root folder.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_permission"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/permissions/{perm-id}
```
##### <a name="response"></a><span data-ttu-id="57274-124">応答</span><span class="sxs-lookup"><span data-stu-id="57274-124">Response</span></span>
<span data-ttu-id="57274-125">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="57274-125">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 762

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "write" ]
}
```

## <a name="remarks"></a><span data-ttu-id="57274-126">備考</span><span class="sxs-lookup"><span data-stu-id="57274-126">Remarks</span></span>

<span data-ttu-id="57274-127">[アクセス権](../resources/permission.md)リソースは、_ファセット_を使用してリソースによって表されるアクセス許可の種類に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="57274-127">The [Permission](../resources/permission.md) resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="57274-p102">[**リンク**](../resources/sharinglink.md) ファセットのあるアクセス許可は、項目上に作成された共有するリンクを表します。共有リンクは、リンクを持つすべてのユーザーのアイテムへのアクセス許可を提供する固有のトークンを含みます。</span><span class="sxs-lookup"><span data-stu-id="57274-p102">Permissions with a [**link**](../resources/sharinglink.md) facet represent sharing links created on the item. Sharing links contain a unique token that provides access to the item for anyone with the link.</span></span>

<span data-ttu-id="57274-130">[**招待**](../resources/sharinginvitation.md) ファセットを持つアクセス許可は、指定のユーザーやグループをファイルへのアクセスへ招待することで追加されたアクセス許可を表します。</span><span class="sxs-lookup"><span data-stu-id="57274-130">Permissions with a [**invitation**](../resources/sharinginvitation.md) facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Get permission"
}-->
