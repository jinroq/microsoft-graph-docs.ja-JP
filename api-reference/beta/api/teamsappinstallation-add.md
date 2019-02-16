---
title: アプリをチームに追加する
description: 指定したチームにアプリをインストールします。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 261d186e23b516e58a428ecfdd2883f7a3bc111d
ms.sourcegitcommit: 4e9acb8029aca36dfade509a25f1111e1bd0ec6d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/16/2019
ms.locfileid: "30070828"
---
# <a name="add-app-to-team"></a><span data-ttu-id="901c8-103">アプリをチームに追加する</span><span class="sxs-lookup"><span data-stu-id="901c8-103">Add app to team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="901c8-104">指定した[チーム](../resources/team.md)に[アプリ](../resources/teamsapp.md)をインストールします。</span><span class="sxs-lookup"><span data-stu-id="901c8-104">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

><span data-ttu-id="901c8-105">**注:** アプリケーションのアクセス許可を使用している場合は、既知の問題が発生します。</span><span class="sxs-lookup"><span data-stu-id="901c8-105">**Note:** If you're using application permissions, a known issue will occur.</span></span> <span data-ttu-id="901c8-106">詳細については、「[既知の問題](/graph/known-issues)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="901c8-106">For details, see [known issues](/graph/known-issues).</span></span>

## <a name="permissions"></a><span data-ttu-id="901c8-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="901c8-107">Permissions</span></span>
<span data-ttu-id="901c8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="901c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="901c8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="901c8-110">Permission type</span></span>      | <span data-ttu-id="901c8-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="901c8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="901c8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="901c8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="901c8-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="901c8-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="901c8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="901c8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="901c8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="901c8-115">Not supported.</span></span>    |
|<span data-ttu-id="901c8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="901c8-116">Application</span></span> | <span data-ttu-id="901c8-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="901c8-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="901c8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="901c8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="901c8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="901c8-119">Request headers</span></span>
| <span data-ttu-id="901c8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="901c8-120">Header</span></span>       | <span data-ttu-id="901c8-121">値</span><span class="sxs-lookup"><span data-stu-id="901c8-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="901c8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="901c8-122">Authorization</span></span>  | <span data-ttu-id="901c8-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="901c8-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="901c8-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="901c8-125">Request body</span></span>

| <span data-ttu-id="901c8-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="901c8-126">Property</span></span>     | <span data-ttu-id="901c8-127">型</span><span class="sxs-lookup"><span data-stu-id="901c8-127">Type</span></span>   |<span data-ttu-id="901c8-128">説明</span><span class="sxs-lookup"><span data-stu-id="901c8-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="901c8-129">teamsApp</span><span class="sxs-lookup"><span data-stu-id="901c8-129">teamsApp</span></span>|<span data-ttu-id="901c8-130">String</span><span class="sxs-lookup"><span data-stu-id="901c8-130">String</span></span>|<span data-ttu-id="901c8-131">追加するアプリの id。</span><span class="sxs-lookup"><span data-stu-id="901c8-131">The id of the app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="901c8-132">応答</span><span class="sxs-lookup"><span data-stu-id="901c8-132">Response</span></span>

<span data-ttu-id="901c8-133">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="901c8-133">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="901c8-134">例</span><span class="sxs-lookup"><span data-stu-id="901c8-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="901c8-135">要求</span><span class="sxs-lookup"><span data-stu-id="901c8-135">Request</span></span>
<span data-ttu-id="901c8-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="901c8-136">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="901c8-137">応答</span><span class="sxs-lookup"><span data-stu-id="901c8-137">Response</span></span>
<span data-ttu-id="901c8-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="901c8-138">The following is an example of the response.</span></span> <span data-ttu-id="901c8-139">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="901c8-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="901c8-140">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="901c8-140">All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/teamsappinstallation-add.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

## <a name="see-also"></a><span data-ttu-id="901c8-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="901c8-141">See also</span></span>

