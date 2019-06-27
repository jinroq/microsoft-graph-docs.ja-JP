---
title: secureScoreControlProfiles の更新
description: 任意の統合ソリューション内の編集可能な secureScoreControlProfile オブジェクトを更新して、担当者や tenantNote などのさまざまなプロパティを変更します。
author: preetikr
localization_priority: Normal
ms.openlocfilehash: f4239cb769277ea7e75e30c8dd3807cd481213bb
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35279297"
---
# <a name="update-securescorecontrolprofile"></a><span data-ttu-id="0d33b-103">secureScoreControlProfiles の更新</span><span class="sxs-lookup"><span data-stu-id="0d33b-103">Update secureScoreControlProfile</span></span>

<span data-ttu-id="0d33b-104">任意の統合ソリューション内の編集可能な**secureScoreControlProfile**オブジェクトを更新して、 \*\*\*\* 担当者や**tenantnote**などのさまざまなプロパティを変更します。</span><span class="sxs-lookup"><span data-stu-id="0d33b-104">Update an editable **secureScoreControlProfile** object within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d33b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0d33b-105">Permissions</span></span>

<span data-ttu-id="0d33b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0d33b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d33b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0d33b-108">Permission type</span></span>      | <span data-ttu-id="0d33b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0d33b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d33b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0d33b-110">Delegated (work or school account)</span></span> |   <span data-ttu-id="0d33b-111">SecurityEvents。</span><span class="sxs-lookup"><span data-stu-id="0d33b-111">SecurityEvents.ReadWrite.All.</span></span>  |
|<span data-ttu-id="0d33b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0d33b-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0d33b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d33b-113">Not supported.</span></span>  |
|<span data-ttu-id="0d33b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0d33b-114">Application</span></span> | <span data-ttu-id="0d33b-115">SecurityEvents。</span><span class="sxs-lookup"><span data-stu-id="0d33b-115">SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d33b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0d33b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0d33b-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0d33b-117">Request headers</span></span>

| <span data-ttu-id="0d33b-118">名前</span><span class="sxs-lookup"><span data-stu-id="0d33b-118">Name</span></span>       | <span data-ttu-id="0d33b-119">説明</span><span class="sxs-lookup"><span data-stu-id="0d33b-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0d33b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d33b-120">Authorization</span></span>  | <span data-ttu-id="0d33b-121">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="0d33b-121">Bearer {code}.</span></span> <span data-ttu-id="0d33b-122">必須です。</span><span class="sxs-lookup"><span data-stu-id="0d33b-122">Required.</span></span>|
|<span data-ttu-id="0d33b-123">Prefer</span><span class="sxs-lookup"><span data-stu-id="0d33b-123">Prefer</span></span> | <span data-ttu-id="0d33b-124">戻り値 = 表現。</span><span class="sxs-lookup"><span data-stu-id="0d33b-124">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d33b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="0d33b-125">Request body</span></span>

