---
title: アプリケーションをチームに追加します。
description: 指定されたチームには、アプリケーションをインストールします。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: d3f67b8ea49f9940b60bcf0aec7eea15a59388b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855861"
---
# <a name="add-app-to-team"></a><span data-ttu-id="a0750-103">アプリケーションをチームに追加します。</span><span class="sxs-lookup"><span data-stu-id="a0750-103">Add app to team</span></span>

> <span data-ttu-id="a0750-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a0750-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0750-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a0750-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a0750-106">指定された[チーム](../resources/team.md)には、[アプリケーション](../resources/teamsapp.md)をインストールします。</span><span class="sxs-lookup"><span data-stu-id="a0750-106">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a0750-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a0750-107">Permissions</span></span>
<span data-ttu-id="a0750-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a0750-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0750-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a0750-110">Permission type</span></span>      | <span data-ttu-id="a0750-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a0750-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0750-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a0750-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a0750-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0750-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a0750-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a0750-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0750-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a0750-115">Not supported.</span></span>    |
|<span data-ttu-id="a0750-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a0750-116">Application</span></span> | <span data-ttu-id="a0750-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a0750-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0750-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a0750-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="a0750-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a0750-119">Request headers</span></span>
| <span data-ttu-id="a0750-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a0750-120">Header</span></span>       | <span data-ttu-id="a0750-121">値</span><span class="sxs-lookup"><span data-stu-id="a0750-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a0750-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0750-122">Authorization</span></span>  | <span data-ttu-id="a0750-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a0750-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a0750-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a0750-125">Request body</span></span>

| <span data-ttu-id="a0750-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a0750-126">Property</span></span>     | <span data-ttu-id="a0750-127">種類</span><span class="sxs-lookup"><span data-stu-id="a0750-127">Type</span></span>   |<span data-ttu-id="a0750-128">説明</span><span class="sxs-lookup"><span data-stu-id="a0750-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0750-129">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a0750-129">teamsApp</span></span>|<span data-ttu-id="a0750-130">String</span><span class="sxs-lookup"><span data-stu-id="a0750-130">String</span></span>|<span data-ttu-id="a0750-131">追加するのにはアプリケーションの id です。</span><span class="sxs-lookup"><span data-stu-id="a0750-131">The id of the app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="a0750-132">応答</span><span class="sxs-lookup"><span data-stu-id="a0750-132">Response</span></span>

<span data-ttu-id="a0750-133">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="a0750-133">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="a0750-134">例</span><span class="sxs-lookup"><span data-stu-id="a0750-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a0750-135">要求</span><span class="sxs-lookup"><span data-stu-id="a0750-135">Request</span></span>
<span data-ttu-id="a0750-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a0750-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/installedApps
{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
#### <a name="response"></a><span data-ttu-id="a0750-137">応答</span><span class="sxs-lookup"><span data-stu-id="a0750-137">Response</span></span>
<span data-ttu-id="a0750-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a0750-138">The following is an example of the response.</span></span> <span data-ttu-id="a0750-139">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="a0750-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a0750-140">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a0750-140">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="a0750-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="a0750-141">See also</span></span>

