---
title: 組織を更新する
description: 現在認証されている組織のプロパティを更新します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b627ca31c93a236d1b646b3b4ff958dad27864e5
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657288"
---
# <a name="update-organization"></a><span data-ttu-id="822ca-103">組織を更新する</span><span class="sxs-lookup"><span data-stu-id="822ca-103">Update organization</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="822ca-104">現在認証されている組織のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="822ca-104">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="822ca-105">この例では`organization` 、は、1つのレコードのコレクションとして定義されているため、要求でその**ID**を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="822ca-105">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="822ca-106">**ID**は、組織の**tenantId**とも呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="822ca-106">The **ID** is also known as the **tenantId** of the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="822ca-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="822ca-107">Permissions</span></span>

<span data-ttu-id="822ca-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="822ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="822ca-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="822ca-110">Permission type</span></span> | <span data-ttu-id="822ca-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="822ca-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="822ca-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="822ca-112">Delegated (work or school account)</span></span> | <span data-ttu-id="822ca-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="822ca-113">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="822ca-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="822ca-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="822ca-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="822ca-115">Not supported.</span></span> |
|<span data-ttu-id="822ca-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="822ca-116">Application</span></span> | <span data-ttu-id="822ca-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="822ca-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="822ca-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="822ca-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}
```

## <a name="request-headers"></a><span data-ttu-id="822ca-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="822ca-119">Request headers</span></span>

| <span data-ttu-id="822ca-120">名前</span><span class="sxs-lookup"><span data-stu-id="822ca-120">Name</span></span>       | <span data-ttu-id="822ca-121">型</span><span class="sxs-lookup"><span data-stu-id="822ca-121">Type</span></span> | <span data-ttu-id="822ca-122">説明</span><span class="sxs-lookup"><span data-stu-id="822ca-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="822ca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="822ca-123">Authorization</span></span>  | <span data-ttu-id="822ca-124">string</span><span class="sxs-lookup"><span data-stu-id="822ca-124">string</span></span>  | <span data-ttu-id="822ca-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="822ca-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="822ca-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="822ca-127">Request body</span></span>

<span data-ttu-id="822ca-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="822ca-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="822ca-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="822ca-131">Property</span></span>     | <span data-ttu-id="822ca-132">型</span><span class="sxs-lookup"><span data-stu-id="822ca-132">Type</span></span>   |<span data-ttu-id="822ca-133">説明</span><span class="sxs-lookup"><span data-stu-id="822ca-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="822ca-134">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="822ca-134">marketingNotificationEmails</span></span>|<span data-ttu-id="822ca-135">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="822ca-135">String collection</span></span>|                                        <span data-ttu-id="822ca-136">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="822ca-136">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="822ca-137">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="822ca-137">privacyProfile</span></span>|[<span data-ttu-id="822ca-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="822ca-138">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="822ca-139">組織のプライバシー プロファイル (statementUrl と contactEmail を設定します)。</span><span class="sxs-lookup"><span data-stu-id="822ca-139">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="822ca-140">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="822ca-140">securityComplianceNotificationMails</span></span>|<span data-ttu-id="822ca-141">String collection</span><span class="sxs-lookup"><span data-stu-id="822ca-141">String collection</span></span>||
|<span data-ttu-id="822ca-142">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="822ca-142">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="822ca-143">String コレクション</span><span class="sxs-lookup"><span data-stu-id="822ca-143">String collection</span></span>||
|<span data-ttu-id="822ca-144">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="822ca-144">technicalNotificationMails</span></span>|<span data-ttu-id="822ca-145">String collection</span><span class="sxs-lookup"><span data-stu-id="822ca-145">String collection</span></span>|                                        <span data-ttu-id="822ca-146">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="822ca-146">**Notes**: not nullable.</span></span>            |

<span data-ttu-id="822ca-147">**組織**リソースが[拡張機能](/graph/extensibility-overview)をサポートしているため`PATCH` 、この操作を使用して、既存の**組織**インスタンスの拡張機能のカスタムプロパティで、独自のアプリ固有のデータを追加、更新、または削除できます。</span><span class="sxs-lookup"><span data-stu-id="822ca-147">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **organization** instance.</span></span>

## <a name="response"></a><span data-ttu-id="822ca-148">応答</span><span class="sxs-lookup"><span data-stu-id="822ca-148">Response</span></span>

<span data-ttu-id="822ca-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="822ca-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="822ca-151">例</span><span class="sxs-lookup"><span data-stu-id="822ca-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="822ca-152">要求</span><span class="sxs-lookup"><span data-stu-id="822ca-152">Request</span></span>
<span data-ttu-id="822ca-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="822ca-153">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="822ca-154">応答</span><span class="sxs-lookup"><span data-stu-id="822ca-154">Response</span></span>

<span data-ttu-id="822ca-155">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="822ca-155">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="822ca-156">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="822ca-156">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="822ca-157">C#</span><span class="sxs-lookup"><span data-stu-id="822ca-157">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_organization-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="822ca-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="822ca-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_organization-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="822ca-159">関連項目</span><span class="sxs-lookup"><span data-stu-id="822ca-159">See also</span></span>

- [<span data-ttu-id="822ca-160">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="822ca-160">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="822ca-161">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="822ca-161">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)

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
    "Error: /api-reference/beta/api/organization-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/organization-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
