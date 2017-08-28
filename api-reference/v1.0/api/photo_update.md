# <a name="update-photo"></a><span data-ttu-id="60285-101">写真を更新する</span><span class="sxs-lookup"><span data-stu-id="60285-101">Update photo</span></span>

<span data-ttu-id="60285-102">写真オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="60285-102">Update the properties of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="60285-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="60285-103">Permissions</span></span>
<span data-ttu-id="60285-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="60285-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="60285-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="60285-106">Permission type</span></span>      | <span data-ttu-id="60285-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="60285-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60285-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="60285-108">Delegated (work or school account)</span></span> | <span data-ttu-id="60285-109">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60285-109">Not supported.</span></span>    |
|<span data-ttu-id="60285-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="60285-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60285-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60285-111">Not supported.</span></span>    |
|<span data-ttu-id="60285-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="60285-112">Application</span></span> | <span data-ttu-id="60285-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60285-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="60285-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="60285-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/photo
PATCH /groups/{id}/photo
PATCH /drive/root/createdByUser/photo
```

## <a name="request-headers"></a><span data-ttu-id="60285-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60285-115">Request headers</span></span>
| <span data-ttu-id="60285-116">名前</span><span class="sxs-lookup"><span data-stu-id="60285-116">Name</span></span>       | <span data-ttu-id="60285-117">型</span><span class="sxs-lookup"><span data-stu-id="60285-117">Type</span></span> | <span data-ttu-id="60285-118">説明</span><span class="sxs-lookup"><span data-stu-id="60285-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="60285-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="60285-119">Authorization</span></span>  | <span data-ttu-id="60285-120">string</span><span class="sxs-lookup"><span data-stu-id="60285-120">string</span></span>  | <span data-ttu-id="60285-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="60285-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60285-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="60285-123">Request body</span></span>
<span data-ttu-id="60285-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="60285-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="60285-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60285-127">Property</span></span>     | <span data-ttu-id="60285-128">型</span><span class="sxs-lookup"><span data-stu-id="60285-128">Type</span></span>   |<span data-ttu-id="60285-129">説明</span><span class="sxs-lookup"><span data-stu-id="60285-129">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="60285-130">応答</span><span class="sxs-lookup"><span data-stu-id="60285-130">Response</span></span>

<span data-ttu-id="60285-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[写真](../resources/photo.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="60285-131">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="60285-132">例</span><span class="sxs-lookup"><span data-stu-id="60285-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="60285-133">要求</span><span class="sxs-lookup"><span data-stu-id="60285-133">Request</span></span>
<span data-ttu-id="60285-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="60285-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_photo"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
##### <a name="response"></a><span data-ttu-id="60285-135">応答</span><span class="sxs-lookup"><span data-stu-id="60285-135">Response</span></span>
<span data-ttu-id="60285-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="60285-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
