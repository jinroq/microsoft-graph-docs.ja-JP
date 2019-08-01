---
title: secureScoreControlProfiles の更新
description: 任意の統合ソリューション内の編集可能な secureScoreControlProfile オブジェクトを更新して、担当者や tenantNote などのさまざまなプロパティを変更します。
author: preetikr
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: aa8998dd720a19e744b68dbaa5bac4522662d3f4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36024715"
---
# <a name="update-securescorecontrolprofile"></a><span data-ttu-id="20f08-103">secureScoreControlProfiles の更新</span><span class="sxs-lookup"><span data-stu-id="20f08-103">Update secureScoreControlProfile</span></span>

<span data-ttu-id="20f08-104">任意の統合ソリューション内の編集可能な**secureScoreControlProfile**オブジェクトを更新して、 \*\*\*\* 担当者や**tenantnote**などのさまざまなプロパティを変更します。</span><span class="sxs-lookup"><span data-stu-id="20f08-104">Update an editable **secureScoreControlProfile** object within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="20f08-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="20f08-105">Permissions</span></span>

<span data-ttu-id="20f08-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="20f08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20f08-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="20f08-108">Permission type</span></span>      | <span data-ttu-id="20f08-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="20f08-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20f08-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="20f08-110">Delegated (work or school account)</span></span> |   <span data-ttu-id="20f08-111">SecurityEvents。</span><span class="sxs-lookup"><span data-stu-id="20f08-111">SecurityEvents.ReadWrite.All.</span></span>  |
|<span data-ttu-id="20f08-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="20f08-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="20f08-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20f08-113">Not supported.</span></span>  |
|<span data-ttu-id="20f08-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="20f08-114">Application</span></span> | <span data-ttu-id="20f08-115">SecurityEvents。</span><span class="sxs-lookup"><span data-stu-id="20f08-115">SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="20f08-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="20f08-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="20f08-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="20f08-117">Request headers</span></span>

| <span data-ttu-id="20f08-118">名前</span><span class="sxs-lookup"><span data-stu-id="20f08-118">Name</span></span>       | <span data-ttu-id="20f08-119">説明</span><span class="sxs-lookup"><span data-stu-id="20f08-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="20f08-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="20f08-120">Authorization</span></span>  | <span data-ttu-id="20f08-121">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="20f08-121">Bearer {code}.</span></span> <span data-ttu-id="20f08-122">必須です。</span><span class="sxs-lookup"><span data-stu-id="20f08-122">Required.</span></span>|
|<span data-ttu-id="20f08-123">Prefer</span><span class="sxs-lookup"><span data-stu-id="20f08-123">Prefer</span></span> | <span data-ttu-id="20f08-124">戻り値 = 表現。</span><span class="sxs-lookup"><span data-stu-id="20f08-124">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20f08-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="20f08-125">Request body</span></span>

<span data-ttu-id="20f08-126">要求本文で、更新する必要のある関連フィールドの値の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="20f08-126">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="20f08-127">本文には、有効`vendorInformation`な`provider` `vendor`フィールドとフィールドのプロパティが含まれて**いる必要があり**ます。</span><span class="sxs-lookup"><span data-stu-id="20f08-127">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="20f08-128">次の表に、 **secureScoreControlProfile**で更新できるフィールドを示します。</span><span class="sxs-lookup"><span data-stu-id="20f08-128">The following table lists the fields that can be updated for a **secureScoreControlProfile**.</span></span> <span data-ttu-id="20f08-129">要求本文に含まれていない既存のプロパティの値は変更されません。</span><span class="sxs-lookup"><span data-stu-id="20f08-129">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="20f08-130">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="20f08-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="20f08-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="20f08-131">Property</span></span>   | <span data-ttu-id="20f08-132">型</span><span class="sxs-lookup"><span data-stu-id="20f08-132">Type</span></span> |<span data-ttu-id="20f08-133">説明</span><span class="sxs-lookup"><span data-stu-id="20f08-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20f08-134">assignedTo</span><span class="sxs-lookup"><span data-stu-id="20f08-134">assignedTo</span></span>|<span data-ttu-id="20f08-135">String</span><span class="sxs-lookup"><span data-stu-id="20f08-135">String</span></span>|<span data-ttu-id="20f08-136">トリアージ、実装、または修復のために、コントロールが割り当てられているアナリストの名前。</span><span class="sxs-lookup"><span data-stu-id="20f08-136">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="20f08-137">comment</span><span class="sxs-lookup"><span data-stu-id="20f08-137">comment</span></span>|<span data-ttu-id="20f08-138">String</span><span class="sxs-lookup"><span data-stu-id="20f08-138">String</span></span>|<span data-ttu-id="20f08-139">コントロールに関するアナリストコメント (カスタマーコントロール管理向け)。</span><span class="sxs-lookup"><span data-stu-id="20f08-139">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="20f08-140">state</span><span class="sxs-lookup"><span data-stu-id="20f08-140">state</span></span>| <span data-ttu-id="20f08-141">String</span><span class="sxs-lookup"><span data-stu-id="20f08-141">String</span></span>|<span data-ttu-id="20f08-142">コントロールに対するアナリスト主導の設定。</span><span class="sxs-lookup"><span data-stu-id="20f08-142">Analyst driven setting on the control.</span></span> <span data-ttu-id="20f08-143">使用可能な値は、`Default`、`Ignored`、`ThirdParty`、`Reviewed` です。</span><span class="sxs-lookup"><span data-stu-id="20f08-143">Possible values are: `Default`, `Ignored`, `ThirdParty`, `Reviewed`.</span></span>|
| <span data-ttu-id="20f08-144">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="20f08-144">vendorInformation</span></span> | [<span data-ttu-id="20f08-145">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="20f08-145">securityVendorInformation</span></span>](../resources/securityvendorinformation.md) | <span data-ttu-id="20f08-146">セキュリティ製品/サービスベンダー、プロバイダ、およびサブプロバイダに関する詳細を含む複合型 (たとえば、vendor = Microsoft; provider = SecureScore;)。</span><span class="sxs-lookup"><span data-stu-id="20f08-146">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore;).</span></span> <span data-ttu-id="20f08-147">**プロバイダーおよびベンダーフィールドは必須です。**</span><span class="sxs-lookup"><span data-stu-id="20f08-147">**Provider and vendor fields are required.**</span></span> |


