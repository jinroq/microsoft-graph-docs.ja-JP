---
title: 添付ファイルを作成する
description: OutlookTask の添付ファイルを追加するのにには、この API を使用します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: ae6c420c9c0ccf10df4d2d62a27f4b8c0d857c32
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525025"
---
# <a name="create-attachment"></a><span data-ttu-id="e72b6-103">添付ファイルを作成する</span><span class="sxs-lookup"><span data-stu-id="e72b6-103">Create attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e72b6-104">[添付ファイル](../resources/attachment.md)を[outlookTask](../resources/outlooktask.md)に追加するのにには、この API を使用します。</span><span class="sxs-lookup"><span data-stu-id="e72b6-104">Use this API to add an [attachment](../resources/attachment.md) to an [outlookTask](../resources/outlooktask.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e72b6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e72b6-105">Permissions</span></span>

<span data-ttu-id="e72b6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e72b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e72b6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e72b6-108">Permission type</span></span>      | <span data-ttu-id="e72b6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e72b6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e72b6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e72b6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e72b6-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e72b6-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="e72b6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e72b6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e72b6-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e72b6-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="e72b6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e72b6-114">Application</span></span> | <span data-ttu-id="e72b6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e72b6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e72b6-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e72b6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/attachments
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="request-headers"></a><span data-ttu-id="e72b6-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e72b6-117">Request headers</span></span>

| <span data-ttu-id="e72b6-118">名前</span><span class="sxs-lookup"><span data-stu-id="e72b6-118">Name</span></span>       | <span data-ttu-id="e72b6-119">説明</span><span class="sxs-lookup"><span data-stu-id="e72b6-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e72b6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e72b6-120">Authorization</span></span>  | <span data-ttu-id="e72b6-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e72b6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e72b6-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e72b6-123">Content-Type</span></span> | <span data-ttu-id="e72b6-124">エンティティの本文内のデータの種類を表す文字列。</span><span class="sxs-lookup"><span data-stu-id="e72b6-124">A string that represents the type of data in the body of an entity.</span></span> <span data-ttu-id="e72b6-125">必須です。</span><span class="sxs-lookup"><span data-stu-id="e72b6-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e72b6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e72b6-126">Request body</span></span>

<span data-ttu-id="e72b6-127">要求本文で、[attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e72b6-127">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e72b6-128">応答</span><span class="sxs-lookup"><span data-stu-id="e72b6-128">Response</span></span>

<span data-ttu-id="e72b6-129">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [attachment](../resources/attachment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e72b6-129">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e72b6-130">例</span><span class="sxs-lookup"><span data-stu-id="e72b6-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e72b6-131">要求</span><span class="sxs-lookup"><span data-stu-id="e72b6-131">Request</span></span>

<span data-ttu-id="e72b6-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e72b6-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_attachment_from_outlooktask"
}-->

```http
POST https://graph.microsoft.com/beta/users/{id}/outlook/tasks/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true
}
```

### <a name="response"></a><span data-ttu-id="e72b6-133">応答</span><span class="sxs-lookup"><span data-stu-id="e72b6-133">Response</span></span>

<span data-ttu-id="e72b6-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e72b6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktask-post-attachments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
