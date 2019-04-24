---
title: Update groupLifecyclePolicy
description: groupLifecyclePolicygroupLifecyclePolicy リソース タイプ オブジェクトのプロパティを更新します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 69073693203981debbfa8010468df271ea65cef3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32501764"
---
# <a name="update-grouplifecyclepolicy"></a><span data-ttu-id="b3d2b-103">Update groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="b3d2b-103">Update groupLifecyclePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3d2b-104">groupLifecyclePolicy[groupLifecyclePolicy リソース タイプ](../resources/grouplifecyclepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b3d2b-104">Update the properties of a groupLifecyclePolicy[groupLifecyclePolicy resource type](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3d2b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b3d2b-105">Permissions</span></span>

<span data-ttu-id="b3d2b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b3d2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="b3d2b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b3d2b-108">Permission type</span></span>      | <span data-ttu-id="b3d2b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b3d2b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3d2b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b3d2b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b3d2b-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3d2b-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="b3d2b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b3d2b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3d2b-113">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="b3d2b-113">Not supported</span></span> |
|<span data-ttu-id="b3d2b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b3d2b-114">Application</span></span> | <span data-ttu-id="b3d2b-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3d2b-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3d2b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b3d2b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="b3d2b-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b3d2b-117">Optional request headers</span></span>
| <span data-ttu-id="b3d2b-118">名前</span><span class="sxs-lookup"><span data-stu-id="b3d2b-118">Name</span></span> | <span data-ttu-id="b3d2b-119">説明</span><span class="sxs-lookup"><span data-stu-id="b3d2b-119">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="b3d2b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3d2b-120">Authorization</span></span> | <span data-ttu-id="b3d2b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b3d2b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b3d2b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b3d2b-123">Content-Type</span></span>  | <span data-ttu-id="b3d2b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b3d2b-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b3d2b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b3d2b-125">Request body</span></span>

<span data-ttu-id="b3d2b-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="b3d2b-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b3d2b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3d2b-129">Property</span></span> | <span data-ttu-id="b3d2b-130">型</span><span class="sxs-lookup"><span data-stu-id="b3d2b-130">Type</span></span> | <span data-ttu-id="b3d2b-131">説明</span><span class="sxs-lookup"><span data-stu-id="b3d2b-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b3d2b-132">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="b3d2b-132">alternateNotificationEmails</span></span>|<span data-ttu-id="b3d2b-133">String</span><span class="sxs-lookup"><span data-stu-id="b3d2b-133">String</span></span>| <span data-ttu-id="b3d2b-134">所有者のいないグループに対して通知を送信する電子メール アドレスのリスト</span><span class="sxs-lookup"><span data-stu-id="b3d2b-134">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="b3d2b-135">電子メール アドレスをセミコロンで区切って、複数の電子メール アドレスを定義することができます。</span><span class="sxs-lookup"><span data-stu-id="b3d2b-135">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="b3d2b-136">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="b3d2b-136">groupLifetimeInDays</span></span>|<span data-ttu-id="b3d2b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b3d2b-137">Int32</span></span>| <span data-ttu-id="b3d2b-138">グループの有効期限が切れ、更新が必要になるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="b3d2b-138">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="b3d2b-139">更新されると、グループの有効期限は定義された日数、延長されます。</span><span class="sxs-lookup"><span data-stu-id="b3d2b-139">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="b3d2b-140">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="b3d2b-140">managedGroupTypes</span></span>|<span data-ttu-id="b3d2b-141">String</span><span class="sxs-lookup"><span data-stu-id="b3d2b-141">String</span></span>| <span data-ttu-id="b3d2b-142">有効期限ポリシーを適用するグループの種類。</span><span class="sxs-lookup"><span data-stu-id="b3d2b-142">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="b3d2b-143">可能な値は、**All**、**Selected**、または **None** です。</span><span class="sxs-lookup"><span data-stu-id="b3d2b-143">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="response"></a><span data-ttu-id="b3d2b-144">応答</span><span class="sxs-lookup"><span data-stu-id="b3d2b-144">Response</span></span>

<span data-ttu-id="b3d2b-145">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="b3d2b-145">If successful, this method returns a `200 OK` response code and updated [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b3d2b-146">例</span><span class="sxs-lookup"><span data-stu-id="b3d2b-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b3d2b-147">要求</span><span class="sxs-lookup"><span data-stu-id="b3d2b-147">Request</span></span>

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
##### <a name="response"></a><span data-ttu-id="b3d2b-148">応答</span><span class="sxs-lookup"><span data-stu-id="b3d2b-148">Response</span></span>
<span data-ttu-id="b3d2b-149">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="b3d2b-149">Note: The response object shown here may be truncated for brevity.</span></span> 
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
    "Error: /api-reference/beta/api/grouplifecyclepolicy-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
