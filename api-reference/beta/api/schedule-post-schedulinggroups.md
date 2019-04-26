---
title: schedulingGroup を作成する
description: 新しい schedulingGroup を作成します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 98d565cf5a6c521e8db0a420cc5e9d70c83ebd7d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331522"
---
# <a name="create-schedulinggroup"></a><span data-ttu-id="a695d-103">schedulingGroup を作成する</span><span class="sxs-lookup"><span data-stu-id="a695d-103">Create schedulingGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a695d-104">新しい[schedulingGroup](../resources/schedulinggroup.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="a695d-104">Create a new [schedulingGroup](../resources/schedulinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a695d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a695d-105">Permissions</span></span>

<span data-ttu-id="a695d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a695d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a695d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a695d-108">Permission type</span></span>      | <span data-ttu-id="a695d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a695d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a695d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a695d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a695d-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a695d-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a695d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a695d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a695d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a695d-113">Not supported.</span></span>    |
|<span data-ttu-id="a695d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a695d-114">Application</span></span> | <span data-ttu-id="a695d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a695d-115">Not supported.</span></span> |

> <span data-ttu-id="a695d-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a695d-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a695d-117">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="a695d-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a695d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a695d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/schedulingGroups
```

## <a name="request-headers"></a><span data-ttu-id="a695d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a695d-119">Request headers</span></span>

| <span data-ttu-id="a695d-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a695d-120">Header</span></span>       | <span data-ttu-id="a695d-121">値</span><span class="sxs-lookup"><span data-stu-id="a695d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a695d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a695d-122">Authorization</span></span>  | <span data-ttu-id="a695d-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a695d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a695d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a695d-125">Content-Type</span></span>  | <span data-ttu-id="a695d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a695d-126">application/json</span></span>  |

## <a name="response"></a><span data-ttu-id="a695d-127">応答</span><span class="sxs-lookup"><span data-stu-id="a695d-127">Response</span></span>

<span data-ttu-id="a695d-128">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[schedulingGroup](../resources/schedulinggroup.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a695d-128">If successful, this method returns a `201 Created` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a695d-129">例</span><span class="sxs-lookup"><span data-stu-id="a695d-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a695d-130">要求</span><span class="sxs-lookup"><span data-stu-id="a695d-130">Request</span></span>

<span data-ttu-id="a695d-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a695d-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-post-schedulinggroups"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups
Content-type: application/json

{
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ]
}
```

#### <a name="response"></a><span data-ttu-id="a695d-132">応答</span><span class="sxs-lookup"><span data-stu-id="a695d-132">Response</span></span>

<span data-ttu-id="a695d-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a695d-133">The following is an example of the response.</span></span> 

><span data-ttu-id="a695d-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a695d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedulingGroup"
} -->

```http
HTTP/1.1 201 Created
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
  "description": "Creates a new schedulingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
