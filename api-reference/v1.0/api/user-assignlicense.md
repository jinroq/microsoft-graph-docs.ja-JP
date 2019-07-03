---
title: assignLicense
description: ユーザーのサブスクリプションを追加または削除します。また、サブスクリプションに関連付けられている特定のプランを有効または無効にすることもできます。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fdabaee96cfae7ed85b575188c295a37db76a54c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460582"
---
# <a name="assignlicense"></a><span data-ttu-id="0a771-104">assignLicense</span><span class="sxs-lookup"><span data-stu-id="0a771-104">assignLicense</span></span>
<span data-ttu-id="0a771-p102">ユーザーのサブスクリプションを追加または削除します。また、サブスクリプションに関連付けられている特定のプランを有効または無効にすることもできます。</span><span class="sxs-lookup"><span data-stu-id="0a771-p102">Add or remove subscriptions for the user. You can also enable and disable specific plans associated with a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a771-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0a771-107">Permissions</span></span>
<span data-ttu-id="0a771-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0a771-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a771-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0a771-110">Permission type</span></span>      | <span data-ttu-id="0a771-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0a771-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a771-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0a771-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0a771-113">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a771-113">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="0a771-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0a771-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a771-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a771-115">Not supported.</span></span>    |
|<span data-ttu-id="0a771-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0a771-116">Application</span></span> | <span data-ttu-id="0a771-117">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a771-117">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a771-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0a771-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="0a771-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a771-119">Request headers</span></span>
| <span data-ttu-id="0a771-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a771-120">Header</span></span>       | <span data-ttu-id="0a771-121">値</span><span class="sxs-lookup"><span data-stu-id="0a771-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0a771-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a771-122">Authorization</span></span>  | <span data-ttu-id="0a771-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0a771-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0a771-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0a771-125">Content-Type</span></span>  | <span data-ttu-id="0a771-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0a771-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0a771-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0a771-127">Request body</span></span>
<span data-ttu-id="0a771-128">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="0a771-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0a771-129">パラメーター</span><span class="sxs-lookup"><span data-stu-id="0a771-129">Parameter</span></span>    | <span data-ttu-id="0a771-130">型</span><span class="sxs-lookup"><span data-stu-id="0a771-130">Type</span></span>   |<span data-ttu-id="0a771-131">説明</span><span class="sxs-lookup"><span data-stu-id="0a771-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a771-132">addLicenses</span><span class="sxs-lookup"><span data-stu-id="0a771-132">addLicenses</span></span>|<span data-ttu-id="0a771-133">AssignedLicense collection</span><span class="sxs-lookup"><span data-stu-id="0a771-133">AssignedLicense collection</span></span>|<span data-ttu-id="0a771-p105">追加するライセンスを指定する [assignedLicense](../resources/assignedlicense.md) オブジェクトのコレクションです。[assignedLicense](../resources/assignedlicense.md) オブジェクト上で **disabledPlans** プロパティを設定すると、ライセンスに関連付けられたプランを無効にできます。</span><span class="sxs-lookup"><span data-stu-id="0a771-p105">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add. You can disable plans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="0a771-136">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="0a771-136">removeLicenses</span></span>|<span data-ttu-id="0a771-137">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="0a771-137">Guid collection</span></span>|<span data-ttu-id="0a771-138">削除するライセンスを識別する GUID のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="0a771-138">A collection of GUIDs that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="0a771-139">応答</span><span class="sxs-lookup"><span data-stu-id="0a771-139">Response</span></span>

<span data-ttu-id="0a771-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[ユーザー](../resources/user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0a771-140">If successful, this method returns `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a771-141">例</span><span class="sxs-lookup"><span data-stu-id="0a771-141">Example</span></span>
<span data-ttu-id="0a771-142">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="0a771-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0a771-143">要求</span><span class="sxs-lookup"><span data-stu-id="0a771-143">Request</span></span>
<span data-ttu-id="0a771-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0a771-144">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0a771-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a771-145">--Http</span></span>](#tab/http)
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
      "skuId": "guid"
    }
  ],
  "removeLicenses": [ "bea13e0c-3828-4daa-a392-28af7ff61a0f" ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0a771-146">C#</span><span class="sxs-lookup"><span data-stu-id="0a771-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-assignlicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0a771-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="0a771-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-assignlicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0a771-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a771-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-assignlicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0a771-149">応答</span><span class="sxs-lookup"><span data-stu-id="0a771-149">Response</span></span>
<span data-ttu-id="0a771-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0a771-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "skuId": "0118A350-71FC-4EC3-8F0C-6A1CB8867561"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "2016-10-02T12:13:14Z",
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
