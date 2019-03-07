---
title: チーム内のアプリをアップグレードする
description: チーム内のアプリのインストールをアップグレードする
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1000bcbb8aeaa26cd1b580bd4c11a4018a3a82f9
ms.sourcegitcommit: d1a9e7c8e1376a99c5a5416257889ec113613a77
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/07/2019
ms.locfileid: "30458646"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="64016-103">チーム内のアプリをアップグレードする</span><span class="sxs-lookup"><span data-stu-id="64016-103">Upgrade an app in a team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64016-104">[チーム](../resources/team.md)内の[アプリのインストール](../resources/teamsappinstallation.md)をアプリの最新バージョンにアップグレードします。</span><span class="sxs-lookup"><span data-stu-id="64016-104">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="64016-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="64016-105">Permissions</span></span>

<span data-ttu-id="64016-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="64016-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64016-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="64016-108">Permission type</span></span>      | <span data-ttu-id="64016-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="64016-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64016-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="64016-110">Delegated (work or school account)</span></span> | <span data-ttu-id="64016-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64016-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="64016-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="64016-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64016-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="64016-113">Not supported.</span></span>    |
|<span data-ttu-id="64016-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="64016-114">Application</span></span> | <span data-ttu-id="64016-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64016-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="64016-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="64016-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="64016-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="64016-117">Request headers</span></span>
| <span data-ttu-id="64016-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="64016-118">Header</span></span>       | <span data-ttu-id="64016-119">値</span><span class="sxs-lookup"><span data-stu-id="64016-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="64016-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="64016-120">Authorization</span></span>  | <span data-ttu-id="64016-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="64016-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="64016-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="64016-123">Request body</span></span>
<span data-ttu-id="64016-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="64016-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64016-125">応答</span><span class="sxs-lookup"><span data-stu-id="64016-125">Response</span></span>

<span data-ttu-id="64016-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="64016-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64016-128">例</span><span class="sxs-lookup"><span data-stu-id="64016-128">Example</span></span>

#### <a name="request"></a><span data-ttu-id="64016-129">要求</span><span class="sxs-lookup"><span data-stu-id="64016-129">Request</span></span>
<span data-ttu-id="64016-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="64016-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
#### <a name="response"></a><span data-ttu-id="64016-131">応答</span><span class="sxs-lookup"><span data-stu-id="64016-131">Response</span></span>
<span data-ttu-id="64016-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="64016-132">The following is an example of the response.</span></span> 

><span data-ttu-id="64016-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="64016-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
