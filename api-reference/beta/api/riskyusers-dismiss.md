---
title: riskyUsers を閉じる
description: riskyUsers オブジェクトのリスクを無視します。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: 3027320b25c35e60e1b5dccabc7ff34ea642a953
ms.sourcegitcommit: 9fd437a77da99d8436d6c852edd99a9ba873f8cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/09/2019
ms.locfileid: "31560102"
---
# <a name="dismiss-riskyusers"></a><span data-ttu-id="db832-103">riskyUsers を閉じる</span><span class="sxs-lookup"><span data-stu-id="db832-103">Dismiss riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="db832-104">**注:** riskyUsers API を使用するには、Azure AD Premium P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="db832-104">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="db832-105">**riskyUser**オブジェクトのリスクを無視します。</span><span class="sxs-lookup"><span data-stu-id="db832-105">Dismiss the risk of a **riskyUser** object.</span></span> <span data-ttu-id="db832-106">このアクションは、対象ユーザーのリスクレベルを [なし] に設定します。</span><span class="sxs-lookup"><span data-stu-id="db832-106">This action will set the targeted user's risk level to none.</span></span>
## <a name="permissions"></a><span data-ttu-id="db832-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="db832-107">Permissions</span></span>
<span data-ttu-id="db832-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="db832-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db832-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="db832-110">Permission type</span></span>      | <span data-ttu-id="db832-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="db832-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db832-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="db832-112">Delegated (work or school account)</span></span> | <span data-ttu-id="db832-113">IdentityRiskyUser</span><span class="sxs-lookup"><span data-stu-id="db832-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="db832-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="db832-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db832-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="db832-115">Not supported.</span></span>    |
|<span data-ttu-id="db832-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="db832-116">Application</span></span> | <span data-ttu-id="db832-117">IdentityRiskyUser</span><span class="sxs-lookup"><span data-stu-id="db832-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db832-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="db832-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
```


## <a name="request-headers"></a><span data-ttu-id="db832-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="db832-119">Request headers</span></span>
| <span data-ttu-id="db832-120">名前</span><span class="sxs-lookup"><span data-stu-id="db832-120">Name</span></span>      |<span data-ttu-id="db832-121">説明</span><span class="sxs-lookup"><span data-stu-id="db832-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="db832-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="db832-122">Authorization</span></span>  | <span data-ttu-id="db832-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="db832-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="db832-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="db832-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="db832-126">変更を保存するかどうかを決定するブックセッション ID。</span><span class="sxs-lookup"><span data-stu-id="db832-126">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="db832-127">省略可能。</span><span class="sxs-lookup"><span data-stu-id="db832-127">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="db832-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="db832-128">Request body</span></span>
<span data-ttu-id="db832-129">要求本文で無視する userIds を指定します。</span><span class="sxs-lookup"><span data-stu-id="db832-129">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="db832-130">応答</span><span class="sxs-lookup"><span data-stu-id="db832-130">Response</span></span>

<span data-ttu-id="db832-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="db832-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="db832-133">例</span><span class="sxs-lookup"><span data-stu-id="db832-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db832-134">要求</span><span class="sxs-lookup"><span data-stu-id="db832-134">Request</span></span>
<span data-ttu-id="db832-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="db832-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "dismiss_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/dismiss
Content-Type: application/json

{
  "userIds": [
    "04487ee0-f4f6-4e7f-8999-facc5a30e232",
    "13387ee0-f4f6-4e7f-8999-facc5120e345"
  ]
}
```
##### <a name="response"></a><span data-ttu-id="db832-136">応答</span><span class="sxs-lookup"><span data-stu-id="db832-136">Response</span></span>
<span data-ttu-id="db832-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="db832-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Dismiss riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
