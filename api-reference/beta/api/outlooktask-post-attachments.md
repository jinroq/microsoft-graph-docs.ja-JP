---
title: 添付ファイルを作成します。
description: OutlookTask の添付ファイルを追加するのにには、この API を使用します。
author: angelgolfer-ms
ms.openlocfilehash: 9b4f74ee469783cd6e143446cd3fc28f28000aa8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355686"
---
# <a name="create-attachment"></a><span data-ttu-id="d62b4-103">添付ファイルを作成する</span><span class="sxs-lookup"><span data-stu-id="d62b4-103">Create attachment</span></span>

> <span data-ttu-id="d62b4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d62b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d62b4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d62b4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d62b4-106">[添付ファイル](../resources/attachment.md)を[outlookTask](../resources/outlooktask.md)に追加するのにには、この API を使用します。</span><span class="sxs-lookup"><span data-stu-id="d62b4-106">Use this API to add an [attachment](../resources/attachment.md) to an [outlookTask](../resources/outlooktask.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="d62b4-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d62b4-107">Permissions</span></span>
<span data-ttu-id="d62b4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d62b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d62b4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d62b4-110">Permission type</span></span>      | <span data-ttu-id="d62b4-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d62b4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d62b4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d62b4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d62b4-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d62b4-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="d62b4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d62b4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d62b4-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d62b4-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="d62b4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d62b4-116">Application</span></span> | <span data-ttu-id="d62b4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d62b4-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d62b4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d62b4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}/attachments
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}/attachments

```
## <a name="request-headers"></a><span data-ttu-id="d62b4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d62b4-119">Request headers</span></span>
| <span data-ttu-id="d62b4-120">名前</span><span class="sxs-lookup"><span data-stu-id="d62b4-120">Name</span></span>       | <span data-ttu-id="d62b4-121">説明</span><span class="sxs-lookup"><span data-stu-id="d62b4-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d62b4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d62b4-122">Authorization</span></span>  | <span data-ttu-id="d62b4-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d62b4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d62b4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d62b4-125">Content-Type</span></span> | <span data-ttu-id="d62b4-126">エンティティの本文内のデータの種類を表す文字列。</span><span class="sxs-lookup"><span data-stu-id="d62b4-126">A string that represents the type of data in the body of an entity.</span></span> <span data-ttu-id="d62b4-127">必須です。</span><span class="sxs-lookup"><span data-stu-id="d62b4-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d62b4-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="d62b4-128">Request body</span></span>
<span data-ttu-id="d62b4-129">要求本文で、[attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d62b4-129">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d62b4-130">応答</span><span class="sxs-lookup"><span data-stu-id="d62b4-130">Response</span></span>

<span data-ttu-id="d62b4-131">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [attachment](../resources/attachment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d62b4-131">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d62b4-132">例</span><span class="sxs-lookup"><span data-stu-id="d62b4-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d62b4-133">要求</span><span class="sxs-lookup"><span data-stu-id="d62b4-133">Request</span></span>
<span data-ttu-id="d62b4-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d62b4-134">Here is an example of the request.</span></span>
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
<span data-ttu-id="d62b4-135">要求本文で、[Attachment](../resources/attachment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d62b4-135">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d62b4-136">応答</span><span class="sxs-lookup"><span data-stu-id="d62b4-136">Response</span></span>
<span data-ttu-id="d62b4-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d62b4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->