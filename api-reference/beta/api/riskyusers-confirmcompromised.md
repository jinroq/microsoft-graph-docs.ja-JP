---
title: riskyUsers が侵害されたことを確認する
description: riskyUsers オブジェクトが侵害されていることを確認します。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: 9ae07bf8d1d4a41764aa145a9c7508da339d7ce2
ms.sourcegitcommit: fd9f62fd9a6d311f98afe2e31afca8b818c402c2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/30/2019
ms.locfileid: "31013125"
---
# <a name="confirm-riskyusers-compromised"></a><span data-ttu-id="b1af5-103">riskyUsers が侵害されたことを確認する</span><span class="sxs-lookup"><span data-stu-id="b1af5-103">Confirm riskyUsers compromised</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="b1af5-104">**注:** riskyUsers API には、Azure AD Premium P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="b1af5-104">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="b1af5-105">[riskyUsers](../resources/riskyuser.md)オブジェクトが侵害されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="b1af5-105">Confirm a [riskyUsers](../resources/riskyuser.md) object as compromised.</span></span> <span data-ttu-id="b1af5-106">これにより、対象ユーザーのリスクレベルが [高」に設定されます。</span><span class="sxs-lookup"><span data-stu-id="b1af5-106">This will set the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1af5-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b1af5-107">Permissions</span></span>
<span data-ttu-id="b1af5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b1af5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1af5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b1af5-110">Permission type</span></span>      | <span data-ttu-id="b1af5-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b1af5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1af5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b1af5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b1af5-113">IdentityRiskyUser</span><span class="sxs-lookup"><span data-stu-id="b1af5-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="b1af5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b1af5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1af5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1af5-115">Not supported.</span></span>    |
|<span data-ttu-id="b1af5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b1af5-116">Application</span></span> | <span data-ttu-id="b1af5-117">IdentityRiskyUser</span><span class="sxs-lookup"><span data-stu-id="b1af5-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1af5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b1af5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/confirmCompromised
```


## <a name="request-headers"></a><span data-ttu-id="b1af5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b1af5-119">Request headers</span></span>
| <span data-ttu-id="b1af5-120">名前</span><span class="sxs-lookup"><span data-stu-id="b1af5-120">Name</span></span>      |<span data-ttu-id="b1af5-121">説明</span><span class="sxs-lookup"><span data-stu-id="b1af5-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b1af5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1af5-122">Authorization</span></span>  | <span data-ttu-id="b1af5-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b1af5-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b1af5-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b1af5-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="b1af5-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="b1af5-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1af5-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="b1af5-128">Request body</span></span>
<span data-ttu-id="b1af5-129">要求本文で無視する userIds を指定します。</span><span class="sxs-lookup"><span data-stu-id="b1af5-129">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="b1af5-130">応答</span><span class="sxs-lookup"><span data-stu-id="b1af5-130">Response</span></span>

<span data-ttu-id="b1af5-131">成功した場合、このメソッド`204 No Content`は応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="b1af5-131">If successful, this method returns a `204 No Content` response code</span></span>
## <a name="example"></a><span data-ttu-id="b1af5-132">例</span><span class="sxs-lookup"><span data-stu-id="b1af5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1af5-133">要求</span><span class="sxs-lookup"><span data-stu-id="b1af5-133">Request</span></span>
<span data-ttu-id="b1af5-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b1af5-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "confirm_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/confirmCompromised


Request Body
{
  "userIds": [
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf",
    "20f91ec9-d140-4d90-9cd9-f618587a1471"
  ]
}
```
##### <a name="response"></a><span data-ttu-id="b1af5-135">応答</span><span class="sxs-lookup"><span data-stu-id="b1af5-135">Response</span></span>
<span data-ttu-id="b1af5-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b1af5-136">Here is an example of the response.</span></span>
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
  "description": "Confirm compromised riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyusers-confirmcompromised.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
