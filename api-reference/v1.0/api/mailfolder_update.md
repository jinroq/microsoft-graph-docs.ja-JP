# <a name="update-mailfolder"></a><span data-ttu-id="4aee6-101">MailFolder を更新する</span><span class="sxs-lookup"><span data-stu-id="4aee6-101">Update mailfolder</span></span>

<span data-ttu-id="4aee6-102">mailFolder オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4aee6-102">Update the properties of mailfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4aee6-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4aee6-103">Permissions</span></span>
<span data-ttu-id="4aee6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4aee6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4aee6-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4aee6-106">Permission type</span></span>      | <span data-ttu-id="4aee6-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4aee6-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4aee6-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4aee6-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4aee6-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4aee6-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4aee6-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4aee6-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4aee6-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4aee6-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4aee6-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4aee6-112">Application</span></span> | <span data-ttu-id="4aee6-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4aee6-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4aee6-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4aee6-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4aee6-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4aee6-115">Request headers</span></span>
| <span data-ttu-id="4aee6-116">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4aee6-116">Header</span></span>       | <span data-ttu-id="4aee6-117">値</span><span class="sxs-lookup"><span data-stu-id="4aee6-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4aee6-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="4aee6-118">Authorization</span></span>  | <span data-ttu-id="4aee6-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4aee6-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4aee6-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4aee6-121">Content-Type</span></span>  | <span data-ttu-id="4aee6-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4aee6-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4aee6-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="4aee6-124">Request body</span></span>
<span data-ttu-id="4aee6-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="4aee6-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4aee6-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4aee6-128">Property</span></span>     | <span data-ttu-id="4aee6-129">型</span><span class="sxs-lookup"><span data-stu-id="4aee6-129">Type</span></span>   |<span data-ttu-id="4aee6-130">説明</span><span class="sxs-lookup"><span data-stu-id="4aee6-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4aee6-131">displayName</span><span class="sxs-lookup"><span data-stu-id="4aee6-131">displayName</span></span>|<span data-ttu-id="4aee6-132">String</span><span class="sxs-lookup"><span data-stu-id="4aee6-132">String</span></span>|<span data-ttu-id="4aee6-133">mailFolder の表示名。</span><span class="sxs-lookup"><span data-stu-id="4aee6-133">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="4aee6-134">応答</span><span class="sxs-lookup"><span data-stu-id="4aee6-134">Response</span></span>

<span data-ttu-id="4aee6-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [mailFolder](../resources/mailfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4aee6-135">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4aee6-136">例</span><span class="sxs-lookup"><span data-stu-id="4aee6-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4aee6-137">要求</span><span class="sxs-lookup"><span data-stu-id="4aee6-137">Request</span></span>
<span data-ttu-id="4aee6-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4aee6-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_mailfolder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailFolders/{id}
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```
##### <a name="response"></a><span data-ttu-id="4aee6-139">応答</span><span class="sxs-lookup"><span data-stu-id="4aee6-139">Response</span></span>
<span data-ttu-id="4aee6-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4aee6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update mailfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
