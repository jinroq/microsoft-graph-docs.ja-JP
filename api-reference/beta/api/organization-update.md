---
title: 組織を更新する
description: 現在認証されている組織のプロパティを更新します。
localization_priority: Normal
ms.openlocfilehash: ae91b0f7cf92619f07f042c515bad2aab0d1035a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890420"
---
# <a name="update-organization"></a><span data-ttu-id="f5e8d-103">組織を更新する</span><span class="sxs-lookup"><span data-stu-id="f5e8d-103">Update organization</span></span>

> <span data-ttu-id="f5e8d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f5e8d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5e8d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5e8d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f5e8d-106">現在認証されている組織のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f5e8d-106">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="f5e8d-107">この例では、 `organization` 、1 つのレコードの集合として定義されている要求の**ID**を指定する必要がありますので。</span><span class="sxs-lookup"><span data-stu-id="f5e8d-107">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="f5e8d-108">**ID**は、組織の**tenantId**とも呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="f5e8d-108">The **ID** is also known as the **tenantId** of the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5e8d-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f5e8d-109">Permissions</span></span>

<span data-ttu-id="f5e8d-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f5e8d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5e8d-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f5e8d-112">Permission type</span></span> | <span data-ttu-id="f5e8d-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f5e8d-113">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5e8d-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f5e8d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f5e8d-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f5e8d-115">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="f5e8d-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f5e8d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5e8d-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5e8d-117">Not supported.</span></span> |
|<span data-ttu-id="f5e8d-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f5e8d-118">Application</span></span> | <span data-ttu-id="f5e8d-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5e8d-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5e8d-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f5e8d-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f5e8d-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f5e8d-121">Request headers</span></span>

| <span data-ttu-id="f5e8d-122">名前</span><span class="sxs-lookup"><span data-stu-id="f5e8d-122">Name</span></span>       | <span data-ttu-id="f5e8d-123">種類</span><span class="sxs-lookup"><span data-stu-id="f5e8d-123">Type</span></span> | <span data-ttu-id="f5e8d-124">説明</span><span class="sxs-lookup"><span data-stu-id="f5e8d-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f5e8d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5e8d-125">Authorization</span></span>  | <span data-ttu-id="f5e8d-126">string</span><span class="sxs-lookup"><span data-stu-id="f5e8d-126">string</span></span>  | <span data-ttu-id="f5e8d-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f5e8d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5e8d-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="f5e8d-129">Request body</span></span>

<span data-ttu-id="f5e8d-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="f5e8d-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f5e8d-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5e8d-133">Property</span></span>     | <span data-ttu-id="f5e8d-134">種類</span><span class="sxs-lookup"><span data-stu-id="f5e8d-134">Type</span></span>   |<span data-ttu-id="f5e8d-135">説明</span><span class="sxs-lookup"><span data-stu-id="f5e8d-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5e8d-136">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="f5e8d-136">marketingNotificationEmails</span></span>|<span data-ttu-id="f5e8d-137">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f5e8d-137">String collection</span></span>|                                        <span data-ttu-id="f5e8d-138">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="f5e8d-138">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="f5e8d-139">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="f5e8d-139">privacyProfile</span></span>|[<span data-ttu-id="f5e8d-140">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="f5e8d-140">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="f5e8d-141">組織のプライバシー プロファイル (statementUrl と contactEmail を設定します)。</span><span class="sxs-lookup"><span data-stu-id="f5e8d-141">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="f5e8d-142">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="f5e8d-142">securityComplianceNotificationMails</span></span>|<span data-ttu-id="f5e8d-143">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f5e8d-143">String collection</span></span>||
|<span data-ttu-id="f5e8d-144">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="f5e8d-144">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="f5e8d-145">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f5e8d-145">String collection</span></span>||
|<span data-ttu-id="f5e8d-146">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="f5e8d-146">technicalNotificationMails</span></span>|<span data-ttu-id="f5e8d-147">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f5e8d-147">String collection</span></span>|                                        <span data-ttu-id="f5e8d-148">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="f5e8d-148">**Notes**: not nullable.</span></span>            |

<span data-ttu-id="f5e8d-149">使用することが**組織**のリソースは、[拡張機能](/graph/extensibility-overview)をサポートするため、`PATCH`を追加、更新、または**組織**の既存のインスタンスで拡張機能のカスタム プロパティに独自のアプリケーション固有データを削除する操作です。</span><span class="sxs-lookup"><span data-stu-id="f5e8d-149">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **organization** instance.</span></span>

## <a name="response"></a><span data-ttu-id="f5e8d-150">応答</span><span class="sxs-lookup"><span data-stu-id="f5e8d-150">Response</span></span>

<span data-ttu-id="f5e8d-p106">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="f5e8d-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5e8d-153">例</span><span class="sxs-lookup"><span data-stu-id="f5e8d-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f5e8d-154">要求</span><span class="sxs-lookup"><span data-stu-id="f5e8d-154">Request</span></span>
<span data-ttu-id="f5e8d-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f5e8d-155">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="f5e8d-156">応答</span><span class="sxs-lookup"><span data-stu-id="f5e8d-156">Response</span></span>

<span data-ttu-id="f5e8d-157">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="f5e8d-157">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="f5e8d-158">関連項目</span><span class="sxs-lookup"><span data-stu-id="f5e8d-158">See also</span></span>

- [<span data-ttu-id="f5e8d-159">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="f5e8d-159">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="f5e8d-160">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="f5e8d-160">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)

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
