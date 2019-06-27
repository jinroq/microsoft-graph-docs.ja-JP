---
title: 組織を更新する
description: 現在認証されている組織のプロパティを更新します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 08a7a2173208fbeaecd1b76b9b75f1e7678a1103
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265885"
---
# <a name="update-organization"></a><span data-ttu-id="de6ad-103">組織を更新する</span><span class="sxs-lookup"><span data-stu-id="de6ad-103">Update organization</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de6ad-104">現在認証されている組織のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="de6ad-104">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="de6ad-105">この例では`organization` 、は、1つのレコードのコレクションとして定義されているため、要求でその**ID**を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="de6ad-105">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="de6ad-106">**ID**は、組織の**tenantId**とも呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="de6ad-106">The **ID** is also known as the **tenantId** of the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="de6ad-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="de6ad-107">Permissions</span></span>

<span data-ttu-id="de6ad-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="de6ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de6ad-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="de6ad-110">Permission type</span></span> | <span data-ttu-id="de6ad-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="de6ad-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de6ad-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="de6ad-112">Delegated (work or school account)</span></span> | <span data-ttu-id="de6ad-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="de6ad-113">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="de6ad-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="de6ad-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de6ad-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de6ad-115">Not supported.</span></span> |
|<span data-ttu-id="de6ad-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="de6ad-116">Application</span></span> | <span data-ttu-id="de6ad-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de6ad-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="de6ad-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="de6ad-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}
```

## <a name="request-headers"></a><span data-ttu-id="de6ad-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="de6ad-119">Request headers</span></span>

| <span data-ttu-id="de6ad-120">名前</span><span class="sxs-lookup"><span data-stu-id="de6ad-120">Name</span></span>       | <span data-ttu-id="de6ad-121">型</span><span class="sxs-lookup"><span data-stu-id="de6ad-121">Type</span></span> | <span data-ttu-id="de6ad-122">説明</span><span class="sxs-lookup"><span data-stu-id="de6ad-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="de6ad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="de6ad-123">Authorization</span></span>  | <span data-ttu-id="de6ad-124">string</span><span class="sxs-lookup"><span data-stu-id="de6ad-124">string</span></span>  | <span data-ttu-id="de6ad-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="de6ad-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de6ad-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="de6ad-127">Request body</span></span>

<span data-ttu-id="de6ad-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="de6ad-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="de6ad-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de6ad-131">Property</span></span>     | <span data-ttu-id="de6ad-132">型</span><span class="sxs-lookup"><span data-stu-id="de6ad-132">Type</span></span>   |<span data-ttu-id="de6ad-133">説明</span><span class="sxs-lookup"><span data-stu-id="de6ad-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de6ad-134">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="de6ad-134">marketingNotificationEmails</span></span>|<span data-ttu-id="de6ad-135">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="de6ad-135">String collection</span></span>|                                        <span data-ttu-id="de6ad-136">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="de6ad-136">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="de6ad-137">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="de6ad-137">privacyProfile</span></span>|[<span data-ttu-id="de6ad-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="de6ad-138">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="de6ad-139">組織のプライバシー プロファイル (statementUrl と contactEmail を設定します)。</span><span class="sxs-lookup"><span data-stu-id="de6ad-139">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="de6ad-140">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="de6ad-140">securityComplianceNotificationMails</span></span>|<span data-ttu-id="de6ad-141">String collection</span><span class="sxs-lookup"><span data-stu-id="de6ad-141">String collection</span></span>||
|<span data-ttu-id="de6ad-142">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="de6ad-142">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="de6ad-143">String コレクション</span><span class="sxs-lookup"><span data-stu-id="de6ad-143">String collection</span></span>||
|<span data-ttu-id="de6ad-144">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="de6ad-144">technicalNotificationMails</span></span>|<span data-ttu-id="de6ad-145">String collection</span><span class="sxs-lookup"><span data-stu-id="de6ad-145">String collection</span></span>|                                        <span data-ttu-id="de6ad-146">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="de6ad-146">**Notes**: not nullable.</span></span>            |

<span data-ttu-id="de6ad-147">**組織**リソースが[拡張機能](/graph/extensibility-overview)をサポートしているため`PATCH` 、この操作を使用して、既存の**組織**インスタンスの拡張機能のカスタムプロパティで、独自のアプリ固有のデータを追加、更新、または削除できます。</span><span class="sxs-lookup"><span data-stu-id="de6ad-147">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **organization** instance.</span></span>

## <a name="response"></a><span data-ttu-id="de6ad-148">応答</span><span class="sxs-lookup"><span data-stu-id="de6ad-148">Response</span></span>

<span data-ttu-id="de6ad-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="de6ad-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de6ad-151">例</span><span class="sxs-lookup"><span data-stu-id="de6ad-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de6ad-152">要求</span><span class="sxs-lookup"><span data-stu-id="de6ad-152">Request</span></span>
<span data-ttu-id="de6ad-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="de6ad-153">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/{id}
Content-type: application/json
Content-length: 411

{
  "marketingNotificationEmails" : ["marketing@contoso.com"],
  "privacyProfile" :
    {
      "contactEmail":"alice@contoso.com",
      "statementUrl":"https://contoso.com/privacyStatement"
    },
  "securityComplianceNotificationMails" : ["security@contoso.com"],
  "securityComplianceNotificationPhones" : ["(123) 456-7890"],
  "technicalNotificationMails" : ["tech@contoso.com"]
}
```

##### <a name="response"></a><span data-ttu-id="de6ad-154">応答</span><span class="sxs-lookup"><span data-stu-id="de6ad-154">Response</span></span>

<span data-ttu-id="de6ad-155">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="de6ad-155">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="de6ad-156">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="de6ad-156">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="de6ad-157">C#</span><span class="sxs-lookup"><span data-stu-id="de6ad-157">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_organization-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de6ad-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="de6ad-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_organization-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="de6ad-159">目的-C</span><span class="sxs-lookup"><span data-stu-id="de6ad-159">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_organization-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="de6ad-160">関連項目</span><span class="sxs-lookup"><span data-stu-id="de6ad-160">See also</span></span>

- [<span data-ttu-id="de6ad-161">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="de6ad-161">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="de6ad-162">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="de6ad-162">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)

<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/organization-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/organization-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/organization-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
