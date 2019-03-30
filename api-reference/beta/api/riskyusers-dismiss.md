---
title: riskyUsers を閉じる
description: riskyUsers オブジェクトのリスクを無視します。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: 8e7a64e5762808691c4997c83b112a17c9667d47
ms.sourcegitcommit: fd9f62fd9a6d311f98afe2e31afca8b818c402c2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/30/2019
ms.locfileid: "31013132"
---
# <a name="dismiss-riskyusers"></a><span data-ttu-id="02ec7-103">riskyUsers を閉じる</span><span class="sxs-lookup"><span data-stu-id="02ec7-103">Dismiss riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="02ec7-104">**注:** riskyUsers API を使用するには、Azure AD Premium P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="02ec7-104">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="02ec7-105">**riskyUsers**オブジェクトのリスクを無視します。</span><span class="sxs-lookup"><span data-stu-id="02ec7-105">Dismiss the risk of a **riskyUsers** object.</span></span> <span data-ttu-id="02ec7-106">このアクションは、対象ユーザーのリスクレベルを [なし] に設定します。</span><span class="sxs-lookup"><span data-stu-id="02ec7-106">This action will set the targeted user's risk level to none.</span></span>
## <a name="permissions"></a><span data-ttu-id="02ec7-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="02ec7-107">Permissions</span></span>
<span data-ttu-id="02ec7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="02ec7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02ec7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="02ec7-110">Permission type</span></span>      | <span data-ttu-id="02ec7-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="02ec7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02ec7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="02ec7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="02ec7-113">IdentityRiskyUser</span><span class="sxs-lookup"><span data-stu-id="02ec7-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="02ec7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="02ec7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02ec7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02ec7-115">Not supported.</span></span>    |
|<span data-ttu-id="02ec7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="02ec7-116">Application</span></span> | <span data-ttu-id="02ec7-117">IdentityRiskyUser</span><span class="sxs-lookup"><span data-stu-id="02ec7-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02ec7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="02ec7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
```


## <a name="request-headers"></a><span data-ttu-id="02ec7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="02ec7-119">Request headers</span></span>
| <span data-ttu-id="02ec7-120">名前</span><span class="sxs-lookup"><span data-stu-id="02ec7-120">Name</span></span>      |<span data-ttu-id="02ec7-121">説明</span><span class="sxs-lookup"><span data-stu-id="02ec7-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="02ec7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="02ec7-122">Authorization</span></span>  | <span data-ttu-id="02ec7-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="02ec7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="02ec7-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="02ec7-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="02ec7-126">変更を保存するかどうかを決定するブックセッション ID。</span><span class="sxs-lookup"><span data-stu-id="02ec7-126">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="02ec7-127">省略可能。</span><span class="sxs-lookup"><span data-stu-id="02ec7-127">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="02ec7-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="02ec7-128">Request body</span></span>
<span data-ttu-id="02ec7-129">要求本文で無視する userIds を指定します。</span><span class="sxs-lookup"><span data-stu-id="02ec7-129">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="02ec7-130">応答</span><span class="sxs-lookup"><span data-stu-id="02ec7-130">Response</span></span>

<span data-ttu-id="02ec7-131">成功した場合、このメソッドは `204 NoContent` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="02ec7-131">If successful, this method returns a `204 NoContent` response code.</span></span>
## <a name="example"></a><span data-ttu-id="02ec7-132">例</span><span class="sxs-lookup"><span data-stu-id="02ec7-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="02ec7-133">要求</span><span class="sxs-lookup"><span data-stu-id="02ec7-133">Request</span></span>
<span data-ttu-id="02ec7-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="02ec7-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "dismiss_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/dismiss

Request Body
{
  "userIds": [
    "04487ee0-f4f6-4e7f-8999-facc5a30e232",
    "13387ee0-f4f6-4e7f-8999-facc5120e345"
  ]
}
```
##### <a name="response"></a><span data-ttu-id="02ec7-135">応答</span><span class="sxs-lookup"><span data-stu-id="02ec7-135">Response</span></span>
<span data-ttu-id="02ec7-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="02ec7-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUsers"
} -->
```http
HTTP/1.1 204 NoContent
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
