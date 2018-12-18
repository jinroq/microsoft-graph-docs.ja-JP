---
title: Update groupLifecyclePolicy
description: groupLifecyclePolicygroupLifecyclePolicy リソース タイプ オブジェクトのプロパティを更新します。
author: dkershaw10
ms.openlocfilehash: 6977bb53a1b885ee65f110238727d4db0c212391
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303620"
---
# <a name="update-grouplifecyclepolicy"></a><span data-ttu-id="349c1-103">Update groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="349c1-103">Update groupLifecyclePolicy</span></span>

> <span data-ttu-id="349c1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="349c1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="349c1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="349c1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="349c1-106">groupLifecyclePolicy[groupLifecyclePolicy リソース タイプ](../resources/grouplifecyclepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="349c1-106">Update the properties of a groupLifecyclePolicy[groupLifecyclePolicy resource type](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="349c1-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="349c1-107">Permissions</span></span>

<span data-ttu-id="349c1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="349c1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="349c1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="349c1-110">Permission type</span></span>      | <span data-ttu-id="349c1-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="349c1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="349c1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="349c1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="349c1-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="349c1-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="349c1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="349c1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="349c1-115">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="349c1-115">Not supported</span></span> |
|<span data-ttu-id="349c1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="349c1-116">Application</span></span> | <span data-ttu-id="349c1-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="349c1-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="349c1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="349c1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="349c1-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="349c1-119">Optional request headers</span></span>
| <span data-ttu-id="349c1-120">名前</span><span class="sxs-lookup"><span data-stu-id="349c1-120">Name</span></span> | <span data-ttu-id="349c1-121">説明</span><span class="sxs-lookup"><span data-stu-id="349c1-121">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="349c1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="349c1-122">Authorization</span></span> | <span data-ttu-id="349c1-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="349c1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="349c1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="349c1-125">Content-Type</span></span>  | <span data-ttu-id="349c1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="349c1-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="349c1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="349c1-127">Request body</span></span>

<span data-ttu-id="349c1-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="349c1-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="349c1-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="349c1-131">Property</span></span> | <span data-ttu-id="349c1-132">種類</span><span class="sxs-lookup"><span data-stu-id="349c1-132">Type</span></span> | <span data-ttu-id="349c1-133">説明</span><span class="sxs-lookup"><span data-stu-id="349c1-133">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="349c1-134">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="349c1-134">alternateNotificationEmails</span></span>|<span data-ttu-id="349c1-135">String</span><span class="sxs-lookup"><span data-stu-id="349c1-135">String</span></span>| <span data-ttu-id="349c1-136">所有者のいないグループに対して通知を送信する電子メール アドレスのリスト</span><span class="sxs-lookup"><span data-stu-id="349c1-136">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="349c1-137">電子メール アドレスをセミコロンで区切って、複数の電子メール アドレスを定義することができます。</span><span class="sxs-lookup"><span data-stu-id="349c1-137">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="349c1-138">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="349c1-138">groupLifetimeInDays</span></span>|<span data-ttu-id="349c1-139">Int32</span><span class="sxs-lookup"><span data-stu-id="349c1-139">Int32</span></span>| <span data-ttu-id="349c1-140">グループの有効期限が切れ、更新が必要になるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="349c1-140">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="349c1-141">更新されると、グループの有効期限は定義された日数、延長されます。</span><span class="sxs-lookup"><span data-stu-id="349c1-141">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="349c1-142">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="349c1-142">managedGroupTypes</span></span>|<span data-ttu-id="349c1-143">String</span><span class="sxs-lookup"><span data-stu-id="349c1-143">String</span></span>| <span data-ttu-id="349c1-144">有効期限ポリシーを適用するグループの種類。</span><span class="sxs-lookup"><span data-stu-id="349c1-144">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="349c1-145">可能な値は、**All**、**Selected**、または **None** です。</span><span class="sxs-lookup"><span data-stu-id="349c1-145">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="response"></a><span data-ttu-id="349c1-146">応答</span><span class="sxs-lookup"><span data-stu-id="349c1-146">Response</span></span>

<span data-ttu-id="349c1-147">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="349c1-147">If successful, this method returns a `200 OK` response code and updated [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="349c1-148">例</span><span class="sxs-lookup"><span data-stu-id="349c1-148">Example</span></span>

##### <a name="request"></a><span data-ttu-id="349c1-149">要求</span><span class="sxs-lookup"><span data-stu-id="349c1-149">Request</span></span>

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
##### <a name="response"></a><span data-ttu-id="349c1-150">応答</span><span class="sxs-lookup"><span data-stu-id="349c1-150">Response</span></span>
<span data-ttu-id="349c1-151">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="349c1-151">Note: The response object shown here may be truncated for brevity.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "Update groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->