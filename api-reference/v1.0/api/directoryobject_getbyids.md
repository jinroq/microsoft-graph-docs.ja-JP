# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="ac76b-101">ID のリストからディレクトリ オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="ac76b-101">Get directory objects from a list of ids</span></span>

<span data-ttu-id="ac76b-p101">ID のリストで指定されたディレクトリ オブジェクトを返します。注:ここで返されるディレクトリ オブジェクトは、**すべて**のプロパティを含む完全なオブジェクトです。この操作に `$select` クエリ オプションは使用できません。</span><span class="sxs-lookup"><span data-stu-id="ac76b-p101">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="ac76b-105">この関数の一般的な用途は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="ac76b-105">Some common uses for this function are to:</span></span>

* <span data-ttu-id="ac76b-106">[getMemberObjects](directoryobject_getmemberobjects.md) または [getMemberGroups](directoryobject_getmembergroups.md) などの (ID のコレクションを返す) 関数から返された ID を、バッキング ディレクトリ オブジェクトに解決する。</span><span class="sxs-lookup"><span data-stu-id="ac76b-106">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](directoryobject_getmemberobjects.md) or [getMemberGroups](directoryobject_getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="ac76b-107">アプリケーションによって外部記憶装置に保存されている ID をバッキング ディレクトリ オブジェクトに解決する。</span><span class="sxs-lookup"><span data-stu-id="ac76b-107">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac76b-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ac76b-108">Permissions</span></span>

<span data-ttu-id="ac76b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ac76b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="ac76b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ac76b-111">Permission type</span></span>      | <span data-ttu-id="ac76b-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ac76b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac76b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ac76b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ac76b-114">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ac76b-114">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ac76b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ac76b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac76b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac76b-116">Not supported.</span></span>    |
|<span data-ttu-id="ac76b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ac76b-117">Application</span></span> | <span data-ttu-id="ac76b-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac76b-118">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac76b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ac76b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getById
```

## <a name="request-headers"></a><span data-ttu-id="ac76b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ac76b-120">Request headers</span></span>

| <span data-ttu-id="ac76b-121">名前</span><span class="sxs-lookup"><span data-stu-id="ac76b-121">Name</span></span>       | <span data-ttu-id="ac76b-122">型</span><span class="sxs-lookup"><span data-stu-id="ac76b-122">Type</span></span> | <span data-ttu-id="ac76b-123">説明</span><span class="sxs-lookup"><span data-stu-id="ac76b-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ac76b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac76b-124">Authorization</span></span>  | <span data-ttu-id="ac76b-125">string</span><span class="sxs-lookup"><span data-stu-id="ac76b-125">string</span></span>  | <span data-ttu-id="ac76b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ac76b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ac76b-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ac76b-128">Content-Type</span></span>  | <span data-ttu-id="ac76b-129">application/json</span><span class="sxs-lookup"><span data-stu-id="ac76b-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ac76b-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="ac76b-130">Request body</span></span>

<span data-ttu-id="ac76b-131">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="ac76b-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ac76b-132">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ac76b-132">Parameter</span></span>   | <span data-ttu-id="ac76b-133">型</span><span class="sxs-lookup"><span data-stu-id="ac76b-133">Type</span></span> |<span data-ttu-id="ac76b-134">説明</span><span class="sxs-lookup"><span data-stu-id="ac76b-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac76b-135">ids</span><span class="sxs-lookup"><span data-stu-id="ac76b-135">ids</span></span>|<span data-ttu-id="ac76b-136">String collection</span><span class="sxs-lookup"><span data-stu-id="ac76b-136">String collection</span></span>| <span data-ttu-id="ac76b-p104">オブジェクトを戻す ID のコレクション。最大 1000 ID まで指定できます。</span><span class="sxs-lookup"><span data-stu-id="ac76b-p104">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="ac76b-139">types</span><span class="sxs-lookup"><span data-stu-id="ac76b-139">types</span></span>|<span data-ttu-id="ac76b-140">String collection</span><span class="sxs-lookup"><span data-stu-id="ac76b-140">String collection</span></span>| <span data-ttu-id="ac76b-p105">検索する一連のリソース コレクションを指定するリソース型のコレクションです。指定しない場合、既定値は、ディレクトリで定義されているすべてのリソース型を含む [directoryObject](../resources/directoryobject.md) になります。`directoryObject` から派生する任意のオブジェクトをコレクションに指定できます。例: [user](../resources/user.md)、[group](../resources/group.md)、[device](../resources/device.md) など。値では、大文字と小文字は区別されません。</span><span class="sxs-lookup"><span data-stu-id="ac76b-p105">A collection of resource types that specifies the set of resource collections to search. If not specified, the default is [directoryObject](../resources/directoryobject.md), which contains all of the resource types defined in the directory. Any object that derives from `directoryObject` may be specified in the collection; for example: [user](../resources/user.md), [group](../resources/group.md), [device](../resources/device.md), and so on. The values are not case sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="ac76b-145">応答</span><span class="sxs-lookup"><span data-stu-id="ac76b-145">Response</span></span>

<span data-ttu-id="ac76b-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ac76b-146">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac76b-147">例</span><span class="sxs-lookup"><span data-stu-id="ac76b-147">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ac76b-148">要求</span><span class="sxs-lookup"><span data-stu-id="ac76b-148">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getById"
}-->

```http
POST https://graph.microsoft.com/v1.0/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893-8749-40a3-97b7-68513b600544","5d6059b6-368d-45f8-91e1-8e07d485f1d0"],
    "types":["user"]
}
```

##### <a name="response"></a><span data-ttu-id="ac76b-149">応答</span><span class="sxs-lookup"><span data-stu-id="ac76b-149">Response</span></span>

<span data-ttu-id="ac76b-p106">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ac76b-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
