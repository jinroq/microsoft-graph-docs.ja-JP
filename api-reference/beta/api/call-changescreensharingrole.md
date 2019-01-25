---
title: '電話: changeScreenSharingRole'
description: 起動し、画面の呼び出しでの共有を停止します。 この API を使用して、通話や会議の参加者と画面の内容を共有するアプリケーションを許可します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f0bdd9a4c8e900d9a1ec5f7801fa959ebdaae1e1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514734"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="0e23f-104">電話: changeScreenSharingRole</span><span class="sxs-lookup"><span data-stu-id="0e23f-104">call: changeScreenSharingRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e23f-105">起動し、画面の呼び出しでの共有を停止します。</span><span class="sxs-lookup"><span data-stu-id="0e23f-105">Start and stop sharing screen in the call.</span></span> <span data-ttu-id="0e23f-106">この API を使用して、通話や会議の参加者と画面の内容を共有するアプリケーションを許可します。</span><span class="sxs-lookup"><span data-stu-id="0e23f-106">This API is used to allow applications to share screen content with the participants of a call or meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e23f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0e23f-107">Permissions</span></span>
<span data-ttu-id="0e23f-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0e23f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0e23f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0e23f-110">Permission type</span></span>                        | <span data-ttu-id="0e23f-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0e23f-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0e23f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0e23f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0e23f-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="0e23f-113">Not Supported</span></span>                               |
| <span data-ttu-id="0e23f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0e23f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e23f-115">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="0e23f-115">Not Supported</span></span>                               |
| <span data-ttu-id="0e23f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0e23f-116">Application</span></span>                            | <span data-ttu-id="0e23f-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="0e23f-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="0e23f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0e23f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/changeScreenSharingRole
POST /applications/{id}/calls/{id}/changeScreenSharingRole
```

## <a name="request-headers"></a><span data-ttu-id="0e23f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0e23f-119">Request headers</span></span>
| <span data-ttu-id="0e23f-120">名前</span><span class="sxs-lookup"><span data-stu-id="0e23f-120">Name</span></span>          | <span data-ttu-id="0e23f-121">説明</span><span class="sxs-lookup"><span data-stu-id="0e23f-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="0e23f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e23f-122">Authorization</span></span> | <span data-ttu-id="0e23f-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0e23f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e23f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="0e23f-125">Request body</span></span>
<span data-ttu-id="0e23f-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="0e23f-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0e23f-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="0e23f-127">Parameter</span></span>      | <span data-ttu-id="0e23f-128">型</span><span class="sxs-lookup"><span data-stu-id="0e23f-128">Type</span></span>    |<span data-ttu-id="0e23f-129">説明</span><span class="sxs-lookup"><span data-stu-id="0e23f-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e23f-130">role</span><span class="sxs-lookup"><span data-stu-id="0e23f-130">role</span></span>|<span data-ttu-id="0e23f-131">String</span><span class="sxs-lookup"><span data-stu-id="0e23f-131">String</span></span>|<span data-ttu-id="0e23f-132">使用可能な値: 'ビューアー'、'共有'</span><span class="sxs-lookup"><span data-stu-id="0e23f-132">Possible values are: 'Viewer', 'Sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="0e23f-133">応答</span><span class="sxs-lookup"><span data-stu-id="0e23f-133">Response</span></span>
<span data-ttu-id="0e23f-134">応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="0e23f-134">Returns `202 Accepted` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0e23f-135">例</span><span class="sxs-lookup"><span data-stu-id="0e23f-135">Example</span></span>
<span data-ttu-id="0e23f-136">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="0e23f-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="0e23f-137">要求</span><span class="sxs-lookup"><span data-stu-id="0e23f-137">Request</span></span>
<span data-ttu-id="0e23f-138">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="0e23f-138">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-changeScreenSharingRole"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/changeScreenSharingRole
Content-Type: application/json
Content-Length: 24

{
  "role": "viewer"
}
```

##### <a name="response"></a><span data-ttu-id="0e23f-139">応答</span><span class="sxs-lookup"><span data-stu-id="0e23f-139">Response</span></span>
<span data-ttu-id="0e23f-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="0e23f-140">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: changeScreenSharingRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-changescreensharingrole.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
