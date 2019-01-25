---
title: セクションを作成する
description: 指定されたノートブックに新しいセクションを作成します。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 3f40c9d89c8b507b142748378b0a9a90be82203d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526810"
---
# <a name="create-section"></a><span data-ttu-id="eabcc-103">セクションを作成する</span><span class="sxs-lookup"><span data-stu-id="eabcc-103">Create section</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eabcc-104">指定されたノートブックに新しい[セクション](../resources/section.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="eabcc-104">Create a new [section](../resources/section.md) in the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="eabcc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="eabcc-105">Permissions</span></span>
<span data-ttu-id="eabcc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eabcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eabcc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eabcc-108">Permission type</span></span>      | <span data-ttu-id="eabcc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="eabcc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eabcc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eabcc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="eabcc-111">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eabcc-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="eabcc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eabcc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eabcc-113">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eabcc-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="eabcc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eabcc-114">Application</span></span> | <span data-ttu-id="eabcc-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eabcc-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eabcc-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eabcc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/sections
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/sections
POST /groups/{id}/onenote/notebooks/{id}/sections
POST /sites/{id}/onenote/notebooks/{id}/sections
```
## <a name="request-headers"></a><span data-ttu-id="eabcc-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eabcc-117">Request headers</span></span>
| <span data-ttu-id="eabcc-118">名前</span><span class="sxs-lookup"><span data-stu-id="eabcc-118">Name</span></span>       | <span data-ttu-id="eabcc-119">型</span><span class="sxs-lookup"><span data-stu-id="eabcc-119">Type</span></span> | <span data-ttu-id="eabcc-120">説明</span><span class="sxs-lookup"><span data-stu-id="eabcc-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="eabcc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eabcc-121">Authorization</span></span>  | <span data-ttu-id="eabcc-122">string</span><span class="sxs-lookup"><span data-stu-id="eabcc-122">string</span></span>  | <span data-ttu-id="eabcc-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="eabcc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eabcc-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eabcc-125">Content-Type</span></span> | <span data-ttu-id="eabcc-126">string</span><span class="sxs-lookup"><span data-stu-id="eabcc-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="eabcc-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="eabcc-127">Request body</span></span>
<span data-ttu-id="eabcc-128">要求本文でセクション名を入力します。</span><span class="sxs-lookup"><span data-stu-id="eabcc-128">In the request body, supply a name for the section.</span></span>

<span data-ttu-id="eabcc-p103">同じ階層レベルでは、セクションの名前を一意にする必要があります。名前は 50 文字以内で、次の文字は使用できません: ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="eabcc-p103">Within the same hierarchy level, section names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="eabcc-131">応答</span><span class="sxs-lookup"><span data-stu-id="eabcc-131">Response</span></span>

<span data-ttu-id="eabcc-132">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [section](../resources/section.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="eabcc-132">If successful, this method returns a `201 Created` response code and a [section](../resources/section.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eabcc-133">例</span><span class="sxs-lookup"><span data-stu-id="eabcc-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eabcc-134">要求</span><span class="sxs-lookup"><span data-stu-id="eabcc-134">Request</span></span>
<span data-ttu-id="eabcc-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="eabcc-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_section_from_notebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/sections
Content-type: application/json
Content-length: 27

{
  "displayName": "Section name"
}
```
##### <a name="response"></a><span data-ttu-id="eabcc-136">応答</span><span class="sxs-lookup"><span data-stu-id="eabcc-136">Response</span></span>
<span data-ttu-id="eabcc-p104">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="eabcc-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 272

{
  "isDefault": true,
  "pagesUrl": "pagesUrl-value",
  "displayName": "name-value",
  "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
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
  "description": "Create Section",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/notebook-post-sections.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
