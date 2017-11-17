# <a name="list-group-settings"></a><span data-ttu-id="29d12-101">グループ設定の一覧表示</span><span class="sxs-lookup"><span data-stu-id="29d12-101">List group settings</span></span>

<span data-ttu-id="29d12-102">グループ設定オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="29d12-102">Retrieve a list of group setting objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="29d12-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="29d12-103">Permissions</span></span>

<span data-ttu-id="29d12-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="29d12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="29d12-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="29d12-106">Permission type</span></span>      | <span data-ttu-id="29d12-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="29d12-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29d12-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="29d12-108">Delegated (work or school account)</span></span> | <span data-ttu-id="29d12-109">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="29d12-109">One of the following scopes is required to execute this API: Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="29d12-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="29d12-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29d12-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29d12-111">Not supported.</span></span>    |
|<span data-ttu-id="29d12-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="29d12-112">Application</span></span> | <span data-ttu-id="29d12-113">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29d12-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29d12-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="29d12-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="29d12-115">テナント全体またはグループ設定を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="29d12-115">List tenant-wide or group settings.</span></span>

```http
GET /groupSettings
GET group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="29d12-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="29d12-116">Optional query parameters</span></span>
<span data-ttu-id="29d12-117">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://graph.microsoft.io/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="29d12-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="29d12-118">注: $filter はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29d12-118">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="29d12-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="29d12-119">Request headers</span></span>
| <span data-ttu-id="29d12-120">名前</span><span class="sxs-lookup"><span data-stu-id="29d12-120">Name</span></span> | <span data-ttu-id="29d12-121">説明</span><span class="sxs-lookup"><span data-stu-id="29d12-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="29d12-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="29d12-122">Authorization</span></span>  | <span data-ttu-id="29d12-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="29d12-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29d12-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="29d12-125">Request body</span></span>
<span data-ttu-id="29d12-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="29d12-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29d12-127">応答</span><span class="sxs-lookup"><span data-stu-id="29d12-127">Response</span></span>

<span data-ttu-id="29d12-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [groupSetting](../resources/groupsetting.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="29d12-128">If successful, this method returns a `200 OK` response code and collection of [groupSetting](../resources/groupsetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="29d12-129">例</span><span class="sxs-lookup"><span data-stu-id="29d12-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="29d12-130">要求</span><span class="sxs-lookup"><span data-stu-id="29d12-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettings
```
##### <a name="response"></a><span data-ttu-id="29d12-131">応答</span><span class="sxs-lookup"><span data-stu-id="29d12-131">Response</span></span>

<span data-ttu-id="29d12-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="29d12-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "displayName": "displayName-value",
      "templateId": "templateId-value",
      "values": [
        {
          "name": "name-value",
          "value": "value-value"
        }
      ],
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->