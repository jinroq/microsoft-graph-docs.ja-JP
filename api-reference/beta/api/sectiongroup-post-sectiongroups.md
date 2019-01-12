---
title: sectionGroup を作成する
description: 指定されたセクション グループに新しいセクション グループを作成します。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 2236cdcf832d3fd0ea496c5b4c4634b38803c303
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932967"
---
# <a name="create-sectiongroup"></a><span data-ttu-id="5eec3-103">sectionGroup を作成する</span><span class="sxs-lookup"><span data-stu-id="5eec3-103">Create sectionGroup</span></span>

> <span data-ttu-id="5eec3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5eec3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5eec3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5eec3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5eec3-106">指定されたセクション グループに新しい[セクション グループ](../resources/sectiongroup.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="5eec3-106">Create a new [section group](../resources/sectiongroup.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="5eec3-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5eec3-107">Permissions</span></span>
<span data-ttu-id="5eec3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5eec3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5eec3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5eec3-110">Permission type</span></span>      | <span data-ttu-id="5eec3-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5eec3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5eec3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5eec3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5eec3-113">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5eec3-113">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="5eec3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5eec3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5eec3-115">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5eec3-115">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="5eec3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5eec3-116">Application</span></span> | <span data-ttu-id="5eec3-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5eec3-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5eec3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5eec3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
POST /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
POST /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="5eec3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5eec3-119">Request headers</span></span>
| <span data-ttu-id="5eec3-120">名前</span><span class="sxs-lookup"><span data-stu-id="5eec3-120">Name</span></span>       | <span data-ttu-id="5eec3-121">型</span><span class="sxs-lookup"><span data-stu-id="5eec3-121">Type</span></span> | <span data-ttu-id="5eec3-122">説明</span><span class="sxs-lookup"><span data-stu-id="5eec3-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5eec3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5eec3-123">Authorization</span></span>  | <span data-ttu-id="5eec3-124">string</span><span class="sxs-lookup"><span data-stu-id="5eec3-124">string</span></span>  | <span data-ttu-id="5eec3-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5eec3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5eec3-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5eec3-127">Content-Type</span></span> | <span data-ttu-id="5eec3-128">string</span><span class="sxs-lookup"><span data-stu-id="5eec3-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="5eec3-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="5eec3-129">Request body</span></span>
<span data-ttu-id="5eec3-130">要求本文でセクション グループ名を指定します。</span><span class="sxs-lookup"><span data-stu-id="5eec3-130">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="5eec3-p104">同じ階層レベルのセクション グループには一意の名前が必要です。名前は 50 文字以内で、次の文字は使用できません: ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="5eec3-p104">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="5eec3-133">応答</span><span class="sxs-lookup"><span data-stu-id="5eec3-133">Response</span></span>

<span data-ttu-id="5eec3-134">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [sectionGroup](../resources/sectiongroup.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5eec3-134">If successful, this method returns a `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5eec3-135">例</span><span class="sxs-lookup"><span data-stu-id="5eec3-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5eec3-136">要求</span><span class="sxs-lookup"><span data-stu-id="5eec3-136">Request</span></span>
<span data-ttu-id="5eec3-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5eec3-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_sectiongroup_from_sectiongroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}/sectionGroups
Content-type: application/json
Content-length: 30

{
  "displayName": "Section group name"
}
```
##### <a name="response"></a><span data-ttu-id="5eec3-138">応答</span><span class="sxs-lookup"><span data-stu-id="5eec3-138">Response</span></span>
<span data-ttu-id="5eec3-p105">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5eec3-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectiongroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

{
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "displayName": "name-value",  
  "createdBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "lastModifiedBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create SectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
