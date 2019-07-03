---
title: List schedulingGroups
description: このスケジュールで schedulingGroup の一覧を取得します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 28573cb4e495d0d138cedefe0ba4c34c743bb44a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447670"
---
# <a name="list-schedulegroups"></a><span data-ttu-id="a62e2-103">ScheduleGroups を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a62e2-103">List scheduleGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a62e2-104">この[スケジュール](../resources/schedule.md)で[schedulingGroups](../resources/schedulinggroup.md)の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="a62e2-104">Get the list of [schedulingGroups](../resources/schedulinggroup.md) in this [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a62e2-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a62e2-105">Permissions</span></span>

<span data-ttu-id="a62e2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a62e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a62e2-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a62e2-108">Permission type</span></span>      | <span data-ttu-id="a62e2-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a62e2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a62e2-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a62e2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a62e2-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a62e2-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a62e2-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a62e2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a62e2-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a62e2-113">Not supported.</span></span>    |
|<span data-ttu-id="a62e2-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a62e2-114">Application</span></span> | <span data-ttu-id="a62e2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a62e2-115">Not supported.</span></span> |

> <span data-ttu-id="a62e2-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a62e2-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a62e2-117">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="a62e2-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a62e2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a62e2-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/schedulingGroups
```

## <a name="request-headers"></a><span data-ttu-id="a62e2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a62e2-119">Request headers</span></span>

| <span data-ttu-id="a62e2-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a62e2-120">Header</span></span>       | <span data-ttu-id="a62e2-121">値</span><span class="sxs-lookup"><span data-stu-id="a62e2-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a62e2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a62e2-122">Authorization</span></span>  | <span data-ttu-id="a62e2-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a62e2-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a62e2-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a62e2-125">Content-Type</span></span>  | <span data-ttu-id="a62e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a62e2-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a62e2-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a62e2-127">Request body</span></span>
<span data-ttu-id="a62e2-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a62e2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a62e2-129">応答</span><span class="sxs-lookup"><span data-stu-id="a62e2-129">Response</span></span>

<span data-ttu-id="a62e2-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[schedulingGroup](../resources/schedulinggroup.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a62e2-130">If successful, this method returns a `200 OK` response code and a collection of [schedulingGroup](../resources/schedulinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a62e2-131">例</span><span class="sxs-lookup"><span data-stu-id="a62e2-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a62e2-132">要求</span><span class="sxs-lookup"><span data-stu-id="a62e2-132">Request</span></span>

<span data-ttu-id="a62e2-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a62e2-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a62e2-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a62e2-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-list-schedulinggroups"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a62e2-135">C#</span><span class="sxs-lookup"><span data-stu-id="a62e2-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-list-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a62e2-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="a62e2-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-list-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a62e2-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="a62e2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-list-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a62e2-138">応答</span><span class="sxs-lookup"><span data-stu-id="a62e2-138">Response</span></span>

<span data-ttu-id="a62e2-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a62e2-139">The following is an example of the response.</span></span> 

><span data-ttu-id="a62e2-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a62e2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedulingGroup",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "value": [
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
        "@odata.type":"microsoft.graph.identitySet",
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
          "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
          "displayName": "John Doe"
        }
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get the list of schedulingGroup in this schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
