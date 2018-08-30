# <a name="listing-versions-of-a-listitem"></a><span data-ttu-id="ffaf5-101">リストアイテムのバージョンを一覧表示</span><span class="sxs-lookup"><span data-stu-id="ffaf5-101">Listing versions of a ListItem (preview)</span></span>

<span data-ttu-id="ffaf5-102">SharePoint は、リスト アイテムの履歴を保持するように構成できます。</span><span class="sxs-lookup"><span data-stu-id="ffaf5-102">SharePoint can be configured to retain the history for list items.</span></span>

<span data-ttu-id="ffaf5-103">旧バージョンは、ユーザーまたは場所ごとに固有の場合がある管理者設定に応じて、一定期間保持することができます。</span><span class="sxs-lookup"><span data-stu-id="ffaf5-103">Previous versions may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="ffaf5-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ffaf5-104">Permissions</span></span>

<span data-ttu-id="ffaf5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ffaf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|            <span data-ttu-id="ffaf5-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ffaf5-107">Permission type</span></span>             | <span data-ttu-id="ffaf5-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ffaf5-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="ffaf5-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ffaf5-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="ffaf5-110">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffaf5-110">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="ffaf5-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ffaf5-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ffaf5-112">該当なし</span><span class="sxs-lookup"><span data-stu-id="ffaf5-112">n/a</span></span>                                         |
| <span data-ttu-id="ffaf5-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ffaf5-113">Application</span></span>                            | <span data-ttu-id="ffaf5-114">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffaf5-114">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="ffaf5-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ffaf5-115">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="ffaf5-116">応答</span><span class="sxs-lookup"><span data-stu-id="ffaf5-116">Response</span></span>

<span data-ttu-id="ffaf5-117">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [ListItemVersion](../resources/listitemversion.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ffaf5-117">If successful, this method returns a `200 OK` response code and collection of [ListItemVersion](../resources/listitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="ffaf5-118">例</span><span class="sxs-lookup"><span data-stu-id="ffaf5-118">Example</span></span>

<span data-ttu-id="ffaf5-119">次の使用例では、SharePoint リスト内のリスト アイテムのバージョンを取得します。</span><span class="sxs-lookup"><span data-stu-id="ffaf5-119">This example retrieves the versions of a listItem in a SharePoint list:</span></span>

### <a name="http-request"></a><span data-ttu-id="ffaf5-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ffaf5-120">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions-listitem", "scopes": "files.read sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="ffaf5-121">応答</span><span class="sxs-lookup"><span data-stu-id="ffaf5-121">Response</span></span>

<span data-ttu-id="ffaf5-122">バージョンのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ffaf5-122">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.listItemVersion)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value":
  [
    {
      "id": "3.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-14T12:34:53.912Z"
    },
    {
      "id": "2.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-11T10:21:03.000Z"
    },
    {
      "id": "1.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-10T15:20:01.125Z"
    }
  ]
}
```


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
