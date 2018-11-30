---
title: 組織を更新する
description: 現在認証されている組織のプロパティを更新します。
ms.openlocfilehash: ac07f3ded31f8d6c7169d24208ed7e8cf967e07a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023387"
---
# <a name="update-organization"></a><span data-ttu-id="aaa30-103">組織を更新する</span><span class="sxs-lookup"><span data-stu-id="aaa30-103">Update organization</span></span>

<span data-ttu-id="aaa30-104">現在認証されている組織のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="aaa30-104">Update the properties of the currently authenticated organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="aaa30-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="aaa30-105">Permissions</span></span>

<span data-ttu-id="aaa30-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aaa30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaa30-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aaa30-108">Permission type</span></span> | <span data-ttu-id="aaa30-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="aaa30-109">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aaa30-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aaa30-110">Delegated (work or school account)</span></span> | <span data-ttu-id="aaa30-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aaa30-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="aaa30-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aaa30-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aaa30-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aaa30-113">Not supported.</span></span>    |
|<span data-ttu-id="aaa30-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aaa30-114">Application</span></span> | <span data-ttu-id="aaa30-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aaa30-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aaa30-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aaa30-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization

```

## <a name="request-headers"></a><span data-ttu-id="aaa30-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aaa30-117">Request headers</span></span>

| <span data-ttu-id="aaa30-118">名前</span><span class="sxs-lookup"><span data-stu-id="aaa30-118">Name</span></span>       | <span data-ttu-id="aaa30-119">型</span><span class="sxs-lookup"><span data-stu-id="aaa30-119">Type</span></span> | <span data-ttu-id="aaa30-120">説明</span><span class="sxs-lookup"><span data-stu-id="aaa30-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="aaa30-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="aaa30-121">Authorization</span></span>  | <span data-ttu-id="aaa30-122">string</span><span class="sxs-lookup"><span data-stu-id="aaa30-122">string</span></span>  | <span data-ttu-id="aaa30-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="aaa30-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aaa30-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="aaa30-125">Request body</span></span>
<span data-ttu-id="aaa30-126">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="aaa30-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="aaa30-127">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="aaa30-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="aaa30-128">最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="aaa30-128">For best performance, you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="aaa30-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aaa30-129">Property</span></span>     | <span data-ttu-id="aaa30-130">型</span><span class="sxs-lookup"><span data-stu-id="aaa30-130">Type</span></span>   |<span data-ttu-id="aaa30-131">説明</span><span class="sxs-lookup"><span data-stu-id="aaa30-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aaa30-132">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="aaa30-132">marketingNotificationEmails</span></span>|<span data-ttu-id="aaa30-133">String コレクション</span><span class="sxs-lookup"><span data-stu-id="aaa30-133">String collection</span></span>|                                        <span data-ttu-id="aaa30-134">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="aaa30-134">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="aaa30-135">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="aaa30-135">privacyProfile</span></span>|[<span data-ttu-id="aaa30-136">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="aaa30-136">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="aaa30-137">組織のプライバシー プロファイル (statementUrl と contactEmail を設定します)。</span><span class="sxs-lookup"><span data-stu-id="aaa30-137">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="aaa30-138">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="aaa30-138">securityComplianceNotificationMails</span></span>|<span data-ttu-id="aaa30-139">String コレクション</span><span class="sxs-lookup"><span data-stu-id="aaa30-139">String collection</span></span>||
|<span data-ttu-id="aaa30-140">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="aaa30-140">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="aaa30-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="aaa30-141">String collection</span></span>||
|<span data-ttu-id="aaa30-142">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="aaa30-142">technicalNotificationMails</span></span>|<span data-ttu-id="aaa30-143">String コレクション</span><span class="sxs-lookup"><span data-stu-id="aaa30-143">String collection</span></span>|                                        <span data-ttu-id="aaa30-144">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="aaa30-144">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="aaa30-145">応答</span><span class="sxs-lookup"><span data-stu-id="aaa30-145">Response</span></span>

<span data-ttu-id="aaa30-146">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="aaa30-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="aaa30-147">例</span><span class="sxs-lookup"><span data-stu-id="aaa30-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="aaa30-148">要求</span><span class="sxs-lookup"><span data-stu-id="aaa30-148">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization
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

### <a name="response"></a><span data-ttu-id="aaa30-149">応答</span><span class="sxs-lookup"><span data-stu-id="aaa30-149">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
