# <a name="list-permissions-on-a-driveitem"></a><span data-ttu-id="70912-101">DriveItem のアクセス許可を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="70912-101">List permissions on a DriveItem</span></span>

<span data-ttu-id="70912-102">[DriveItem](../resources/driveitem.md) の有効なアクセス許可を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="70912-102">List the effective permissions of on a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="70912-p101">DriveItem の **permissions** リレーションシップは、[DriveItem の取得](item_get.md)または DriveItem のコレクションの取得の一環として展開することはできません。permissions プロパティに直接アクセスする必要があります。</span><span class="sxs-lookup"><span data-stu-id="70912-p101">The **permissions** relationship of DriveItem cannot be expanded as part of a call to [get DriveItem](item_get.md) or a collection of DriveItems. You must access the permissions property directly.</span></span>

## <a name="access-to-permissions"></a><span data-ttu-id="70912-105">アクセス許可にアクセスする</span><span class="sxs-lookup"><span data-stu-id="70912-105">Access to Permissions</span></span>

<span data-ttu-id="70912-106">アクセス許可のコレクションには、機密情報が含まれている可能性があり、呼び出し元によっては使用できないこともあります。</span><span class="sxs-lookup"><span data-stu-id="70912-106">The permissions collection includes potentially sensitive information and may not be available for every caller.</span></span>

* <span data-ttu-id="70912-p102">アイテムのオーナーの場合は、すべてのアクセス許可が返されます。これには、共同所有者が含まれます。</span><span class="sxs-lookup"><span data-stu-id="70912-p102">For the owner of the item, all permissions will be returned. This includes co-owners.</span></span>
* <span data-ttu-id="70912-109">所有者以外の呼び出し元の場合、その呼び出し元に適用されるアクセス許可のみが返されます。</span><span class="sxs-lookup"><span data-stu-id="70912-109">For a non-owner caller, only the permissions that apply to the caller are returned.</span></span>
* <span data-ttu-id="70912-110">秘密 (`shareId` や `webUrl` など) を含むアクセス許可のプロパティは、そのアクセス許可を作成できる呼び出し元にのみ返されます。</span><span class="sxs-lookup"><span data-stu-id="70912-110">Permission properties that contain secrets (e.g. `shareId` and `webUrl`) are only returned for callers that are able to create the Permission.</span></span>

## <a name="permissions"></a><span data-ttu-id="70912-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="70912-111">Permissions</span></span>
<span data-ttu-id="70912-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="70912-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="70912-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="70912-114">Permission type</span></span>      | <span data-ttu-id="70912-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="70912-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70912-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="70912-116">Delegated (work or school account)</span></span> | <span data-ttu-id="70912-117">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70912-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="70912-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="70912-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70912-119">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70912-119">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="70912-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="70912-120">Application</span></span> | <span data-ttu-id="70912-121">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70912-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70912-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="70912-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{item-id}/permissions
GET /me/drive/root:/{path}:/permissions
GET /drives/{drive-id}/items/{item-id}/permissions
GET /groups/{group-id}/drive/items/{item-id}/permissions
```

## <a name="request-headers"></a><span data-ttu-id="70912-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="70912-123">Request headers</span></span>

| <span data-ttu-id="70912-124">名前</span><span class="sxs-lookup"><span data-stu-id="70912-124">Name</span></span>          | <span data-ttu-id="70912-125">型</span><span class="sxs-lookup"><span data-stu-id="70912-125">Type</span></span>   | <span data-ttu-id="70912-126">説明</span><span class="sxs-lookup"><span data-stu-id="70912-126">Description</span></span>                                                                                                                                     |
|:--------------|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="70912-127">if-none-match</span><span class="sxs-lookup"><span data-stu-id="70912-127">if-none-match</span></span> | <span data-ttu-id="70912-128">string</span><span class="sxs-lookup"><span data-stu-id="70912-128">string</span></span> | <span data-ttu-id="70912-129">この要求ヘッダーが含まれている場合、指定された etag がアイテムの現在の etag に一致すると、`HTTP 304 Not Modified` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="70912-129">If this request header is included and the etag provided matches the current etag on the item, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="70912-130">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="70912-130">Optional query parameters</span></span>
<span data-ttu-id="70912-131">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="70912-131">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="70912-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="70912-132">Request body</span></span>
<span data-ttu-id="70912-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="70912-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70912-134">応答</span><span class="sxs-lookup"><span data-stu-id="70912-134">Response</span></span>

<span data-ttu-id="70912-135">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと、[Permission](../resources/permission.md) リソースのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="70912-135">If successful, this method returns a `200 OK` response code and collection of [Permission](../resources/permission.md) resources in the response body.</span></span>

<span data-ttu-id="70912-136">アイテムの有効なアクセス許可は、次の 2 つのソースが元になります。</span><span class="sxs-lookup"><span data-stu-id="70912-136">Effective permissions of an item can come from two sources:</span></span>

* <span data-ttu-id="70912-137">アイテム自体に直接適用されるアクセス許可</span><span class="sxs-lookup"><span data-stu-id="70912-137">Permissions applied directly on the item itself</span></span>
* <span data-ttu-id="70912-138">アイテムの先祖から継承されたアクセス許可</span><span class="sxs-lookup"><span data-stu-id="70912-138">Permissions inherited from the item's ancestors</span></span>

<span data-ttu-id="70912-p104">呼び出し元は、**inheritedFrom** プロパティを確認して、アクセス許可が継承されているかどうかによって区別できます。このプロパティは、アクセス許可が継承された先祖を参照する [**itemReference**](../resources/itemreference.md) リソースです。</span><span class="sxs-lookup"><span data-stu-id="70912-p104">Callers can differentiate if the permission is inherited or not by checking the **inheritedFrom** property. This property is an [**itemReference**](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

## <a name="example"></a><span data-ttu-id="70912-141">例</span><span class="sxs-lookup"><span data-stu-id="70912-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70912-142">要求</span><span class="sxs-lookup"><span data-stu-id="70912-142">Request</span></span>
<span data-ttu-id="70912-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="70912-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_permissions"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/permissions
```


##### <a name="response"></a><span data-ttu-id="70912-144">応答</span><span class="sxs-lookup"><span data-stu-id="70912-144">Response</span></span>
<span data-ttu-id="70912-145">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="70912-145">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit"
      }
    },
    {
      "id": "2",
      "roles": ["write"],
      "grantedTo": {
        "user": {
          "id": "5D33DD65C6932946",
          "displayName": "John Doe"
        }
      },
      "inheritedFrom": {
        "driveId": "1234567890ABD",
        "id": "1234567890ABC!123",
        "path": "/drive/root:/Documents" }
    },
    {
      "id": "3",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit",
        "application": {
          "id": "12345",
          "displayName": "TimeTravelPlus"
        }
      }
    }
  ]
}
```

<span data-ttu-id="70912-146">単一のアクセス許可リソースの取得の詳細については、「[アクセス許可を取得する](permission_get.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="70912-146">See [Get permission](permission_get.md) for more details on retrieving a single permission resource.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List permissions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/List permissions"
}-->
