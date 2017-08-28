# <a name="assignlicense"></a><span data-ttu-id="7904c-101">assignLicense</span><span class="sxs-lookup"><span data-stu-id="7904c-101">assignLicense</span></span>
<span data-ttu-id="7904c-p101">ユーザーのサブスクリプションを追加または削除します。サブスクリプションに関連付けられている特定のプランを有効または無効にすることもできます。</span><span class="sxs-lookup"><span data-stu-id="7904c-p101">Add or remove subscriptions for the user. You can also enable and disable specific plans associated with a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="7904c-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7904c-104">Permissions</span></span>
<span data-ttu-id="7904c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7904c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7904c-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7904c-107">Permission type</span></span>      | <span data-ttu-id="7904c-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7904c-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7904c-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7904c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="7904c-110">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7904c-110">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="7904c-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7904c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7904c-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7904c-112">Not supported.</span></span>    |
|<span data-ttu-id="7904c-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7904c-113">Application</span></span> | <span data-ttu-id="7904c-114">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7904c-114">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7904c-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7904c-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="7904c-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7904c-116">Request headers</span></span>
| <span data-ttu-id="7904c-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7904c-117">Header</span></span>       | <span data-ttu-id="7904c-118">値</span><span class="sxs-lookup"><span data-stu-id="7904c-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7904c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="7904c-119">Authorization</span></span>  | <span data-ttu-id="7904c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7904c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7904c-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7904c-122">Content-Type</span></span>  | <span data-ttu-id="7904c-123">application/json</span><span class="sxs-lookup"><span data-stu-id="7904c-123">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7904c-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="7904c-124">Request body</span></span>
<span data-ttu-id="7904c-125">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="7904c-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7904c-126">パラメーター</span><span class="sxs-lookup"><span data-stu-id="7904c-126">Parameter</span></span>    | <span data-ttu-id="7904c-127">型</span><span class="sxs-lookup"><span data-stu-id="7904c-127">Type</span></span>   |<span data-ttu-id="7904c-128">説明</span><span class="sxs-lookup"><span data-stu-id="7904c-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7904c-129">addLicenses</span><span class="sxs-lookup"><span data-stu-id="7904c-129">addLicenses</span></span>|<span data-ttu-id="7904c-130">AssignedLicense</span><span class="sxs-lookup"><span data-stu-id="7904c-130">AssignedLicense</span></span>|<span data-ttu-id="7904c-p104">追加するライセンスを指定する [assignedLicense](../resources/assignedlicense.md) オブジェクトのコレクションです。[assignedLicense](../resources/assignedlicense.md) オブジェクト上で **disabledPlans** プロパティを設定すると、ライセンスに関連付けられたプランを無効にできます。</span><span class="sxs-lookup"><span data-stu-id="7904c-p104">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add. You can disable plans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="7904c-133">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="7904c-133">removeLicenses</span></span>|<span data-ttu-id="7904c-134">Guid</span><span class="sxs-lookup"><span data-stu-id="7904c-134">Guid</span></span>|<span data-ttu-id="7904c-135">削除するライセンスを識別する GUID のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="7904c-135">A collection of GUIDs that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="7904c-136">応答</span><span class="sxs-lookup"><span data-stu-id="7904c-136">Response</span></span>

<span data-ttu-id="7904c-137">成功した場合、このメソッドは `200, OK` 応答コードと、応答本文で[ユーザー](../resources/user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7904c-137">If successful, this method returns `200, OK` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7904c-138">例</span><span class="sxs-lookup"><span data-stu-id="7904c-138">Example</span></span>
<span data-ttu-id="7904c-139">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="7904c-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7904c-140">要求</span><span class="sxs-lookup"><span data-stu-id="7904c-140">Request</span></span>
<span data-ttu-id="7904c-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7904c-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_assignlicense"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value"
    }
  ],
  "removeLicenses": [ "bea13e0c-3828-4daa-a392-28af7ff61a0f" ]
}
```

##### <a name="response"></a><span data-ttu-id="7904c-142">応答</span><span class="sxs-lookup"><span data-stu-id="7904c-142">Response</span></span>
<span data-ttu-id="7904c-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7904c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "datetime-value",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