## <a name="response"></a><span data-ttu-id="20f08-148">応答</span><span class="sxs-lookup"><span data-stu-id="20f08-148">Response</span></span>

<span data-ttu-id="20f08-149">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="20f08-149">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="20f08-150">オプションの要求ヘッダーが使用されている場合、 `200 OK`メソッドは応答コードと、応答本文で更新された[securescorecontrolprofiles の](../resources/securescorecontrolprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="20f08-150">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20f08-151">例</span><span class="sxs-lookup"><span data-stu-id="20f08-151">Example</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="20f08-152">例 1: 希望するヘッダーのない要求</span><span class="sxs-lookup"><span data-stu-id="20f08-152">Example 1: Request without Prefer header</span></span>

### <a name="request"></a><span data-ttu-id="20f08-153">要求</span><span class="sxs-lookup"><span data-stu-id="20f08-153">Request</span></span>

<span data-ttu-id="20f08-154">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="20f08-154">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="20f08-155">プロトコル</span><span class="sxs-lookup"><span data-stu-id="20f08-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles/NonOwnerAccess
Content-type: application/json

{
  "assignedTo": "",
  "comment": "control is reviewed",
  "state": "Reviewed",
  "vendorInformation": {

    "provider": "SecureScore",
    "providerVersion": null,
    "subProvider": null,
    "vendor": "Microsoft"
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="20f08-156">C#</span><span class="sxs-lookup"><span data-stu-id="20f08-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-update-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="20f08-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="20f08-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-update-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="20f08-158">目的-C</span><span class="sxs-lookup"><span data-stu-id="20f08-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-update-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="20f08-159">Java</span><span class="sxs-lookup"><span data-stu-id="20f08-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/securescorecontrolprofiles-update-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="20f08-160">応答</span><span class="sxs-lookup"><span data-stu-id="20f08-160">Response</span></span>

<span data-ttu-id="20f08-161">成功応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="20f08-161">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="20f08-162">例 2: 要求ヘッダーを使用した要求</span><span class="sxs-lookup"><span data-stu-id="20f08-162">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="20f08-163">要求</span><span class="sxs-lookup"><span data-stu-id="20f08-163">Request</span></span>

<span data-ttu-id="20f08-164">次の例は、 `Prefer`要求ヘッダーを含む要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="20f08-164">The following example shows a request that includes the `Prefer` request header.</span></span>

<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles/NonOwnerAccess
Content-type: application/json

{
  "assignedTo": "",
  "comment": "control is reviewed",
  "state": "Reviewed",
  "vendorInformation": {
    "provider": "SecureScore",
    "providerVersion": null,
    "subProvider": null,
    "vendor": "Microsoft"
  }
}
```

#### <a name="response"></a><span data-ttu-id="20f08-165">応答</span><span class="sxs-lookup"><span data-stu-id="20f08-165">Response</span></span>

<span data-ttu-id="20f08-166">オプション`Prefer: return=representation`の要求ヘッダーを使用する場合の応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="20f08-166">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

> <span data-ttu-id="20f08-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="20f08-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "NonOwnerAccess",
  "azureTenantId": "00000001-0001-0001-0001-000000000001c",
  "actionType": "Review",
  "actionUrl": "https://outlook.office365.com/NonOwnerAccessReport.aspx",
  "controlCategory": "Data",
  "title": "Review mailbox access by non-owners bi-weekly", 
  "deprecated": false,
  "implementationCost": "Low",
  "lastModifiedDateTime": null,
  "maxScore": 5.0,
  "rank": 25,
  "remediation": "Once you have opened the search tool, specify a date range and select access by <b>All non-owners</b> or <b>External users</b>",
  "remediationImpact": "This change will have no effect on your users",
  "service": "EXO",
  "threats": [
    "Account Breach",
    "Data Exfiltration",
    "Malicious Insider"
  ],
  "tier": "Core",
  "userImpact": "Low",
  "complianceInformation": [
    {
      "certificationName": "FedRAMP_Moderate",
      "certificationControls": [
        {
          "name": "AC-6(9)",
          "url": "",
        }
      ]
    }         
  ],
  "controlStateUpdates": [
    {
      "assignedTo": "",
      "comment": "control is reviewed",
      "state": "Reviewed",
      "updatedBy": "user1@contoso.com",
      "updatedDateTime": "2019-03-19T22:37:14.628799Z"
    }
  ],
  "vendorInformation": {
    "provider": "SecureScore",
    "providerVersion": null,
    "subProvider": null,
    "vendor": "Microsoft"
  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
