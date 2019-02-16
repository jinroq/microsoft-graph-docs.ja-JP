---
title: チームからアプリを削除する
description: 指定したチームからアプリをアンインストールします。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a4857a5e56a16eb9ee0989108fcfe3b185bb5f0c
ms.sourcegitcommit: 4e9acb8029aca36dfade509a25f1111e1bd0ec6d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/16/2019
ms.locfileid: "30070821"
---
# <a name="delete-app-from-team"></a><span data-ttu-id="33d23-103">チームからアプリを削除する</span><span class="sxs-lookup"><span data-stu-id="33d23-103">Delete app from team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33d23-104">指定した[チーム](../resources/team.md)から[アプリ](../resources/teamsappinstallation.md)をアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="33d23-104">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

><span data-ttu-id="33d23-105">**注:** アプリケーションのアクセス許可を使用している場合は、既知の問題が発生します。</span><span class="sxs-lookup"><span data-stu-id="33d23-105">**Note:** If you're using application permissions, a known issue will occur.</span></span> <span data-ttu-id="33d23-106">詳細については、「[既知の問題](/graph/known-issues)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="33d23-106">For details, see [known issues](/graph/known-issues).</span></span>

## <a name="permissions"></a><span data-ttu-id="33d23-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="33d23-107">Permissions</span></span>
<span data-ttu-id="33d23-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="33d23-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33d23-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="33d23-110">Permission type</span></span>      | <span data-ttu-id="33d23-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="33d23-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33d23-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="33d23-112">Delegated (work or school account)</span></span> | <span data-ttu-id="33d23-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33d23-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="33d23-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="33d23-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33d23-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33d23-115">Not supported.</span></span>    |
|<span data-ttu-id="33d23-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="33d23-116">Application</span></span> | <span data-ttu-id="33d23-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33d23-117">Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="33d23-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="33d23-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="33d23-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="33d23-119">Request headers</span></span>
| <span data-ttu-id="33d23-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="33d23-120">Header</span></span>       | <span data-ttu-id="33d23-121">値</span><span class="sxs-lookup"><span data-stu-id="33d23-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="33d23-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="33d23-122">Authorization</span></span>  | <span data-ttu-id="33d23-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="33d23-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="33d23-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="33d23-125">Request body</span></span>
<span data-ttu-id="33d23-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="33d23-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33d23-127">応答</span><span class="sxs-lookup"><span data-stu-id="33d23-127">Response</span></span>

<span data-ttu-id="33d23-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="33d23-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33d23-130">例</span><span class="sxs-lookup"><span data-stu-id="33d23-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="33d23-131">要求</span><span class="sxs-lookup"><span data-stu-id="33d23-131">Request</span></span>
<span data-ttu-id="33d23-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="33d23-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}
```
#### <a name="response"></a><span data-ttu-id="33d23-133">応答</span><span class="sxs-lookup"><span data-stu-id="33d23-133">Response</span></span>
<span data-ttu-id="33d23-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="33d23-134">The following is an example of the response.</span></span> <span data-ttu-id="33d23-135">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="33d23-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="33d23-136">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="33d23-136">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/teamsappinstallation-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
