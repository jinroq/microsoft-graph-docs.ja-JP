---
title: アプリをチームに追加する
description: 指定したチームにアプリをインストールします。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 837528e20da88496ab4d9b1133e461cbc462df37
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330055"
---
# <a name="add-app-to-team"></a><span data-ttu-id="0cde1-103">アプリをチームに追加する</span><span class="sxs-lookup"><span data-stu-id="0cde1-103">Add app to team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cde1-104">指定した[チーム](../resources/team.md)に[アプリ](../resources/teamsapp.md)をインストールします。</span><span class="sxs-lookup"><span data-stu-id="0cde1-104">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0cde1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0cde1-105">Permissions</span></span>
<span data-ttu-id="0cde1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0cde1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cde1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0cde1-108">Permission type</span></span>      | <span data-ttu-id="0cde1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0cde1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0cde1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0cde1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0cde1-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cde1-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0cde1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0cde1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0cde1-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0cde1-113">Not supported.</span></span>    |
|<span data-ttu-id="0cde1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0cde1-114">Application</span></span> | <span data-ttu-id="0cde1-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cde1-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0cde1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0cde1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="0cde1-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0cde1-117">Request headers</span></span>
| <span data-ttu-id="0cde1-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0cde1-118">Header</span></span>       | <span data-ttu-id="0cde1-119">値</span><span class="sxs-lookup"><span data-stu-id="0cde1-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0cde1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cde1-120">Authorization</span></span>  | <span data-ttu-id="0cde1-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0cde1-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0cde1-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="0cde1-123">Request body</span></span>

| <span data-ttu-id="0cde1-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0cde1-124">Property</span></span>     | <span data-ttu-id="0cde1-125">型</span><span class="sxs-lookup"><span data-stu-id="0cde1-125">Type</span></span>   |<span data-ttu-id="0cde1-126">説明</span><span class="sxs-lookup"><span data-stu-id="0cde1-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0cde1-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="0cde1-127">teamsApp</span></span>|<span data-ttu-id="0cde1-128">String</span><span class="sxs-lookup"><span data-stu-id="0cde1-128">String</span></span>|<span data-ttu-id="0cde1-129">追加するアプリの id。</span><span class="sxs-lookup"><span data-stu-id="0cde1-129">The id of the app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="0cde1-130">応答</span><span class="sxs-lookup"><span data-stu-id="0cde1-130">Response</span></span>

<span data-ttu-id="0cde1-131">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="0cde1-131">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="0cde1-132">例</span><span class="sxs-lookup"><span data-stu-id="0cde1-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0cde1-133">要求</span><span class="sxs-lookup"><span data-stu-id="0cde1-133">Request</span></span>
<span data-ttu-id="0cde1-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0cde1-134">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="0cde1-135">応答</span><span class="sxs-lookup"><span data-stu-id="0cde1-135">Response</span></span>
<span data-ttu-id="0cde1-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0cde1-136">The following is an example of the response.</span></span> <span data-ttu-id="0cde1-137">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="0cde1-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0cde1-138">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0cde1-138">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

## <a name="see-also"></a><span data-ttu-id="0cde1-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="0cde1-139">See also</span></span>

