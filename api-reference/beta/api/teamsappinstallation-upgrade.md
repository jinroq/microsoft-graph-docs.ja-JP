---
title: チームでアプリケーションをアップグレードします。
description: チームで、アプリケーションのインストールをアップグレードします。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 194763ea8464dd0651c3af1cef73e479b403d083
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831375"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="0a4cc-103">チームでアプリケーションをアップグレードします。</span><span class="sxs-lookup"><span data-stu-id="0a4cc-103">Upgrade an app in a team</span></span>

> <span data-ttu-id="0a4cc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0a4cc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a4cc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a4cc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0a4cc-106">[チーム](../resources/team.md)で[アプリケーションのインストール](../resources/teamsappinstallation.md)をアプリケーションの最新バージョンにアップグレードします。</span><span class="sxs-lookup"><span data-stu-id="0a4cc-106">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a4cc-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0a4cc-107">Permissions</span></span>

<span data-ttu-id="0a4cc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0a4cc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a4cc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0a4cc-110">Permission type</span></span>      | <span data-ttu-id="0a4cc-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0a4cc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a4cc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0a4cc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0a4cc-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a4cc-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0a4cc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0a4cc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a4cc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a4cc-115">Not supported.</span></span>    |
|<span data-ttu-id="0a4cc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0a4cc-116">Application</span></span> | <span data-ttu-id="0a4cc-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a4cc-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a4cc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0a4cc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="0a4cc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a4cc-119">Request headers</span></span>
| <span data-ttu-id="0a4cc-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a4cc-120">Header</span></span>       | <span data-ttu-id="0a4cc-121">値</span><span class="sxs-lookup"><span data-stu-id="0a4cc-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0a4cc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a4cc-122">Authorization</span></span>  | <span data-ttu-id="0a4cc-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0a4cc-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0a4cc-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="0a4cc-125">Request body</span></span>
<span data-ttu-id="0a4cc-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0a4cc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a4cc-127">応答</span><span class="sxs-lookup"><span data-stu-id="0a4cc-127">Response</span></span>

<span data-ttu-id="0a4cc-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="0a4cc-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a4cc-130">例</span><span class="sxs-lookup"><span data-stu-id="0a4cc-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0a4cc-131">要求</span><span class="sxs-lookup"><span data-stu-id="0a4cc-131">Request</span></span>
<span data-ttu-id="0a4cc-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0a4cc-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
#### <a name="response"></a><span data-ttu-id="0a4cc-133">応答</span><span class="sxs-lookup"><span data-stu-id="0a4cc-133">Response</span></span>
<span data-ttu-id="0a4cc-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0a4cc-134">The following is an example of the response.</span></span> 

><span data-ttu-id="0a4cc-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0a4cc-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
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
