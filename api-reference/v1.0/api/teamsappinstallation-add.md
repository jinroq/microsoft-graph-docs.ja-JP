---
title: アプリケーションをチームに追加します。
description: 指定されたチームには、アプリケーションをインストールします。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8332204de2c75235720d7b2652d029e9f145f576
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922376"
---
# <a name="add-app-to-team"></a><span data-ttu-id="45c6b-103">アプリケーションをチームに追加します。</span><span class="sxs-lookup"><span data-stu-id="45c6b-103">Add app to team</span></span>



<span data-ttu-id="45c6b-104">指定された[チーム](../resources/team.md)には、[アプリケーション](../resources/teamsapp.md)をインストールします。</span><span class="sxs-lookup"><span data-stu-id="45c6b-104">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="45c6b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="45c6b-105">Permissions</span></span>
<span data-ttu-id="45c6b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="45c6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45c6b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="45c6b-108">Permission type</span></span>      | <span data-ttu-id="45c6b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="45c6b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45c6b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="45c6b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="45c6b-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45c6b-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="45c6b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="45c6b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45c6b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45c6b-113">Not supported.</span></span>    |
|<span data-ttu-id="45c6b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="45c6b-114">Application</span></span> | <span data-ttu-id="45c6b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45c6b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="45c6b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="45c6b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="45c6b-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="45c6b-117">Request headers</span></span>
| <span data-ttu-id="45c6b-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="45c6b-118">Header</span></span>       | <span data-ttu-id="45c6b-119">値</span><span class="sxs-lookup"><span data-stu-id="45c6b-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="45c6b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="45c6b-120">Authorization</span></span>  | <span data-ttu-id="45c6b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="45c6b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="45c6b-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="45c6b-123">Request body</span></span>

| <span data-ttu-id="45c6b-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45c6b-124">Property</span></span>     | <span data-ttu-id="45c6b-125">種類</span><span class="sxs-lookup"><span data-stu-id="45c6b-125">Type</span></span>   |<span data-ttu-id="45c6b-126">説明</span><span class="sxs-lookup"><span data-stu-id="45c6b-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45c6b-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="45c6b-127">teamsApp</span></span>| [<span data-ttu-id="45c6b-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="45c6b-128">teamsApp</span></span>](../resources/teamsapp.md) |<span data-ttu-id="45c6b-129">追加するアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="45c6b-129">The app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="45c6b-130">応答</span><span class="sxs-lookup"><span data-stu-id="45c6b-130">Response</span></span>

<span data-ttu-id="45c6b-131">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="45c6b-131">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="45c6b-132">例</span><span class="sxs-lookup"><span data-stu-id="45c6b-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="45c6b-133">要求</span><span class="sxs-lookup"><span data-stu-id="45c6b-133">Request</span></span>
<span data-ttu-id="45c6b-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="45c6b-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST /teams/{id}/installedApps
{
   "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
#### <a name="response"></a><span data-ttu-id="45c6b-135">応答</span><span class="sxs-lookup"><span data-stu-id="45c6b-135">Response</span></span>
<span data-ttu-id="45c6b-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="45c6b-136">The following is an example of the response.</span></span> <span data-ttu-id="45c6b-137">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="45c6b-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="45c6b-138">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="45c6b-138">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

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

## <a name="see-also"></a><span data-ttu-id="45c6b-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="45c6b-139">See also</span></span>

