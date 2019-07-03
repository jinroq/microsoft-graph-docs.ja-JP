---
title: Update groupLifecyclePolicy
description: groupLifecyclePolicygroupLifecyclePolicy リソース タイプ オブジェクトのプロパティを更新します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 13c5b72916ce0ba0b8a6d6516931d99b39ac16f5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35442574"
---
# <a name="update-grouplifecyclepolicy"></a><span data-ttu-id="2a37e-103">Update groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="2a37e-103">Update groupLifecyclePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a37e-104">groupLifecyclePolicy[groupLifecyclePolicy リソース タイプ](../resources/grouplifecyclepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2a37e-104">Update the properties of a groupLifecyclePolicy[groupLifecyclePolicy resource type](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a37e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2a37e-105">Permissions</span></span>

<span data-ttu-id="2a37e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a37e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="2a37e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2a37e-108">Permission type</span></span>      | <span data-ttu-id="2a37e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2a37e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a37e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2a37e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2a37e-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a37e-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="2a37e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2a37e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a37e-113">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="2a37e-113">Not supported</span></span> |
|<span data-ttu-id="2a37e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2a37e-114">Application</span></span> | <span data-ttu-id="2a37e-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a37e-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a37e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2a37e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="2a37e-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2a37e-117">Optional request headers</span></span>
| <span data-ttu-id="2a37e-118">名前</span><span class="sxs-lookup"><span data-stu-id="2a37e-118">Name</span></span> | <span data-ttu-id="2a37e-119">説明</span><span class="sxs-lookup"><span data-stu-id="2a37e-119">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="2a37e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a37e-120">Authorization</span></span> | <span data-ttu-id="2a37e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2a37e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2a37e-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2a37e-123">Content-Type</span></span>  | <span data-ttu-id="2a37e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2a37e-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2a37e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="2a37e-125">Request body</span></span>

<span data-ttu-id="2a37e-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="2a37e-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2a37e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2a37e-129">Property</span></span> | <span data-ttu-id="2a37e-130">型</span><span class="sxs-lookup"><span data-stu-id="2a37e-130">Type</span></span> | <span data-ttu-id="2a37e-131">説明</span><span class="sxs-lookup"><span data-stu-id="2a37e-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2a37e-132">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="2a37e-132">alternateNotificationEmails</span></span>|<span data-ttu-id="2a37e-133">String</span><span class="sxs-lookup"><span data-stu-id="2a37e-133">String</span></span>| <span data-ttu-id="2a37e-134">所有者のいないグループに対して通知を送信する電子メール アドレスのリスト</span><span class="sxs-lookup"><span data-stu-id="2a37e-134">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="2a37e-135">電子メール アドレスをセミコロンで区切って、複数の電子メール アドレスを定義することができます。</span><span class="sxs-lookup"><span data-stu-id="2a37e-135">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="2a37e-136">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="2a37e-136">groupLifetimeInDays</span></span>|<span data-ttu-id="2a37e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="2a37e-137">Int32</span></span>| <span data-ttu-id="2a37e-138">グループの有効期限が切れ、更新が必要になるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="2a37e-138">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="2a37e-139">更新されると、グループの有効期限は定義された日数、延長されます。</span><span class="sxs-lookup"><span data-stu-id="2a37e-139">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="2a37e-140">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="2a37e-140">managedGroupTypes</span></span>|<span data-ttu-id="2a37e-141">String</span><span class="sxs-lookup"><span data-stu-id="2a37e-141">String</span></span>| <span data-ttu-id="2a37e-142">有効期限ポリシーを適用するグループの種類。</span><span class="sxs-lookup"><span data-stu-id="2a37e-142">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="2a37e-143">可能な値は、**All**、**Selected**、または **None** です。</span><span class="sxs-lookup"><span data-stu-id="2a37e-143">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="response"></a><span data-ttu-id="2a37e-144">応答</span><span class="sxs-lookup"><span data-stu-id="2a37e-144">Response</span></span>

<span data-ttu-id="2a37e-145">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="2a37e-145">If successful, this method returns a `200 OK` response code and updated [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2a37e-146">例</span><span class="sxs-lookup"><span data-stu-id="2a37e-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2a37e-147">要求</span><span class="sxs-lookup"><span data-stu-id="2a37e-147">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2a37e-148">プロトコル</span><span class="sxs-lookup"><span data-stu-id="2a37e-148">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="2a37e-149">C#</span><span class="sxs-lookup"><span data-stu-id="2a37e-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2a37e-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="2a37e-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2a37e-151">目的-C</span><span class="sxs-lookup"><span data-stu-id="2a37e-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2a37e-152">応答</span><span class="sxs-lookup"><span data-stu-id="2a37e-152">Response</span></span>
<span data-ttu-id="2a37e-153">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="2a37e-153">Note: The response object shown here may be truncated for brevity.</span></span> 
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
  ]
}
-->
