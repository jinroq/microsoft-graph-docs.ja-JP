# <a name="list-available-drives"></a><span data-ttu-id="eaa6b-101">利用可能なドライブの一覧表示</span><span class="sxs-lookup"><span data-stu-id="eaa6b-101">List available drives</span></span>

<span data-ttu-id="eaa6b-p101">ターゲットとなる[ユーザー](../resources/user.md)または[グループ](../resources/group.md)が利用可能な[ドライブ](../resources/drive.md) リソースの一覧を取得します。SharePoint のルートサイト上のドキュメント ライブラリのセットをアプリで要求することもできます。</span><span class="sxs-lookup"><span data-stu-id="eaa6b-p101">Retrieve the list of [Drive](../resources/drive.md) resources available for a target [User](../resources/user.md) or [Group](../resources/group.md). Your app can also request the set of document libraries on the SharePoint root site.</span></span>

## <a name="permissions"></a><span data-ttu-id="eaa6b-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="eaa6b-104">Permissions</span></span>

<span data-ttu-id="eaa6b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eaa6b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="eaa6b-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eaa6b-107">Permission type</span></span>      | <span data-ttu-id="eaa6b-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="eaa6b-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eaa6b-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eaa6b-109">Delegated (work or school account)</span></span> | <span data-ttu-id="eaa6b-110">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaa6b-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="eaa6b-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eaa6b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eaa6b-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaa6b-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="eaa6b-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eaa6b-113">Application</span></span> | <span data-ttu-id="eaa6b-114">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaa6b-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eaa6b-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eaa6b-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives
GET /me/drives
GET /sites/{site-id}/drives
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eaa6b-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="eaa6b-116">Optional query parameters</span></span>
<span data-ttu-id="eaa6b-117">このメソッドは、応答をカスタマイズするための `$expand``$select`、`$skipToken`、`$top`、および `$orderby` [OData クエリ パラメーター](../../../concepts/query_parameters.md)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="eaa6b-117">This method supports the `$expand` and `$orderby` [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="eaa6b-118">要求本文</span><span class="sxs-lookup"><span data-stu-id="eaa6b-118">Request body</span></span>

<span data-ttu-id="eaa6b-119">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="eaa6b-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eaa6b-120">応答</span><span class="sxs-lookup"><span data-stu-id="eaa6b-120">Response</span></span>

<span data-ttu-id="eaa6b-121">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Drive](../resources/drive.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="eaa6b-121">If successful, this method returns a `200 OK` response code and collection of [Drive](../resources/drive.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eaa6b-122">例</span><span class="sxs-lookup"><span data-stu-id="eaa6b-122">Example</span></span>

##### <a name="request"></a><span data-ttu-id="eaa6b-123">要求</span><span class="sxs-lookup"><span data-stu-id="eaa6b-123">Request</span></span>

<span data-ttu-id="eaa6b-124">以下はユーザーのドライブの要求例です。</span><span class="sxs-lookup"><span data-stu-id="eaa6b-124">Here is an example of the request for the user's drives.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drives"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/drives
```

##### <a name="response"></a><span data-ttu-id="eaa6b-125">応答</span><span class="sxs-lookup"><span data-stu-id="eaa6b-125">Response</span></span>

<span data-ttu-id="eaa6b-126">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="eaa6b-126">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.drive",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 579

{
  "value": [
    {
      "id": "b!t18F8ybsHUq1z3LTz8xvZqP8zaSWjkFNhsME-Fepo75dTf9vQKfeRblBZjoSQrd7",
      "driveType": "business",
      "owner": {
          "user": {
              "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
              "displayName": "Ryan Gregg"
          }
      },
      "quota": {
          "deleted": 256938,
          "remaining": 1099447353539,
          "state": "normal",
          "total": 1099511627776
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="eaa6b-127">注釈</span><span class="sxs-lookup"><span data-stu-id="eaa6b-127">Remarks</span></span>

<span data-ttu-id="eaa6b-p103">ほとんどのユーザーには、ドライブ リソースが 1 つしかありません。複数のドライブが利用可能なグループとユーザーもあります。</span><span class="sxs-lookup"><span data-stu-id="eaa6b-p103">Most users will only have a single Drive resource. Groups and some users may have multiple drive available.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List drives",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/List Drives"
}-->
