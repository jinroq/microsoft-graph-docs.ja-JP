---
title: 組織を更新する
description: 現在認証されている組織のプロパティを更新します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 69c1467aed702918692b8e354ad661a949ca2638
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414358"
---
# <a name="update-organization"></a><span data-ttu-id="de968-103">組織を更新する</span><span class="sxs-lookup"><span data-stu-id="de968-103">Update organization</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de968-104">現在認証されている組織のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="de968-104">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="de968-105">この例では`organization` 、は、1つのレコードのコレクションとして定義されているため、要求でその**ID**を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="de968-105">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="de968-106">**ID**は、組織の**tenantId**とも呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="de968-106">The **ID** is also known as the **tenantId** of the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="de968-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="de968-107">Permissions</span></span>

<span data-ttu-id="de968-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="de968-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de968-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="de968-110">Permission type</span></span> | <span data-ttu-id="de968-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="de968-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de968-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="de968-112">Delegated (work or school account)</span></span> | <span data-ttu-id="de968-113">Directory.accessasuser.all、すべてのディレクトリを示します。</span><span class="sxs-lookup"><span data-stu-id="de968-113">Organization.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="de968-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="de968-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de968-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de968-115">Not supported.</span></span> |
|<span data-ttu-id="de968-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="de968-116">Application</span></span> | <span data-ttu-id="de968-117">組織の ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de968-117">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="de968-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="de968-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}
```

## <a name="request-headers"></a><span data-ttu-id="de968-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="de968-119">Request headers</span></span>

| <span data-ttu-id="de968-120">名前</span><span class="sxs-lookup"><span data-stu-id="de968-120">Name</span></span>       | <span data-ttu-id="de968-121">説明</span><span class="sxs-lookup"><span data-stu-id="de968-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="de968-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="de968-122">Authorization</span></span>  | <span data-ttu-id="de968-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="de968-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="de968-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="de968-125">Content-Type</span></span>   | <span data-ttu-id="de968-126">application/json</span><span class="sxs-lookup"><span data-stu-id="de968-126">application/json</span></span> |


## <a name="request-body"></a><span data-ttu-id="de968-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="de968-127">Request body</span></span>

<span data-ttu-id="de968-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="de968-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="de968-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de968-131">Property</span></span>  | <span data-ttu-id="de968-132">型</span><span class="sxs-lookup"><span data-stu-id="de968-132">Type</span></span> |<span data-ttu-id="de968-133">説明</span><span class="sxs-lookup"><span data-stu-id="de968-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de968-134">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="de968-134">marketingNotificationEmails</span></span>|<span data-ttu-id="de968-135">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="de968-135">String collection</span></span>|                                        <span data-ttu-id="de968-136">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="de968-136">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="de968-137">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="de968-137">privacyProfile</span></span>|[<span data-ttu-id="de968-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="de968-138">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="de968-139">組織のプライバシー プロファイル (statementUrl と contactEmail を設定します)。</span><span class="sxs-lookup"><span data-stu-id="de968-139">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="de968-140">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="de968-140">securityComplianceNotificationMails</span></span>|<span data-ttu-id="de968-141">String collection</span><span class="sxs-lookup"><span data-stu-id="de968-141">String collection</span></span>||
|<span data-ttu-id="de968-142">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="de968-142">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="de968-143">String コレクション</span><span class="sxs-lookup"><span data-stu-id="de968-143">String collection</span></span>||
|<span data-ttu-id="de968-144">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="de968-144">technicalNotificationMails</span></span>|<span data-ttu-id="de968-145">String collection</span><span class="sxs-lookup"><span data-stu-id="de968-145">String collection</span></span>|                                        <span data-ttu-id="de968-146">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="de968-146">**Notes**: not nullable.</span></span>            |

<span data-ttu-id="de968-147">**組織**リソースが[拡張機能](/graph/extensibility-overview)をサポートしているため`PATCH` 、この操作を使用して、既存の**組織**インスタンスの拡張機能のカスタムプロパティで、独自のアプリ固有のデータを追加、更新、または削除できます。</span><span class="sxs-lookup"><span data-stu-id="de968-147">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **organization** instance.</span></span>

## <a name="response"></a><span data-ttu-id="de968-148">応答</span><span class="sxs-lookup"><span data-stu-id="de968-148">Response</span></span>

<span data-ttu-id="de968-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="de968-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de968-151">例</span><span class="sxs-lookup"><span data-stu-id="de968-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de968-152">要求</span><span class="sxs-lookup"><span data-stu-id="de968-152">Request</span></span>
<span data-ttu-id="de968-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="de968-153">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="de968-154">プロトコル</span><span class="sxs-lookup"><span data-stu-id="de968-154">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="de968-155">C#</span><span class="sxs-lookup"><span data-stu-id="de968-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de968-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de968-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="de968-157">目的-C</span><span class="sxs-lookup"><span data-stu-id="de968-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="de968-158">応答</span><span class="sxs-lookup"><span data-stu-id="de968-158">Response</span></span>

<span data-ttu-id="de968-159">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="de968-159">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="de968-160">関連項目</span><span class="sxs-lookup"><span data-stu-id="de968-160">See also</span></span>

- [<span data-ttu-id="de968-161">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="de968-161">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="de968-162">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="de968-162">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)

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
  ]
}
-->
