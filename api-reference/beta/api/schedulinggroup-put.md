---
title: schedulingGroup を置換する
description: 既存の schedulingGroup を置き換えます。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f1ccca9d8df6ae1153de1086c62b9c6cf5756f15
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657701"
---
# <a name="replace-schedulinggroup"></a><span data-ttu-id="fabae-103">schedulingGroup を置換する</span><span class="sxs-lookup"><span data-stu-id="fabae-103">Replace schedulingGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fabae-104">既存の[schedulingGroup](../resources/schedulinggroup.md)を置き換えます。</span><span class="sxs-lookup"><span data-stu-id="fabae-104">Replace an existing [schedulingGroup](../resources/schedulinggroup.md).</span></span>

<span data-ttu-id="fabae-105">指定した[schedulingGroup](../resources/schedulinggroup.md)が存在しない場合、 `404 Not found`このメソッドはを返します。</span><span class="sxs-lookup"><span data-stu-id="fabae-105">If the specified [schedulingGroup](../resources/schedulinggroup.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="fabae-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fabae-106">Permissions</span></span>

<span data-ttu-id="fabae-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fabae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fabae-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fabae-109">Permission type</span></span>      | <span data-ttu-id="fabae-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fabae-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fabae-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fabae-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fabae-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fabae-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fabae-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fabae-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fabae-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fabae-114">Not supported.</span></span>    |
|<span data-ttu-id="fabae-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fabae-115">Application</span></span> | <span data-ttu-id="fabae-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fabae-116">Not supported.</span></span> |

> <span data-ttu-id="fabae-117">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="fabae-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="fabae-118">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="fabae-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="fabae-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fabae-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="fabae-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fabae-120">Request headers</span></span>

| <span data-ttu-id="fabae-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fabae-121">Header</span></span>       | <span data-ttu-id="fabae-122">値</span><span class="sxs-lookup"><span data-stu-id="fabae-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fabae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fabae-123">Authorization</span></span>  | <span data-ttu-id="fabae-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fabae-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fabae-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fabae-126">Content-Type</span></span>  | <span data-ttu-id="fabae-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fabae-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fabae-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="fabae-128">Request body</span></span>

<span data-ttu-id="fabae-129">要求本文で、 [schedulingGroup](../resources/schedulinggroup.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fabae-129">In the request body, supply a JSON representation of a [schedulingGroup](../resources/schedulinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fabae-130">応答</span><span class="sxs-lookup"><span data-stu-id="fabae-130">Response</span></span>

<span data-ttu-id="fabae-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[schedulingGroup](../resources/schedulinggroup.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fabae-131">If successful, this method returns a `200 OK` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fabae-132">例</span><span class="sxs-lookup"><span data-stu-id="fabae-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="fabae-133">要求</span><span class="sxs-lookup"><span data-stu-id="fabae-133">Request</span></span>

<span data-ttu-id="fabae-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fabae-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-put-schedulinggroups"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
Content-type: application/json
Prefer: return=representation

{
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ]
}
```

#### <a name="response"></a><span data-ttu-id="fabae-135">応答</span><span class="sxs-lookup"><span data-stu-id="fabae-135">Response</span></span>

<span data-ttu-id="fabae-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fabae-136">The following is an example of the response.</span></span> 

><span data-ttu-id="fabae-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="fabae-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedulingGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "TAG_f914d037-00a3-4ba4-b712-ef178cbea263",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ],
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Replace an existing schedulingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schedule-put-schedulinggroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
