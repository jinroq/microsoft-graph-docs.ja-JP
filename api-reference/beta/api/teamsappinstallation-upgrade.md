---
title: チーム内のアプリをアップグレードする
description: チーム内のアプリのインストールをアップグレードする
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0ab151203e3b2ec3ee863bae34a8feed0c6d1064
ms.sourcegitcommit: 4e9acb8029aca36dfade509a25f1111e1bd0ec6d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/16/2019
ms.locfileid: "30070807"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="62fe7-103">チーム内のアプリをアップグレードする</span><span class="sxs-lookup"><span data-stu-id="62fe7-103">Upgrade an app in a team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62fe7-104">[チーム](../resources/team.md)内の[アプリのインストール](../resources/teamsappinstallation.md)をアプリの最新バージョンにアップグレードします。</span><span class="sxs-lookup"><span data-stu-id="62fe7-104">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

><span data-ttu-id="62fe7-105">**注:** アプリケーションのアクセス許可を使用している場合は、既知の問題が発生します。</span><span class="sxs-lookup"><span data-stu-id="62fe7-105">**Note:** If you're using application permissions, a known issue will occur.</span></span> <span data-ttu-id="62fe7-106">詳細については、「[既知の問題](/graph/known-issues)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="62fe7-106">For details, see [known issues](/graph/known-issues).</span></span>

## <a name="permissions"></a><span data-ttu-id="62fe7-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="62fe7-107">Permissions</span></span>

<span data-ttu-id="62fe7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="62fe7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62fe7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="62fe7-110">Permission type</span></span>      | <span data-ttu-id="62fe7-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="62fe7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62fe7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="62fe7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="62fe7-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62fe7-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="62fe7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="62fe7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62fe7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62fe7-115">Not supported.</span></span>    |
|<span data-ttu-id="62fe7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="62fe7-116">Application</span></span> | <span data-ttu-id="62fe7-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62fe7-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="62fe7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="62fe7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="62fe7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="62fe7-119">Request headers</span></span>
| <span data-ttu-id="62fe7-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="62fe7-120">Header</span></span>       | <span data-ttu-id="62fe7-121">値</span><span class="sxs-lookup"><span data-stu-id="62fe7-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="62fe7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="62fe7-122">Authorization</span></span>  | <span data-ttu-id="62fe7-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="62fe7-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="62fe7-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="62fe7-125">Request body</span></span>
<span data-ttu-id="62fe7-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="62fe7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62fe7-127">応答</span><span class="sxs-lookup"><span data-stu-id="62fe7-127">Response</span></span>

<span data-ttu-id="62fe7-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="62fe7-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62fe7-130">例</span><span class="sxs-lookup"><span data-stu-id="62fe7-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="62fe7-131">要求</span><span class="sxs-lookup"><span data-stu-id="62fe7-131">Request</span></span>
<span data-ttu-id="62fe7-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="62fe7-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
#### <a name="response"></a><span data-ttu-id="62fe7-133">応答</span><span class="sxs-lookup"><span data-stu-id="62fe7-133">Response</span></span>
<span data-ttu-id="62fe7-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="62fe7-134">The following is an example of the response.</span></span> 

><span data-ttu-id="62fe7-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="62fe7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
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
    "Error: /api-reference/beta/api/teamsappinstallation-upgrade.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
