# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="daea4-101">ID のリストからディレクトリ オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="daea4-101">Get directory objects from a list of ids</span></span>

<span data-ttu-id="daea4-p101">ID のリストで指定されたディレクトリ オブジェクトを返します。注:ここで返されるディレクトリ オブジェクトは、**すべて**のプロパティを含む完全なオブジェクトです。この操作に `$select` クエリ オプションは使用できません。</span><span class="sxs-lookup"><span data-stu-id="daea4-p101">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="daea4-105">この関数の一般的な用途は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="daea4-105">Some common uses for this function are to:</span></span>

* <span data-ttu-id="daea4-106">[getMemberObjects](directoryobject_getmemberobjects.md) または [getMemberGroups](directoryobject_getmembergroups.md) などの (ID のコレクションを返す) 関数から返された ID を、バッキング ディレクトリ オブジェクトに解決する。</span><span class="sxs-lookup"><span data-stu-id="daea4-106">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](directoryobject_getmemberobjects.md) or [getMemberGroups](directoryobject_getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="daea4-107">アプリケーションによって外部記憶装置に保存されている ID をバッキング ディレクトリ オブジェクトに解決する。</span><span class="sxs-lookup"><span data-stu-id="daea4-107">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="daea4-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="daea4-108">Permissions</span></span>

<span data-ttu-id="daea4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="daea4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="daea4-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="daea4-111">Permission type</span></span>      | <span data-ttu-id="daea4-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="daea4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="daea4-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="daea4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="daea4-114">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="daea4-114">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="daea4-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="daea4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="daea4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="daea4-116">Not supported.</span></span>    |
|<span data-ttu-id="daea4-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="daea4-117">Application</span></span> | <span data-ttu-id="daea4-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="daea4-118">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="daea4-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="daea4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="daea4-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="daea4-120">Request headers</span></span>

| <span data-ttu-id="daea4-121">名前</span><span class="sxs-lookup"><span data-stu-id="daea4-121">Name</span></span>       | <span data-ttu-id="daea4-122">型</span><span class="sxs-lookup"><span data-stu-id="daea4-122">Type</span></span> | <span data-ttu-id="daea4-123">説明</span><span class="sxs-lookup"><span data-stu-id="daea4-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="daea4-124">承認</span><span class="sxs-lookup"><span data-stu-id="daea4-124">Authorization</span></span>  | <span data-ttu-id="daea4-125">文字列</span><span class="sxs-lookup"><span data-stu-id="daea4-125">string</span></span>  | <span data-ttu-id="daea4-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="daea4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="daea4-128">コンテンツ タイプ</span><span class="sxs-lookup"><span data-stu-id="daea4-128">Content-Type</span></span>  | <span data-ttu-id="daea4-129">文字列</span><span class="sxs-lookup"><span data-stu-id="daea4-129">string</span></span> | <span data-ttu-id="daea4-130">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="daea4-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="daea4-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="daea4-131">Request body</span></span>

<span data-ttu-id="daea4-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="daea4-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="daea4-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="daea4-133">Parameter</span></span>   | <span data-ttu-id="daea4-134">型</span><span class="sxs-lookup"><span data-stu-id="daea4-134">Type</span></span> |<span data-ttu-id="daea4-135">説明</span><span class="sxs-lookup"><span data-stu-id="daea4-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="daea4-136">ids</span><span class="sxs-lookup"><span data-stu-id="daea4-136">ids</span></span>|<span data-ttu-id="daea4-137">String コレクション</span><span class="sxs-lookup"><span data-stu-id="daea4-137">String collection</span></span>| <span data-ttu-id="daea4-p104">オブジェクトを戻す ID のコレクション。最大 1000 ID まで指定できます。</span><span class="sxs-lookup"><span data-stu-id="daea4-p104">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="daea4-140">types</span><span class="sxs-lookup"><span data-stu-id="daea4-140">types</span></span>|<span data-ttu-id="daea4-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="daea4-141">String collection</span></span>| <span data-ttu-id="daea4-142">検索するリソース コレクションのセットを指定するリソースの種類のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="daea4-142">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="daea4-143">指定しない場合、既定では [directoryObject](../resources/directoryobject.md) となります。これには、すべてのディレクトリで定義されているリソースの種類が含まれます。</span><span class="sxs-lookup"><span data-stu-id="daea4-143">If not specified, the default is [directoryObject](../resources/directoryobject.md), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="daea4-144">`directoryObject` から派生したオブジェクトは、コレクションに指定されることがあります。たとえば、[ユーザー](../resources/user.md)、 [グループ](../resources/group.md)、 [デバイス](../resources/device.md)などです。</span><span class="sxs-lookup"><span data-stu-id="daea4-144">Any object that derives from `directoryObject` may be specified in the collection; for example: [user](../resources/user.md), [group](../resources/group.md), [device](../resources/device.md), and so on.</span></span> <span data-ttu-id="daea4-145">この値は、大文字と小文字は区別されません。</span><span class="sxs-lookup"><span data-stu-id="daea4-145">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="daea4-146">応答</span><span class="sxs-lookup"><span data-stu-id="daea4-146">Response</span></span>

<span data-ttu-id="daea4-147">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="daea4-147">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="daea4-148">例</span><span class="sxs-lookup"><span data-stu-id="daea4-148">Example</span></span>

##### <a name="request"></a><span data-ttu-id="daea4-149">要求</span><span class="sxs-lookup"><span data-stu-id="daea4-149">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getById"
}-->

```http
POST https://graph.microsoft.com/v1.0/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893874940a3-97b7-68513b600544","5d6059b6368d-45f8-91e18e07d485f1d0"],
    "types":["user"]
}
```

##### <a name="response"></a><span data-ttu-id="daea4-150">応答</span><span class="sxs-lookup"><span data-stu-id="daea4-150">Response</span></span>

<span data-ttu-id="daea4-p106">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="daea4-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
    "value": [
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Trevor Jones"
      },
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Billy Smith"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
