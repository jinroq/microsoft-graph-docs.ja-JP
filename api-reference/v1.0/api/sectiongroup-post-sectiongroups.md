---
title: sectionGroup を作成する
description: 指定されたセクション グループに新しいセクション グループを作成します。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: a05e61934c8043c0c6a94c6e0785c0e93e4a3e19
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32520929"
---
# <a name="create-sectiongroup"></a><span data-ttu-id="0728d-103">sectionGroup を作成する</span><span class="sxs-lookup"><span data-stu-id="0728d-103">Create sectionGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0728d-104">指定されたセクション グループに新しい[セクション グループ](../resources/sectiongroup.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="0728d-104">Create a new [section group](../resources/sectiongroup.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="0728d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0728d-105">Permissions</span></span>
<span data-ttu-id="0728d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0728d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0728d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0728d-108">Permission type</span></span>      | <span data-ttu-id="0728d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0728d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0728d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0728d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0728d-111">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0728d-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="0728d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0728d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0728d-113">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0728d-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="0728d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0728d-114">Application</span></span> | <span data-ttu-id="0728d-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0728d-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0728d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0728d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
POST /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
POST /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="0728d-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0728d-117">Request headers</span></span>
| <span data-ttu-id="0728d-118">名前</span><span class="sxs-lookup"><span data-stu-id="0728d-118">Name</span></span>       | <span data-ttu-id="0728d-119">型</span><span class="sxs-lookup"><span data-stu-id="0728d-119">Type</span></span> | <span data-ttu-id="0728d-120">説明</span><span class="sxs-lookup"><span data-stu-id="0728d-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0728d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0728d-121">Authorization</span></span>  | <span data-ttu-id="0728d-122">string</span><span class="sxs-lookup"><span data-stu-id="0728d-122">string</span></span>  | <span data-ttu-id="0728d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0728d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0728d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0728d-125">Content-Type</span></span> | <span data-ttu-id="0728d-126">string</span><span class="sxs-lookup"><span data-stu-id="0728d-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="0728d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0728d-127">Request body</span></span>
<span data-ttu-id="0728d-128">要求本文でセクション グループ名を指定します。</span><span class="sxs-lookup"><span data-stu-id="0728d-128">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="0728d-p103">同じ階層レベルのセクション グループには一意の名前が必要です。名前は 50 文字以内で、次の文字は使用できません: ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="0728d-p103">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="0728d-131">応答</span><span class="sxs-lookup"><span data-stu-id="0728d-131">Response</span></span>

<span data-ttu-id="0728d-132">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [sectionGroup](../resources/sectiongroup.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0728d-132">If successful, this method returns a `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0728d-133">例</span><span class="sxs-lookup"><span data-stu-id="0728d-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0728d-134">要求</span><span class="sxs-lookup"><span data-stu-id="0728d-134">Request</span></span>
<span data-ttu-id="0728d-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0728d-135">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="0728d-136">応答</span><span class="sxs-lookup"><span data-stu-id="0728d-136">Response</span></span>
<span data-ttu-id="0728d-p104">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0728d-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create SectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/sectiongroup-post-sectiongroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
