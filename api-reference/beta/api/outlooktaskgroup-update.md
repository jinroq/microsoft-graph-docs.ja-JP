---
title: outlooktaskgroup を更新する
description: Outlook タスクグループの書き込み可能なプロパティを更新します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: b628f0cf610afef88a198db721ee5395a34d1e08
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539612"
---
# <a name="update-outlooktaskgroup"></a><span data-ttu-id="7baf8-103">outlooktaskgroup を更新する</span><span class="sxs-lookup"><span data-stu-id="7baf8-103">Update outlooktaskgroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7baf8-104">Outlook タスクグループの書き込み可能なプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7baf8-104">Update the writable properties of an Outlook task group.</span></span>

<span data-ttu-id="7baf8-105">既定のタスクグループの名前 ([自分のタスク]) は変更できないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="7baf8-105">Note that you cannot modify the name of the default task group, "My Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="7baf8-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7baf8-106">Permissions</span></span>
<span data-ttu-id="7baf8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7baf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7baf8-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7baf8-109">Permission type</span></span>      | <span data-ttu-id="7baf8-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7baf8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7baf8-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7baf8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7baf8-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7baf8-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="7baf8-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7baf8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7baf8-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7baf8-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="7baf8-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7baf8-115">Application</span></span> | <span data-ttu-id="7baf8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7baf8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7baf8-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7baf8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/taskGroups/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="7baf8-118">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7baf8-118">Optional request headers</span></span>
| <span data-ttu-id="7baf8-119">名前</span><span class="sxs-lookup"><span data-stu-id="7baf8-119">Name</span></span>       | <span data-ttu-id="7baf8-120">説明</span><span class="sxs-lookup"><span data-stu-id="7baf8-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7baf8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7baf8-121">Authorization</span></span>  | <span data-ttu-id="7baf8-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7baf8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7baf8-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="7baf8-124">Request body</span></span>
<span data-ttu-id="7baf8-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="7baf8-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7baf8-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7baf8-128">Property</span></span>     | <span data-ttu-id="7baf8-129">型</span><span class="sxs-lookup"><span data-stu-id="7baf8-129">Type</span></span>   |<span data-ttu-id="7baf8-130">説明</span><span class="sxs-lookup"><span data-stu-id="7baf8-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7baf8-131">name</span><span class="sxs-lookup"><span data-stu-id="7baf8-131">name</span></span>|<span data-ttu-id="7baf8-132">String</span><span class="sxs-lookup"><span data-stu-id="7baf8-132">String</span></span>|<span data-ttu-id="7baf8-133">タスク グループの名前。</span><span class="sxs-lookup"><span data-stu-id="7baf8-133">The name of the task group.</span></span>|

## <a name="response"></a><span data-ttu-id="7baf8-134">応答</span><span class="sxs-lookup"><span data-stu-id="7baf8-134">Response</span></span>

<span data-ttu-id="7baf8-135">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[outlooktaskgroup](../resources/outlooktaskgroup.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7baf8-135">If successful, this method returns a `200 OK` response code and updated [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7baf8-136">例</span><span class="sxs-lookup"><span data-stu-id="7baf8-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7baf8-137">要求</span><span class="sxs-lookup"><span data-stu-id="7baf8-137">Request</span></span>
<span data-ttu-id="7baf8-138">次の例では、タスク グループの名前を "Personal Tasks" に変更します。</span><span class="sxs-lookup"><span data-stu-id="7baf8-138">The following example changes the name of a task group to "Personal Tasks".</span></span> 
<!-- {
  "blockType": "request",
  "name": "update_outlooktaskgroup"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/outlook/taskgroups('AAMkADIyAAAhrbe-AAA=')

Content-type: application/json
Content-length: 28

{
  "name": "Personal Tasks",
}
```
##### <a name="response"></a><span data-ttu-id="7baf8-139">応答</span><span class="sxs-lookup"><span data-stu-id="7baf8-139">Response</span></span>
<span data-ttu-id="7baf8-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7baf8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 138

{
  "id": "AAMkADIyAAAhrbe-AAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAGjw==",
  "isDefaultGroup": false,
  "name": "Personal Tasks",
  "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update outlooktaskgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskgroup-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
