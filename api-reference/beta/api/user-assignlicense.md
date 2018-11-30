---
title: assignLicense
description: 追加またはユーザーを有効にするか、マイクロソフトのクラウド サービスの使用を無効にするためのライセンスを削除します。 たとえば、組織は、100 のライセンスを持つ、Office 365 エンタープライズ E3 サブスクリプションを持つことができ、この要求がこれらのライセンスのいずれかを特定のユーザーに割り当てます。 有効にし、サブスクリプションに関連付けられている特定のプランを無効にできます。 サブスクリプションとライセンスに関する詳細については、この Technet の記事を参照してください。
ms.openlocfilehash: ecfe1f97e2e951998e0a62eea68412279eae524f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074515"
---
# <a name="assignlicense"></a><span data-ttu-id="196c5-106">assignLicense</span><span class="sxs-lookup"><span data-stu-id="196c5-106">assignLicense</span></span>

> <span data-ttu-id="196c5-107">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="196c5-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="196c5-108">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="196c5-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="196c5-109">追加またはユーザーを有効にするか、マイクロソフトのクラウド サービスの使用を無効にするためのライセンスを削除します。</span><span class="sxs-lookup"><span data-stu-id="196c5-109">Add or remove licenses for the user to enable or disable their use of Microsoft cloud offerings.</span></span> <span data-ttu-id="196c5-110">たとえば、組織は、100 のライセンスを持つ、Office 365 エンタープライズ E3 サブスクリプションを持つことができ、この要求がこれらのライセンスのいずれかを特定のユーザーに割り当てます。</span><span class="sxs-lookup"><span data-stu-id="196c5-110">For example, an organization can have an Office 365 Enterprise E3 subscription with 100 licenses, and this request assigns one of those licenses to a specific user.</span></span> <span data-ttu-id="196c5-111">有効にし、サブスクリプションに関連付けられている特定のプランを無効にできます。</span><span class="sxs-lookup"><span data-stu-id="196c5-111">You can also enable and disable specific plans associated with a subscription.</span></span> <span data-ttu-id="196c5-112">サブスクリプションとライセンスに関する詳細については、この[Technet の記事](https://technet.microsoft.com/en-us/library/mt765146.aspx)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="196c5-112">To learn more about subscriptions and licenses, see this [Technet article](https://technet.microsoft.com/en-us/library/mt765146.aspx).</span></span>

<span data-ttu-id="196c5-113">ディレクトリで利用可能なサブスクリプションを取得するには、 [subscribedSkus 要求の取得](subscribedsku-list.md)を実行します。</span><span class="sxs-lookup"><span data-stu-id="196c5-113">To get the subscriptions available in the directory, perform a [GET subscribedSkus request](subscribedsku-list.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="196c5-114">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="196c5-114">Permissions</span></span>
<span data-ttu-id="196c5-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="196c5-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="196c5-117">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="196c5-117">Permission type</span></span>      | <span data-ttu-id="196c5-118">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="196c5-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="196c5-119">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="196c5-119">Delegated (work or school account)</span></span> | <span data-ttu-id="196c5-120">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="196c5-120">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="196c5-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="196c5-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="196c5-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="196c5-122">Not supported.</span></span>    |
|<span data-ttu-id="196c5-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="196c5-123">Application</span></span> | <span data-ttu-id="196c5-124">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="196c5-124">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="196c5-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="196c5-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="196c5-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="196c5-126">Request headers</span></span>
| <span data-ttu-id="196c5-127">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="196c5-127">Header</span></span>       | <span data-ttu-id="196c5-128">値</span><span class="sxs-lookup"><span data-stu-id="196c5-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="196c5-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="196c5-129">Authorization</span></span>  | <span data-ttu-id="196c5-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="196c5-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="196c5-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="196c5-132">Content-Type</span></span>  | <span data-ttu-id="196c5-133">application/json</span><span class="sxs-lookup"><span data-stu-id="196c5-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="196c5-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="196c5-134">Request body</span></span>
<span data-ttu-id="196c5-135">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="196c5-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="196c5-136">パラメーター</span><span class="sxs-lookup"><span data-stu-id="196c5-136">Parameter</span></span>    | <span data-ttu-id="196c5-137">型</span><span class="sxs-lookup"><span data-stu-id="196c5-137">Type</span></span>   |<span data-ttu-id="196c5-138">説明</span><span class="sxs-lookup"><span data-stu-id="196c5-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="196c5-139">addLicenses</span><span class="sxs-lookup"><span data-stu-id="196c5-139">addLicenses</span></span>|<span data-ttu-id="196c5-140">[assignedLicense](../resources/assignedlicense.md) collection</span><span class="sxs-lookup"><span data-stu-id="196c5-140">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="196c5-141">追加するのにはライセンスを指定する[assignedLicense](../resources/assignedlicense.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="196c5-141">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add.</span></span> <span data-ttu-id="196c5-142">[AssignedLicense](../resources/assignedlicense.md)オブジェクトの**disabledPlans**プロパティを設定することにより、ライセンスに関連する servicePlans を無効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="196c5-142">You can disable servicePlans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="196c5-143">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="196c5-143">removeLicenses</span></span>|<span data-ttu-id="196c5-144">Guid</span><span class="sxs-lookup"><span data-stu-id="196c5-144">Guid</span></span>|<span data-ttu-id="196c5-145">削除するライセンスを識別する skuIds のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="196c5-145">A collection of skuIds that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="196c5-146">応答</span><span class="sxs-lookup"><span data-stu-id="196c5-146">Response</span></span>

<span data-ttu-id="196c5-147">かどうかは成功すると、このメソッドを返します`200 OK`応答コードおよび応答の本体の更新された[ユーザー](../resources/user.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="196c5-147">If successful, this method returns `200 OK` response code and an updated [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="196c5-148">使用例</span><span class="sxs-lookup"><span data-stu-id="196c5-148">Example</span></span>
<span data-ttu-id="196c5-149">ユーザーにライセンスを追加します。</span><span class="sxs-lookup"><span data-stu-id="196c5-149">Add licenses to the user.</span></span>
##### <a name="request"></a><span data-ttu-id="196c5-150">要求</span><span class="sxs-lookup"><span data-stu-id="196c5-150">Request</span></span>
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

## <a name="example"></a><span data-ttu-id="196c5-151">使用例</span><span class="sxs-lookup"><span data-stu-id="196c5-151">Example</span></span>
<span data-ttu-id="196c5-152">ユーザーからライセンスを削除します。</span><span class="sxs-lookup"><span data-stu-id="196c5-152">Remove licenses from the user.</span></span>

#####<a name="request"></a><span data-ttu-id="196c5-153">要求</span><span class="sxs-lookup"><span data-stu-id="196c5-153">Request</span></span>
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [],
  "removeLicenses": ["skuId-value-1", "skuId-value-2"]
}
```

##### <a name="response"></a><span data-ttu-id="196c5-154">応答</span><span class="sxs-lookup"><span data-stu-id="196c5-154">Response</span></span>
<span data-ttu-id="196c5-155">どちらの例では、応答は、更新されたユーザー オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="196c5-155">In both examples, the response is the updated user object.</span></span> <span data-ttu-id="196c5-156">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="196c5-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="196c5-157">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="196c5-157">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "user: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
