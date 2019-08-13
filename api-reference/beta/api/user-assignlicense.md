---
title: assignLicense
description: ユーザーのライセンスを追加または削除して、Microsoft クラウド製品の使用を有効または無効にします。 たとえば、組織には100ライセンスを持つ Office 365 Enterprise E3 サブスクリプションがあり、この要求はそれらのライセンスの1つを特定のユーザーに割り当てます。 また、サブスクリプションに関連付けられている特定のプランを有効または無効にすることもできます。 サブスクリプションとライセンスの詳細については、Technet の記事を参照してください。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 085c81ab4daeeca794081087584e514cb7f5517b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362574"
---
# <a name="assignlicense"></a><span data-ttu-id="0fcdb-106">assignLicense</span><span class="sxs-lookup"><span data-stu-id="0fcdb-106">assignLicense</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fcdb-107">ユーザーのライセンスを追加または削除して、Microsoft クラウド製品の使用を有効または無効にします。</span><span class="sxs-lookup"><span data-stu-id="0fcdb-107">Add or remove licenses for the user to enable or disable their use of Microsoft cloud offerings.</span></span> <span data-ttu-id="0fcdb-108">たとえば、組織には100ライセンスを持つ Office 365 Enterprise E3 サブスクリプションがあり、この要求はそれらのライセンスの1つを特定のユーザーに割り当てます。</span><span class="sxs-lookup"><span data-stu-id="0fcdb-108">For example, an organization can have an Office 365 Enterprise E3 subscription with 100 licenses, and this request assigns one of those licenses to a specific user.</span></span> <span data-ttu-id="0fcdb-109">また、サブスクリプションに関連付けられている特定のプランを有効または無効にすることもできます。</span><span class="sxs-lookup"><span data-stu-id="0fcdb-109">You can also enable and disable specific plans associated with a subscription.</span></span> <span data-ttu-id="0fcdb-110">サブスクリプションとライセンスの詳細については、 [Technet の記事](https://technet.microsoft.com/en-us/library/mt765146.aspx)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0fcdb-110">To learn more about subscriptions and licenses, see this [Technet article](https://technet.microsoft.com/en-us/library/mt765146.aspx).</span></span>

