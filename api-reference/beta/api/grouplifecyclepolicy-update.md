---
title: Update groupLifecyclePolicy
description: groupLifecyclePolicygroupLifecyclePolicy リソース タイプ オブジェクトのプロパティを更新します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f2e7e7fd27566476e224d5c58cbd12803b6c38aa
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262721"
---
# <a name="update-grouplifecyclepolicy"></a><span data-ttu-id="c3f8f-103">Update groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="c3f8f-103">Update groupLifecyclePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3f8f-104">groupLifecyclePolicy[groupLifecyclePolicy リソース タイプ](../resources/grouplifecyclepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c3f8f-104">Update the properties of a groupLifecyclePolicy[groupLifecyclePolicy resource type](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3f8f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c3f8f-105">Permissions</span></span>

<span data-ttu-id="c3f8f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3f8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="c3f8f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c3f8f-108">Permission type</span></span>      | <span data-ttu-id="c3f8f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c3f8f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3f8f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c3f8f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c3f8f-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3f8f-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="c3f8f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c3f8f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3f8f-113">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="c3f8f-113">Not supported</span></span> |
|<span data-ttu-id="c3f8f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c3f8f-114">Application</span></span> | <span data-ttu-id="c3f8f-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3f8f-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3f8f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c3f8f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="c3f8f-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3f8f-117">Optional request headers</span></span>
| <span data-ttu-id="c3f8f-118">名前</span><span class="sxs-lookup"><span data-stu-id="c3f8f-118">Name</span></span> | <span data-ttu-id="c3f8f-119">説明</span><span class="sxs-lookup"><span data-stu-id="c3f8f-119">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="c3f8f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3f8f-120">Authorization</span></span> | <span data-ttu-id="c3f8f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c3f8f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c3f8f-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c3f8f-123">Content-Type</span></span>  | <span data-ttu-id="c3f8f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c3f8f-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c3f8f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c3f8f-125">Request body</span></span>

<span data-ttu-id="c3f8f-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="c3f8f-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c3f8f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3f8f-129">Property</span></span> | <span data-ttu-id="c3f8f-130">型</span><span class="sxs-lookup"><span data-stu-id="c3f8f-130">Type</span></span> | <span data-ttu-id="c3f8f-131">説明</span><span class="sxs-lookup"><span data-stu-id="c3f8f-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c3f8f-132">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="c3f8f-132">alternateNotificationEmails</span></span>|<span data-ttu-id="c3f8f-133">String</span><span class="sxs-lookup"><span data-stu-id="c3f8f-133">String</span></span>| <span data-ttu-id="c3f8f-134">所有者のいないグループに対して通知を送信する電子メール アドレスのリスト</span><span class="sxs-lookup"><span data-stu-id="c3f8f-134">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="c3f8f-135">電子メール アドレスをセミコロンで区切って、複数の電子メール アドレスを定義することができます。</span><span class="sxs-lookup"><span data-stu-id="c3f8f-135">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="c3f8f-136">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="c3f8f-136">groupLifetimeInDays</span></span>|<span data-ttu-id="c3f8f-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c3f8f-137">Int32</span></span>| <span data-ttu-id="c3f8f-138">グループの有効期限が切れ、更新が必要になるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="c3f8f-138">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="c3f8f-139">更新されると、グループの有効期限は定義された日数、延長されます。</span><span class="sxs-lookup"><span data-stu-id="c3f8f-139">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="c3f8f-140">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="c3f8f-140">managedGroupTypes</span></span>|<span data-ttu-id="c3f8f-141">String</span><span class="sxs-lookup"><span data-stu-id="c3f8f-141">String</span></span>| <span data-ttu-id="c3f8f-142">有効期限ポリシーを適用するグループの種類。</span><span class="sxs-lookup"><span data-stu-id="c3f8f-142">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="c3f8f-143">可能な値は、**All**、**Selected**、または **None** です。</span><span class="sxs-lookup"><span data-stu-id="c3f8f-143">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="response"></a><span data-ttu-id="c3f8f-144">応答</span><span class="sxs-lookup"><span data-stu-id="c3f8f-144">Response</span></span>

<span data-ttu-id="c3f8f-145">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="c3f8f-145">If successful, this method returns a `200 OK` response code and updated [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c3f8f-146">例</span><span class="sxs-lookup"><span data-stu-id="c3f8f-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c3f8f-147">要求</span><span class="sxs-lookup"><span data-stu-id="c3f8f-147">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_grouplifecyclepolicy"
}-->
```http
PATCH https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
Content-type: application/json
Content-length: 151

{
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
##### <a name="response"></a><span data-ttu-id="c3f8f-148">応答</span><span class="sxs-lookup"><span data-stu-id="c3f8f-148">Response</span></span>
<span data-ttu-id="c3f8f-149">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="c3f8f-149">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "id": "id-value",
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c3f8f-150">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="c3f8f-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c3f8f-151">C#</span><span class="sxs-lookup"><span data-stu-id="c3f8f-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_grouplifecyclepolicy-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c3f8f-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="c3f8f-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_grouplifecyclepolicy-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c3f8f-153">目的-C</span><span class="sxs-lookup"><span data-stu-id="c3f8f-153">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_grouplifecyclepolicy-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/grouplifecyclepolicy-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/grouplifecyclepolicy-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/grouplifecyclepolicy-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
