---
title: 組織を更新する
description: 現在認証されている組織のプロパティを更新します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4201bed43327b17e808750d5f3f38f41e776bd77
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447468"
---
# <a name="update-organization"></a><span data-ttu-id="3c1a7-103">組織を更新する</span><span class="sxs-lookup"><span data-stu-id="3c1a7-103">Update organization</span></span>

<span data-ttu-id="3c1a7-104">現在認証されている組織のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3c1a7-104">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="3c1a7-105">この例では`organization` 、は、1つのレコードのコレクションとして定義されているため、要求でその**ID**を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3c1a7-105">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="3c1a7-106">**ID**は、組織の**tenantId**とも呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="3c1a7-106">The **ID** is also known as the **tenantId** of the organization.</span></span>


## <a name="permissions"></a><span data-ttu-id="3c1a7-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3c1a7-107">Permissions</span></span>

<span data-ttu-id="3c1a7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3c1a7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c1a7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3c1a7-110">Permission type</span></span> | <span data-ttu-id="3c1a7-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3c1a7-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c1a7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3c1a7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3c1a7-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3c1a7-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3c1a7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3c1a7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c1a7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3c1a7-115">Not supported.</span></span>    |
|<span data-ttu-id="3c1a7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3c1a7-116">Application</span></span> | <span data-ttu-id="3c1a7-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3c1a7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c1a7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3c1a7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}

```

## <a name="request-headers"></a><span data-ttu-id="3c1a7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3c1a7-119">Request headers</span></span>

| <span data-ttu-id="3c1a7-120">名前</span><span class="sxs-lookup"><span data-stu-id="3c1a7-120">Name</span></span>       | <span data-ttu-id="3c1a7-121">型</span><span class="sxs-lookup"><span data-stu-id="3c1a7-121">Type</span></span> | <span data-ttu-id="3c1a7-122">説明</span><span class="sxs-lookup"><span data-stu-id="3c1a7-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3c1a7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c1a7-123">Authorization</span></span>  | <span data-ttu-id="3c1a7-124">string</span><span class="sxs-lookup"><span data-stu-id="3c1a7-124">string</span></span>  | <span data-ttu-id="3c1a7-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3c1a7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c1a7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3c1a7-127">Request body</span></span>

<span data-ttu-id="3c1a7-128">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="3c1a7-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="3c1a7-129">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="3c1a7-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="3c1a7-130">最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="3c1a7-130">For best performance, you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3c1a7-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c1a7-131">Property</span></span>     | <span data-ttu-id="3c1a7-132">型</span><span class="sxs-lookup"><span data-stu-id="3c1a7-132">Type</span></span>   |<span data-ttu-id="3c1a7-133">説明</span><span class="sxs-lookup"><span data-stu-id="3c1a7-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c1a7-134">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="3c1a7-134">marketingNotificationEmails</span></span>|<span data-ttu-id="3c1a7-135">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="3c1a7-135">String collection</span></span>|                                        <span data-ttu-id="3c1a7-136">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="3c1a7-136">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="3c1a7-137">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="3c1a7-137">privacyProfile</span></span>|[<span data-ttu-id="3c1a7-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="3c1a7-138">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="3c1a7-139">組織のプライバシー プロファイル (statementUrl と contactEmail を設定します)。</span><span class="sxs-lookup"><span data-stu-id="3c1a7-139">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="3c1a7-140">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="3c1a7-140">securityComplianceNotificationMails</span></span>|<span data-ttu-id="3c1a7-141">String collection</span><span class="sxs-lookup"><span data-stu-id="3c1a7-141">String collection</span></span>||
|<span data-ttu-id="3c1a7-142">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="3c1a7-142">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="3c1a7-143">String コレクション</span><span class="sxs-lookup"><span data-stu-id="3c1a7-143">String collection</span></span>||
|<span data-ttu-id="3c1a7-144">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="3c1a7-144">technicalNotificationMails</span></span>|<span data-ttu-id="3c1a7-145">String collection</span><span class="sxs-lookup"><span data-stu-id="3c1a7-145">String collection</span></span>|                                        <span data-ttu-id="3c1a7-146">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="3c1a7-146">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="3c1a7-147">応答</span><span class="sxs-lookup"><span data-stu-id="3c1a7-147">Response</span></span>

<span data-ttu-id="3c1a7-148">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="3c1a7-148">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3c1a7-149">例</span><span class="sxs-lookup"><span data-stu-id="3c1a7-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c1a7-150">要求</span><span class="sxs-lookup"><span data-stu-id="3c1a7-150">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3c1a7-151">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3c1a7-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/{id}
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="3c1a7-152">C#</span><span class="sxs-lookup"><span data-stu-id="3c1a7-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3c1a7-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="3c1a7-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3c1a7-154">目的-C</span><span class="sxs-lookup"><span data-stu-id="3c1a7-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3c1a7-155">応答</span><span class="sxs-lookup"><span data-stu-id="3c1a7-155">Response</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
