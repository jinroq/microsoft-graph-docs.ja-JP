# <a name="update-permission"></a><span data-ttu-id="c1323-101">アクセス許可を更新する</span><span class="sxs-lookup"><span data-stu-id="c1323-101">Update permission</span></span>

<span data-ttu-id="c1323-102">アクセス許可のプロパティを更新するには、リソースの更新プログラムを適用します。</span><span class="sxs-lookup"><span data-stu-id="c1323-102">Update the properties of a permission by patching the resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1323-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c1323-103">Permissions</span></span>

<span data-ttu-id="c1323-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c1323-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c1323-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c1323-106">Permission type</span></span>      | <span data-ttu-id="c1323-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c1323-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1323-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c1323-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c1323-109">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1323-109">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c1323-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c1323-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1323-111">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1323-111">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c1323-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c1323-112">Application</span></span> | <span data-ttu-id="c1323-113">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1323-113">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1323-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c1323-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/root:/{path}:/permissions/{perm-id}
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="request-headers"></a><span data-ttu-id="c1323-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c1323-115">Request headers</span></span>

| <span data-ttu-id="c1323-116">名前</span><span class="sxs-lookup"><span data-stu-id="c1323-116">Name</span></span>          | <span data-ttu-id="c1323-117">型</span><span class="sxs-lookup"><span data-stu-id="c1323-117">Type</span></span>   | <span data-ttu-id="c1323-118">説明</span><span class="sxs-lookup"><span data-stu-id="c1323-118">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c1323-119">if-match</span><span class="sxs-lookup"><span data-stu-id="c1323-119">if-match</span></span>      | <span data-ttu-id="c1323-120">string</span><span class="sxs-lookup"><span data-stu-id="c1323-120">string</span></span> | <span data-ttu-id="c1323-121">この要求ヘッダーが含まれていて、指定された eTag (または cTag) が項目の現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、項目は削除されません。</span><span class="sxs-lookup"><span data-stu-id="c1323-121">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1323-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="c1323-122">Request body</span></span>
<span data-ttu-id="c1323-p102">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="c1323-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c1323-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1323-126">Property</span></span>     | <span data-ttu-id="c1323-127">型</span><span class="sxs-lookup"><span data-stu-id="c1323-127">Type</span></span>   | <span data-ttu-id="c1323-128">説明</span><span class="sxs-lookup"><span data-stu-id="c1323-128">Description</span></span>                   |
|:-------------|:-------|:------------------------------|
| <span data-ttu-id="c1323-129">**roles**</span><span class="sxs-lookup"><span data-stu-id="c1323-129">**roles**</span></span>    | <span data-ttu-id="c1323-130">String</span><span class="sxs-lookup"><span data-stu-id="c1323-130">String</span></span> | <span data-ttu-id="c1323-131">アクセス許可の種類の配列。</span><span class="sxs-lookup"><span data-stu-id="c1323-131">An array of permission types.</span></span> |

## <a name="response"></a><span data-ttu-id="c1323-132">応答</span><span class="sxs-lookup"><span data-stu-id="c1323-132">Response</span></span>

<span data-ttu-id="c1323-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[アクセス許可](../resources/permission.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c1323-133">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1323-134">例</span><span class="sxs-lookup"><span data-stu-id="c1323-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c1323-135">要求</span><span class="sxs-lookup"><span data-stu-id="c1323-135">Request</span></span>

<span data-ttu-id="c1323-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c1323-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_permission"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```
##### <a name="response"></a><span data-ttu-id="c1323-137">応答</span><span class="sxs-lookup"><span data-stu-id="c1323-137">Response</span></span>

<span data-ttu-id="c1323-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c1323-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "read" ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission"
}-->
