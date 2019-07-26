---
title: アプリをチームに追加する
description: 指定したチームにアプリをインストールします。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 07e8a5989050a0323fdbcde8027e6c89bef0d454
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908467"
---
# <a name="add-app-to-team"></a><span data-ttu-id="e247e-103">アプリをチームに追加する</span><span class="sxs-lookup"><span data-stu-id="e247e-103">Add app to team</span></span>

<span data-ttu-id="e247e-104">指定した[チーム](../resources/team.md)に[アプリ](../resources/teamsapp.md)をインストールします。</span><span class="sxs-lookup"><span data-stu-id="e247e-104">Install an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e247e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e247e-105">Permissions</span></span>

<span data-ttu-id="e247e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e247e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e247e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e247e-108">Permission type</span></span>      | <span data-ttu-id="e247e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e247e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e247e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e247e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e247e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e247e-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e247e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e247e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e247e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e247e-113">Not supported.</span></span>    |
|<span data-ttu-id="e247e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e247e-114">Application</span></span> | <span data-ttu-id="e247e-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e247e-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e247e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e247e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="e247e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e247e-117">Request headers</span></span>

| <span data-ttu-id="e247e-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e247e-118">Header</span></span>       | <span data-ttu-id="e247e-119">値</span><span class="sxs-lookup"><span data-stu-id="e247e-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e247e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e247e-120">Authorization</span></span>  | <span data-ttu-id="e247e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e247e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e247e-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e247e-123">Request body</span></span>

| <span data-ttu-id="e247e-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e247e-124">Property</span></span>   | <span data-ttu-id="e247e-125">型</span><span class="sxs-lookup"><span data-stu-id="e247e-125">Type</span></span> |<span data-ttu-id="e247e-126">説明</span><span class="sxs-lookup"><span data-stu-id="e247e-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e247e-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e247e-127">teamsApp</span></span>| [<span data-ttu-id="e247e-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e247e-128">teamsApp</span></span>](../resources/teamsapp.md) |<span data-ttu-id="e247e-129">追加するアプリ。</span><span class="sxs-lookup"><span data-stu-id="e247e-129">The app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="e247e-130">応答</span><span class="sxs-lookup"><span data-stu-id="e247e-130">Response</span></span>

<span data-ttu-id="e247e-p103">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e247e-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e247e-133">例</span><span class="sxs-lookup"><span data-stu-id="e247e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e247e-134">要求</span><span class="sxs-lookup"><span data-stu-id="e247e-134">Request</span></span>

<span data-ttu-id="e247e-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e247e-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```

### <a name="response"></a><span data-ttu-id="e247e-136">応答</span><span class="sxs-lookup"><span data-stu-id="e247e-136">Response</span></span>

<span data-ttu-id="e247e-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e247e-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
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