<span data-ttu-id="0fcdb-111">ディレクトリで利用可能なサブスクリプションを取得するには、 [Get subscribedSkus 要求](subscribedsku-list.md)を実行します。</span><span class="sxs-lookup"><span data-stu-id="0fcdb-111">To get the subscriptions available in the directory, perform a [GET subscribedSkus request](subscribedsku-list.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="0fcdb-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0fcdb-112">Permissions</span></span>
<span data-ttu-id="0fcdb-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0fcdb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fcdb-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0fcdb-115">Permission type</span></span>      | <span data-ttu-id="0fcdb-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0fcdb-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0fcdb-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0fcdb-117">Delegated (work or school account)</span></span> | <span data-ttu-id="0fcdb-118">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fcdb-118">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="0fcdb-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0fcdb-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fcdb-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0fcdb-120">Not supported.</span></span>    |
|<span data-ttu-id="0fcdb-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0fcdb-121">Application</span></span> | <span data-ttu-id="0fcdb-122">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fcdb-122">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fcdb-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0fcdb-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="0fcdb-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0fcdb-124">Request headers</span></span>
| <span data-ttu-id="0fcdb-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0fcdb-125">Header</span></span>       | <span data-ttu-id="0fcdb-126">値</span><span class="sxs-lookup"><span data-stu-id="0fcdb-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0fcdb-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fcdb-127">Authorization</span></span>  | <span data-ttu-id="0fcdb-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0fcdb-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0fcdb-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0fcdb-130">Content-Type</span></span>  | <span data-ttu-id="0fcdb-131">application/json</span><span class="sxs-lookup"><span data-stu-id="0fcdb-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0fcdb-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="0fcdb-132">Request body</span></span>
<span data-ttu-id="0fcdb-133">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="0fcdb-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0fcdb-134">パラメーター</span><span class="sxs-lookup"><span data-stu-id="0fcdb-134">Parameter</span></span>    | <span data-ttu-id="0fcdb-135">型</span><span class="sxs-lookup"><span data-stu-id="0fcdb-135">Type</span></span>   |<span data-ttu-id="0fcdb-136">説明</span><span class="sxs-lookup"><span data-stu-id="0fcdb-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0fcdb-137">addLicenses</span><span class="sxs-lookup"><span data-stu-id="0fcdb-137">addLicenses</span></span>|<span data-ttu-id="0fcdb-138">[assignedLicense](../resources/assignedlicense.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0fcdb-138">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="0fcdb-139">追加するライセンスを指定する[assignedLicense](../resources/assignedlicense.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="0fcdb-139">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add.</span></span> <span data-ttu-id="0fcdb-140">[AssignedLicense](../resources/assignedlicense.md)オブジェクトの**disabledPlans**プロパティを設定することによって、ライセンスに関連付けられた serviceplans を無効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0fcdb-140">You can disable servicePlans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="0fcdb-141">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="0fcdb-141">removeLicenses</span></span>|<span data-ttu-id="0fcdb-142">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="0fcdb-142">Guid collection</span></span>|<span data-ttu-id="0fcdb-143">削除するライセンスを識別する skuIds のコレクション。</span><span class="sxs-lookup"><span data-stu-id="0fcdb-143">A collection of skuIds that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="0fcdb-144">応答</span><span class="sxs-lookup"><span data-stu-id="0fcdb-144">Response</span></span>

<span data-ttu-id="0fcdb-145">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で更新された[ユーザー](../resources/user.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0fcdb-145">If successful, this method returns `200 OK` response code and an updated [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fcdb-146">例</span><span class="sxs-lookup"><span data-stu-id="0fcdb-146">Example</span></span>
<span data-ttu-id="0fcdb-147">ユーザーにライセンスを追加します。</span><span class="sxs-lookup"><span data-stu-id="0fcdb-147">Add licenses to the user.</span></span>
##### <a name="request"></a><span data-ttu-id="0fcdb-148">要求</span><span class="sxs-lookup"><span data-stu-id="0fcdb-148">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0fcdb-149">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0fcdb-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_assignlicense"
}-->
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value-1"
    },
    {
      "disabledPlans": [ "a571ebcc-fqe0-4ca2-8c8c-7a284fd6c235" ],
      "skuId": "skuId-value-2"
    }
  ],
  "removeLicenses": []
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0fcdb-150">C#</span><span class="sxs-lookup"><span data-stu-id="0fcdb-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-assignlicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0fcdb-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0fcdb-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-assignlicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0fcdb-152">目的-C</span><span class="sxs-lookup"><span data-stu-id="0fcdb-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-assignlicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0fcdb-153">Java</span><span class="sxs-lookup"><span data-stu-id="0fcdb-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-assignlicense-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="example"></a><span data-ttu-id="0fcdb-154">例</span><span class="sxs-lookup"><span data-stu-id="0fcdb-154">Example</span></span>
<span data-ttu-id="0fcdb-155">ユーザーからライセンスを削除します。</span><span class="sxs-lookup"><span data-stu-id="0fcdb-155">Remove licenses from the user.</span></span>

##### <a name="request"></a><span data-ttu-id="0fcdb-156">要求</span><span class="sxs-lookup"><span data-stu-id="0fcdb-156">Request</span></span>
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [],
  "removeLicenses": ["skuId-value-1", "skuId-value-2"]
}
```

##### <a name="response"></a><span data-ttu-id="0fcdb-157">応答</span><span class="sxs-lookup"><span data-stu-id="0fcdb-157">Response</span></span>
<span data-ttu-id="0fcdb-158">どちらの例でも、応答は更新されたユーザーオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="0fcdb-158">In both examples, the response is the updated user object.</span></span> <span data-ttu-id="0fcdb-159">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="0fcdb-159">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0fcdb-160">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0fcdb-160">All of the properties will be returned from an actual call.</span></span>
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
      "assignedDateTime": "2016-10-19T10:37:00Z",
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
<!--
{
  "type": "#page.annotation",
  "description": "user: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
