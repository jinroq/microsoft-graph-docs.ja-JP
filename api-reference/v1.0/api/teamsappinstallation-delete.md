---
title: チームからアプリを削除する
description: 指定したチームからアプリをアンインストールします。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 149b905a6e090960351ae0da70b2a6080fea8fa1
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908475"
---
# <a name="remove-app-from-team"></a><span data-ttu-id="e62be-103">チームからアプリを削除する</span><span class="sxs-lookup"><span data-stu-id="e62be-103">Remove app from team</span></span>

<span data-ttu-id="e62be-104">指定した[チーム](../resources/team.md)から[アプリ](../resources/teamsappinstallation.md)をアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="e62be-104">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e62be-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e62be-105">Permissions</span></span>

<span data-ttu-id="e62be-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e62be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e62be-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e62be-108">Permission type</span></span>      | <span data-ttu-id="e62be-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e62be-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e62be-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e62be-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e62be-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e62be-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e62be-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e62be-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e62be-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e62be-113">Not supported.</span></span>    |
|<span data-ttu-id="e62be-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e62be-114">Application</span></span> | <span data-ttu-id="e62be-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e62be-115">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="e62be-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e62be-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e62be-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e62be-117">Request headers</span></span>

| <span data-ttu-id="e62be-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e62be-118">Header</span></span>       | <span data-ttu-id="e62be-119">値</span><span class="sxs-lookup"><span data-stu-id="e62be-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e62be-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e62be-120">Authorization</span></span>  | <span data-ttu-id="e62be-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e62be-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e62be-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e62be-123">Request body</span></span>

<span data-ttu-id="e62be-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e62be-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e62be-125">応答</span><span class="sxs-lookup"><span data-stu-id="e62be-125">Response</span></span>

<span data-ttu-id="e62be-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e62be-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e62be-128">例</span><span class="sxs-lookup"><span data-stu-id="e62be-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="e62be-129">要求</span><span class="sxs-lookup"><span data-stu-id="e62be-129">Request</span></span>

<span data-ttu-id="e62be-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e62be-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "uninstall_teamsapp"
}-->

```http
DELETE /teams/{id}/installedApps/{id}
```

### <a name="response"></a><span data-ttu-id="e62be-131">応答</span><span class="sxs-lookup"><span data-stu-id="e62be-131">Response</span></span>

<span data-ttu-id="e62be-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e62be-132">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "uninstall_teamsapp",
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
