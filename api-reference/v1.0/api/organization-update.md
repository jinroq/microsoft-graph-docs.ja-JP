---
title: 組織を更新する
description: 現在認証されている組織のプロパティを更新します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7cd98bfecc68405b613adb5453841094f2e02772
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36022671"
---
# <a name="update-organization"></a><span data-ttu-id="5bb87-103">組織を更新する</span><span class="sxs-lookup"><span data-stu-id="5bb87-103">Update organization</span></span>

<span data-ttu-id="5bb87-104">現在認証されている組織のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5bb87-104">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="5bb87-105">この例では`organization` 、は、1つのレコードのコレクションとして定義されているため、要求でその**ID**を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5bb87-105">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="5bb87-106">**ID**は、組織の**tenantId**とも呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="5bb87-106">The **ID** is also known as the **tenantId** of the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="5bb87-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5bb87-107">Permissions</span></span>

<span data-ttu-id="5bb87-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5bb87-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bb87-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5bb87-110">Permission type</span></span> | <span data-ttu-id="5bb87-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5bb87-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5bb87-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5bb87-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5bb87-113">Directory.accessasuser.all、すべてのディレクトリを示します。</span><span class="sxs-lookup"><span data-stu-id="5bb87-113">Organization.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5bb87-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5bb87-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5bb87-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5bb87-115">Not supported.</span></span>    |
|<span data-ttu-id="5bb87-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5bb87-116">Application</span></span> | <span data-ttu-id="5bb87-117">組織の ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5bb87-117">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5bb87-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5bb87-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5bb87-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5bb87-119">Request headers</span></span>

| <span data-ttu-id="5bb87-120">名前</span><span class="sxs-lookup"><span data-stu-id="5bb87-120">Name</span></span>       | <span data-ttu-id="5bb87-121">説明</span><span class="sxs-lookup"><span data-stu-id="5bb87-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="5bb87-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bb87-122">Authorization</span></span>  | <span data-ttu-id="5bb87-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5bb87-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5bb87-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5bb87-125">Content-Type</span></span>   | <span data-ttu-id="5bb87-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5bb87-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5bb87-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5bb87-127">Request body</span></span>

<span data-ttu-id="5bb87-128">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="5bb87-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5bb87-129">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="5bb87-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5bb87-130">最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="5bb87-130">For best performance, you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5bb87-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5bb87-131">Property</span></span>     | <span data-ttu-id="5bb87-132">型</span><span class="sxs-lookup"><span data-stu-id="5bb87-132">Type</span></span>   |<span data-ttu-id="5bb87-133">説明</span><span class="sxs-lookup"><span data-stu-id="5bb87-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5bb87-134">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="5bb87-134">marketingNotificationEmails</span></span>|<span data-ttu-id="5bb87-135">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="5bb87-135">String collection</span></span>|                                        <span data-ttu-id="5bb87-136">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="5bb87-136">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="5bb87-137">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="5bb87-137">privacyProfile</span></span>|[<span data-ttu-id="5bb87-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="5bb87-138">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="5bb87-139">組織のプライバシー プロファイル (statementUrl と contactEmail を設定します)。</span><span class="sxs-lookup"><span data-stu-id="5bb87-139">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="5bb87-140">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="5bb87-140">securityComplianceNotificationMails</span></span>|<span data-ttu-id="5bb87-141">String collection</span><span class="sxs-lookup"><span data-stu-id="5bb87-141">String collection</span></span>||
|<span data-ttu-id="5bb87-142">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="5bb87-142">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="5bb87-143">String コレクション</span><span class="sxs-lookup"><span data-stu-id="5bb87-143">String collection</span></span>||
|<span data-ttu-id="5bb87-144">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="5bb87-144">technicalNotificationMails</span></span>|<span data-ttu-id="5bb87-145">String collection</span><span class="sxs-lookup"><span data-stu-id="5bb87-145">String collection</span></span>|                                        <span data-ttu-id="5bb87-146">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="5bb87-146">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="5bb87-147">応答</span><span class="sxs-lookup"><span data-stu-id="5bb87-147">Response</span></span>

<span data-ttu-id="5bb87-148">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="5bb87-148">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5bb87-149">例</span><span class="sxs-lookup"><span data-stu-id="5bb87-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="5bb87-150">要求</span><span class="sxs-lookup"><span data-stu-id="5bb87-150">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5bb87-151">プロトコル</span><span class="sxs-lookup"><span data-stu-id="5bb87-151">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="5bb87-152">C#</span><span class="sxs-lookup"><span data-stu-id="5bb87-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5bb87-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="5bb87-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5bb87-154">目的-C</span><span class="sxs-lookup"><span data-stu-id="5bb87-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5bb87-155">Java</span><span class="sxs-lookup"><span data-stu-id="5bb87-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5bb87-156">応答</span><span class="sxs-lookup"><span data-stu-id="5bb87-156">Response</span></span>

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
