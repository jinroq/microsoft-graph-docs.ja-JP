---
title: riskyUsers が侵害されたことを確認する
description: riskyUsers オブジェクトが侵害されていることを確認します。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: beca64415a2d03898d57cd9cda2fb248121c424b
ms.sourcegitcommit: 9fd437a77da99d8436d6c852edd99a9ba873f8cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/09/2019
ms.locfileid: "31559976"
---
# <a name="confirm-riskyusers-compromised"></a><span data-ttu-id="054d9-103">riskyUsers が侵害されたことを確認する</span><span class="sxs-lookup"><span data-stu-id="054d9-103">Confirm riskyUsers compromised</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="054d9-104">**注:** riskyUsers API には、Azure AD Premium P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="054d9-104">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="054d9-105">[riskyUser](../resources/riskyuser.md)オブジェクトが侵害されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="054d9-105">Confirm a [riskyUser](../resources/riskyuser.md) object as compromised.</span></span> <span data-ttu-id="054d9-106">これにより、対象ユーザーのリスクレベルが [高」に設定されます。</span><span class="sxs-lookup"><span data-stu-id="054d9-106">This will set the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="054d9-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="054d9-107">Permissions</span></span>
<span data-ttu-id="054d9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="054d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="054d9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="054d9-110">Permission type</span></span>      | <span data-ttu-id="054d9-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="054d9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="054d9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="054d9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="054d9-113">IdentityRiskyUser</span><span class="sxs-lookup"><span data-stu-id="054d9-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="054d9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="054d9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="054d9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="054d9-115">Not supported.</span></span>    |
|<span data-ttu-id="054d9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="054d9-116">Application</span></span> | <span data-ttu-id="054d9-117">IdentityRiskyUser</span><span class="sxs-lookup"><span data-stu-id="054d9-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="054d9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="054d9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/confirmCompromised
```


## <a name="request-headers"></a><span data-ttu-id="054d9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="054d9-119">Request headers</span></span>
| <span data-ttu-id="054d9-120">名前</span><span class="sxs-lookup"><span data-stu-id="054d9-120">Name</span></span>      |<span data-ttu-id="054d9-121">説明</span><span class="sxs-lookup"><span data-stu-id="054d9-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="054d9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="054d9-122">Authorization</span></span>  | <span data-ttu-id="054d9-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="054d9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="054d9-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="054d9-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="054d9-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="054d9-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="054d9-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="054d9-128">Request body</span></span>
<span data-ttu-id="054d9-129">要求本文で無視する userIds を指定します。</span><span class="sxs-lookup"><span data-stu-id="054d9-129">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="054d9-130">応答</span><span class="sxs-lookup"><span data-stu-id="054d9-130">Response</span></span>

<span data-ttu-id="054d9-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="054d9-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="054d9-133">例</span><span class="sxs-lookup"><span data-stu-id="054d9-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="054d9-134">要求</span><span class="sxs-lookup"><span data-stu-id="054d9-134">Request</span></span>
<span data-ttu-id="054d9-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="054d9-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "confirm_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/confirmCompromised
Content-type: application/json

{
  "userIds": [
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf",
    "20f91ec9-d140-4d90-9cd9-f618587a1471"
  ]
}
```
##### <a name="response"></a><span data-ttu-id="054d9-136">応答</span><span class="sxs-lookup"><span data-stu-id="054d9-136">Response</span></span>
<span data-ttu-id="054d9-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="054d9-137">Here is an example of the response.</span></span>
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
  "description": "Confirm compromised riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->
