---
title: 上司を割り当てる
description: この API を使用して、ユーザーの上司を割り当てます。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4148eb1748680458500dc5a625e6b297e0ca5099
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514552"
---
# <a name="assign-a-manager"></a><span data-ttu-id="a367b-103">上司を割り当てる</span><span class="sxs-lookup"><span data-stu-id="a367b-103">Assign a manager</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a367b-104">この API を使用して、ユーザーの上司を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="a367b-104">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="a367b-105">注:直属の部下を割り当てることはできません。代わりにこの API を使用します。</span><span class="sxs-lookup"><span data-stu-id="a367b-105">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="a367b-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a367b-106">Permissions</span></span>
<span data-ttu-id="a367b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a367b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a367b-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a367b-109">Permission type</span></span>      | <span data-ttu-id="a367b-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a367b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a367b-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a367b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a367b-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a367b-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a367b-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a367b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a367b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a367b-114">Not supported.</span></span>    |
|<span data-ttu-id="a367b-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a367b-115">Application</span></span> | <span data-ttu-id="a367b-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a367b-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a367b-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a367b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="a367b-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a367b-118">Request headers</span></span>
| <span data-ttu-id="a367b-119">名前</span><span class="sxs-lookup"><span data-stu-id="a367b-119">Name</span></span>       | <span data-ttu-id="a367b-120">型</span><span class="sxs-lookup"><span data-stu-id="a367b-120">Type</span></span> | <span data-ttu-id="a367b-121">説明</span><span class="sxs-lookup"><span data-stu-id="a367b-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a367b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a367b-122">Authorization</span></span>  | <span data-ttu-id="a367b-123">string</span><span class="sxs-lookup"><span data-stu-id="a367b-123">string</span></span>  | <span data-ttu-id="a367b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a367b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a367b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a367b-126">Request body</span></span>
<span data-ttu-id="a367b-127">要求本文で、追加する [directoryObject](../resources/directoryobject.md) または[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a367b-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="a367b-128">応答</span><span class="sxs-lookup"><span data-stu-id="a367b-128">Response</span></span>

<span data-ttu-id="a367b-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="a367b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a367b-131">例</span><span class="sxs-lookup"><span data-stu-id="a367b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a367b-132">要求</span><span class="sxs-lookup"><span data-stu-id="a367b-132">Request</span></span>
<span data-ttu-id="a367b-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a367b-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
PUT https://graph.microsoft.com/v1.0/users/{id}/manager/$ref
Content-type: application/json
Content-length: xxx

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="a367b-134">要求本文で、追加する[ユーザー](../resources/user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a367b-134">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="a367b-135">応答</span><span class="sxs-lookup"><span data-stu-id="a367b-135">Response</span></span>
<span data-ttu-id="a367b-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a367b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-post-manager.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
