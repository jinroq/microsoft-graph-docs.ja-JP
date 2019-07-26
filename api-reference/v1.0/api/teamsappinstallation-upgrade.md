---
title: チーム内のアプリをアップグレードする
description: チーム内のアプリのインストールをアップグレードする
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c717ca93c832736671f856a6454bcf0de877681c
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908463"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="ad21b-103">チーム内のアプリをアップグレードする</span><span class="sxs-lookup"><span data-stu-id="ad21b-103">Upgrade an app in a team</span></span>

<span data-ttu-id="ad21b-104">[チーム](../resources/team.md)内の[アプリのインストール](../resources/teamsappinstallation.md)をアプリの最新バージョンにアップグレードします。</span><span class="sxs-lookup"><span data-stu-id="ad21b-104">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad21b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ad21b-105">Permissions</span></span>

<span data-ttu-id="ad21b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad21b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad21b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ad21b-108">Permission type</span></span>      | <span data-ttu-id="ad21b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ad21b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad21b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ad21b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ad21b-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad21b-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ad21b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ad21b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad21b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad21b-113">Not supported.</span></span>    |
|<span data-ttu-id="ad21b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ad21b-114">Application</span></span> | <span data-ttu-id="ad21b-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad21b-115">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="ad21b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ad21b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="ad21b-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad21b-117">Request headers</span></span>

| <span data-ttu-id="ad21b-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad21b-118">Header</span></span>       | <span data-ttu-id="ad21b-119">値</span><span class="sxs-lookup"><span data-stu-id="ad21b-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ad21b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad21b-120">Authorization</span></span>  | <span data-ttu-id="ad21b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ad21b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ad21b-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ad21b-123">Request body</span></span>

<span data-ttu-id="ad21b-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ad21b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad21b-125">応答</span><span class="sxs-lookup"><span data-stu-id="ad21b-125">Response</span></span>

<span data-ttu-id="ad21b-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ad21b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad21b-128">例</span><span class="sxs-lookup"><span data-stu-id="ad21b-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad21b-129">要求</span><span class="sxs-lookup"><span data-stu-id="ad21b-129">Request</span></span>

<span data-ttu-id="ad21b-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ad21b-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "upgrade_teamsapp"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```

### <a name="response"></a><span data-ttu-id="ad21b-131">応答</span><span class="sxs-lookup"><span data-stu-id="ad21b-131">Response</span></span>

<span data-ttu-id="ad21b-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ad21b-132">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "upgrade_teamsapp",
  "truncated": true
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
