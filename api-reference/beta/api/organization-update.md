---
title: 組織を更新する
description: 現在認証されている組織のプロパティを更新します。
ms.openlocfilehash: 62e03d7bee58f14acc5d5ace12d55f95d1d07a2d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068343"
---
# <a name="update-organization"></a><span data-ttu-id="5538d-103">組織を更新する</span><span class="sxs-lookup"><span data-stu-id="5538d-103">Update organization</span></span>

> <span data-ttu-id="5538d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5538d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5538d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5538d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5538d-106">現在認証されている組織のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5538d-106">Update the properties of the currently authenticated organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="5538d-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5538d-107">Permissions</span></span>
<span data-ttu-id="5538d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5538d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5538d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5538d-110">Permission type</span></span> | <span data-ttu-id="5538d-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5538d-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5538d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5538d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5538d-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5538d-113">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="5538d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5538d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5538d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5538d-115">Not supported.</span></span> |
|<span data-ttu-id="5538d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5538d-116">Application</span></span> | <span data-ttu-id="5538d-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5538d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5538d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5538d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /organization

```
## <a name="request-headers"></a><span data-ttu-id="5538d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5538d-119">Request headers</span></span>
| <span data-ttu-id="5538d-120">名前</span><span class="sxs-lookup"><span data-stu-id="5538d-120">Name</span></span>       | <span data-ttu-id="5538d-121">型</span><span class="sxs-lookup"><span data-stu-id="5538d-121">Type</span></span> | <span data-ttu-id="5538d-122">説明</span><span class="sxs-lookup"><span data-stu-id="5538d-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5538d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5538d-123">Authorization</span></span>  | <span data-ttu-id="5538d-124">string</span><span class="sxs-lookup"><span data-stu-id="5538d-124">string</span></span>  | <span data-ttu-id="5538d-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5538d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5538d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5538d-127">Request body</span></span>
<span data-ttu-id="5538d-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="5538d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5538d-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5538d-131">Property</span></span>     | <span data-ttu-id="5538d-132">型</span><span class="sxs-lookup"><span data-stu-id="5538d-132">Type</span></span>   |<span data-ttu-id="5538d-133">説明</span><span class="sxs-lookup"><span data-stu-id="5538d-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5538d-134">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="5538d-134">marketingNotificationEmails</span></span>|<span data-ttu-id="5538d-135">String コレクション</span><span class="sxs-lookup"><span data-stu-id="5538d-135">String collection</span></span>|                                        <span data-ttu-id="5538d-136">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="5538d-136">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="5538d-137">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="5538d-137">privacyProfile</span></span>|[<span data-ttu-id="5538d-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="5538d-138">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="5538d-139">組織のプライバシー プロファイル (statementUrl と contactEmail を設定します)。</span><span class="sxs-lookup"><span data-stu-id="5538d-139">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="5538d-140">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="5538d-140">securityComplianceNotificationMails</span></span>|<span data-ttu-id="5538d-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="5538d-141">String collection</span></span>||
|<span data-ttu-id="5538d-142">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="5538d-142">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="5538d-143">String コレクション</span><span class="sxs-lookup"><span data-stu-id="5538d-143">String collection</span></span>||
|<span data-ttu-id="5538d-144">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="5538d-144">technicalNotificationMails</span></span>|<span data-ttu-id="5538d-145">String コレクション</span><span class="sxs-lookup"><span data-stu-id="5538d-145">String collection</span></span>|                                        <span data-ttu-id="5538d-146">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="5538d-146">**Notes**: not nullable.</span></span>            |

<span data-ttu-id="5538d-147">使用することが**組織**のリソースは、[拡張機能](/graph/extensibility-overview)をサポートするため、`PATCH`を追加、更新、または**組織**の既存のインスタンスで拡張機能のカスタム プロパティに独自のアプリケーション固有データを削除する操作です。</span><span class="sxs-lookup"><span data-stu-id="5538d-147">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **organization** instance.</span></span>

## <a name="response"></a><span data-ttu-id="5538d-148">応答</span><span class="sxs-lookup"><span data-stu-id="5538d-148">Response</span></span>

<span data-ttu-id="5538d-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="5538d-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5538d-151">例</span><span class="sxs-lookup"><span data-stu-id="5538d-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5538d-152">要求</span><span class="sxs-lookup"><span data-stu-id="5538d-152">Request</span></span>
<span data-ttu-id="5538d-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5538d-153">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->
```http
PATCH https://graph.microsoft.com/beta/organization
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
##### <a name="response"></a><span data-ttu-id="5538d-154">応答</span><span class="sxs-lookup"><span data-stu-id="5538d-154">Response</span></span>
<span data-ttu-id="5538d-155">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="5538d-155">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeunit"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="5538d-156">関連項目</span><span class="sxs-lookup"><span data-stu-id="5538d-156">See also</span></span>

- [<span data-ttu-id="5538d-157">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="5538d-157">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="5538d-158">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="5538d-158">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
