---
title: outlooktaskgroup の作成
description: ユーザーのメールボックスに Outlook のタスクグループを作成します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 364510c3d866b193012763d17dbc22f2e1d7c8f7
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869261"
---
# <a name="create-outlooktaskgroup"></a><span data-ttu-id="579a0-103">outlooktaskgroup の作成</span><span class="sxs-lookup"><span data-stu-id="579a0-103">Create outlookTaskGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="579a0-104">ユーザーのメールボックスに Outlook のタスクグループを作成します。</span><span class="sxs-lookup"><span data-stu-id="579a0-104">Create an Outlook task group in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="579a0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="579a0-105">Permissions</span></span>
<span data-ttu-id="579a0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="579a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="579a0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="579a0-108">Permission type</span></span>      | <span data-ttu-id="579a0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="579a0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="579a0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="579a0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="579a0-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="579a0-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="579a0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="579a0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="579a0-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="579a0-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="579a0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="579a0-114">Application</span></span> | <span data-ttu-id="579a0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="579a0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="579a0-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="579a0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskGroups
POST /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="request-headers"></a><span data-ttu-id="579a0-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="579a0-117">Request headers</span></span>
| <span data-ttu-id="579a0-118">名前</span><span class="sxs-lookup"><span data-stu-id="579a0-118">Name</span></span>       | <span data-ttu-id="579a0-119">説明</span><span class="sxs-lookup"><span data-stu-id="579a0-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="579a0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="579a0-120">Authorization</span></span>  | <span data-ttu-id="579a0-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="579a0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="579a0-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="579a0-123">Request body</span></span>
<span data-ttu-id="579a0-124">要求本文で、 [outlooktaskgroup](../resources/outlooktaskgroup.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="579a0-124">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="579a0-125">応答</span><span class="sxs-lookup"><span data-stu-id="579a0-125">Response</span></span>

<span data-ttu-id="579a0-126">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[outlooktaskgroup](../resources/outlooktaskgroup.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="579a0-126">If successful, this method returns `201 Created` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="579a0-127">例</span><span class="sxs-lookup"><span data-stu-id="579a0-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="579a0-128">要求</span><span class="sxs-lookup"><span data-stu-id="579a0-128">Request</span></span>
<span data-ttu-id="579a0-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="579a0-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskgroup_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/taskGroups
Content-type: application/json
Content-length: 40

{
  "name": "Leisure tasks"
}
```
<span data-ttu-id="579a0-130">要求本文で、 [outlooktaskgroup](../resources/outlooktaskgroup.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="579a0-130">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="579a0-131">応答</span><span class="sxs-lookup"><span data-stu-id="579a0-131">Response</span></span>
<span data-ttu-id="579a0-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="579a0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 138

{
  "id": "AAMkADIyAAAhrbe-AAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAGjg==",
  "isDefaultGroup": false,
  "name": "Leisure tasks",
  "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-post-taskgroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