<span data-ttu-id="0d33b-126">要求本文で、更新する必要のある関連フィールドの値の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0d33b-126">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0d33b-127">本文には、有効`vendorInformation`な`provider` `vendor`フィールドとフィールドのプロパティが含まれて**いる必要があり**ます。</span><span class="sxs-lookup"><span data-stu-id="0d33b-127">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="0d33b-128">次の表に、 **secureScoreControlProfile**で更新できるフィールドを示します。</span><span class="sxs-lookup"><span data-stu-id="0d33b-128">The following table lists the fields that can be updated for a **secureScoreControlProfile**.</span></span> <span data-ttu-id="0d33b-129">要求本文に含まれていない既存のプロパティの値は変更されません。</span><span class="sxs-lookup"><span data-stu-id="0d33b-129">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="0d33b-130">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="0d33b-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0d33b-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d33b-131">Property</span></span>   | <span data-ttu-id="0d33b-132">型</span><span class="sxs-lookup"><span data-stu-id="0d33b-132">Type</span></span> |<span data-ttu-id="0d33b-133">説明</span><span class="sxs-lookup"><span data-stu-id="0d33b-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d33b-134">assignedTo</span><span class="sxs-lookup"><span data-stu-id="0d33b-134">assignedTo</span></span>|<span data-ttu-id="0d33b-135">String</span><span class="sxs-lookup"><span data-stu-id="0d33b-135">String</span></span>|<span data-ttu-id="0d33b-136">トリアージ、実装、または修復のために、コントロールが割り当てられているアナリストの名前。</span><span class="sxs-lookup"><span data-stu-id="0d33b-136">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="0d33b-137">comment</span><span class="sxs-lookup"><span data-stu-id="0d33b-137">comment</span></span>|<span data-ttu-id="0d33b-138">String</span><span class="sxs-lookup"><span data-stu-id="0d33b-138">String</span></span>|<span data-ttu-id="0d33b-139">コントロールに関するアナリストコメント (カスタマーコントロール管理向け)。</span><span class="sxs-lookup"><span data-stu-id="0d33b-139">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="0d33b-140">state</span><span class="sxs-lookup"><span data-stu-id="0d33b-140">state</span></span>| <span data-ttu-id="0d33b-141">String</span><span class="sxs-lookup"><span data-stu-id="0d33b-141">String</span></span>|<span data-ttu-id="0d33b-142">コントロールに対するアナリスト主導の設定。</span><span class="sxs-lookup"><span data-stu-id="0d33b-142">Analyst driven setting on the control.</span></span> <span data-ttu-id="0d33b-143">使用可能な値は、`Default`、`Ignored`、`ThirdParty`、`Reviewed` です。</span><span class="sxs-lookup"><span data-stu-id="0d33b-143">Possible values are: `Default`, `Ignored`, `ThirdParty`, `Reviewed`.</span></span>|
| <span data-ttu-id="0d33b-144">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="0d33b-144">vendorInformation</span></span> | [<span data-ttu-id="0d33b-145">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="0d33b-145">securityVendorInformation</span></span>](../resources/securityvendorinformation.md) | <span data-ttu-id="0d33b-146">セキュリティ製品/サービスベンダー、プロバイダ、およびサブプロバイダに関する詳細を含む複合型 (たとえば、vendor = Microsoft; provider = SecureScore;)。</span><span class="sxs-lookup"><span data-stu-id="0d33b-146">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore;).</span></span> <span data-ttu-id="0d33b-147">**プロバイダーおよびベンダーフィールドは必須です。**</span><span class="sxs-lookup"><span data-stu-id="0d33b-147">**Provider and vendor fields are required.**</span></span> |


## <a name="response"></a><span data-ttu-id="0d33b-148">応答</span><span class="sxs-lookup"><span data-stu-id="0d33b-148">Response</span></span>

<span data-ttu-id="0d33b-149">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="0d33b-149">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="0d33b-150">オプションの要求ヘッダーが使用されている場合、 `200 OK`メソッドは応答コードと、応答本文で更新された[securescorecontrolprofiles の](../resources/securescorecontrolprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0d33b-150">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d33b-151">例</span><span class="sxs-lookup"><span data-stu-id="0d33b-151">Example</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="0d33b-152">例 1: 希望するヘッダーのない要求</span><span class="sxs-lookup"><span data-stu-id="0d33b-152">Example 1: Request without Prefer header</span></span>

### <a name="request"></a><span data-ttu-id="0d33b-153">要求</span><span class="sxs-lookup"><span data-stu-id="0d33b-153">Request</span></span>

<span data-ttu-id="0d33b-154">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0d33b-154">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0d33b-155">応答</span><span class="sxs-lookup"><span data-stu-id="0d33b-155">Response</span></span>

<span data-ttu-id="0d33b-156">成功応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0d33b-156">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0d33b-157">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="0d33b-157">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0d33b-158">C#</span><span class="sxs-lookup"><span data-stu-id="0d33b-158">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/securescorecontrolprofiles_update-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0d33b-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="0d33b-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/securescorecontrolprofiles_update-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0d33b-160">目的-C</span><span class="sxs-lookup"><span data-stu-id="0d33b-160">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/securescorecontrolprofiles_update-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="0d33b-161">例 2: 要求ヘッダーを使用した要求</span><span class="sxs-lookup"><span data-stu-id="0d33b-161">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="0d33b-162">要求</span><span class="sxs-lookup"><span data-stu-id="0d33b-162">Request</span></span>

<span data-ttu-id="0d33b-163">次の例は、 `Prefer`要求ヘッダーを含む要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="0d33b-163">The following example shows a request that includes the `Prefer` request header.</span></span>

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

#### <a name="response"></a><span data-ttu-id="0d33b-164">応答</span><span class="sxs-lookup"><span data-stu-id="0d33b-164">Response</span></span>

<span data-ttu-id="0d33b-165">オプション`Prefer: return=representation`の要求ヘッダーを使用する場合の応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0d33b-165">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

> <span data-ttu-id="0d33b-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0d33b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "Error: /api-reference/v1.0/api/securescorecontrolprofile-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/securescorecontrolprofile-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/securescorecontrolprofile-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
