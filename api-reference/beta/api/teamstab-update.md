---
title: '[更新] タブ'
description: 指定したタブのプロパティを更新します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 75166f403a197f0abc32d4bc9f79f43a905fea43
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529916"
---
# <a name="update-tab"></a><span data-ttu-id="904b9-103">[更新] タブ</span><span class="sxs-lookup"><span data-stu-id="904b9-103">Update tab</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="904b9-104">指定した[タブ](../resources/teamstab.md)のプロパティを更新します。タブのコンテンツを構成するのには、これを使用できます。</span><span class="sxs-lookup"><span data-stu-id="904b9-104">Update the properties of the specified [tab](../resources/teamstab.md). This can be used to configure the content of the tab.</span></span>

## <a name="permissions"></a><span data-ttu-id="904b9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="904b9-105">Permissions</span></span>
<span data-ttu-id="904b9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="904b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="904b9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="904b9-108">Permission type</span></span>      | <span data-ttu-id="904b9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="904b9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="904b9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="904b9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="904b9-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="904b9-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="904b9-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="904b9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="904b9-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="904b9-113">Not supported.</span></span>    |
|<span data-ttu-id="904b9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="904b9-114">Application</span></span>                            | <span data-ttu-id="904b9-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="904b9-115">Group.ReadWrite.All</span></span>                         |

> <span data-ttu-id="904b9-116">**注**: この API は、管理者のアクセス許可をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="904b9-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="904b9-117">グローバル管理者とサービス管理者のマイクロソフトのチームのメンバーではないことをチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="904b9-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="904b9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="904b9-118">HTTP request</span></span>
```http
PATCH /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="904b9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="904b9-119">Request headers</span></span>
| <span data-ttu-id="904b9-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="904b9-120">Header</span></span>       | <span data-ttu-id="904b9-121">値</span><span class="sxs-lookup"><span data-stu-id="904b9-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="904b9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="904b9-122">Authorization</span></span>  | <span data-ttu-id="904b9-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="904b9-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="904b9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="904b9-125">Content-Type</span></span>  | <span data-ttu-id="904b9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="904b9-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="904b9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="904b9-127">Request body</span></span>
<span data-ttu-id="904b9-128">要求の本文には、 [tab](../resources/teamstab.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="904b9-128">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="904b9-129">応答</span><span class="sxs-lookup"><span data-stu-id="904b9-129">Response</span></span>

<span data-ttu-id="904b9-130">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="904b9-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="904b9-131">例</span><span class="sxs-lookup"><span data-stu-id="904b9-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="904b9-132">要求</span><span class="sxs-lookup"><span data-stu-id="904b9-132">Request</span></span>
<span data-ttu-id="904b9-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="904b9-133">The following is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
Content-type: application/json
Content-length: 211

{
  "name": "My Contoso Tab - updated"
}
```
#### <a name="response"></a><span data-ttu-id="904b9-134">応答</span><span class="sxs-lookup"><span data-stu-id="904b9-134">Response</span></span>
```http
HTTP/1.1 200 Success
Content-type: application/json

{
  "id": "tabId",
  "name": "My Contoso Tab - updated",
  "teamsAppId": "06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "sortOrderIndex": 20,
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```

## <a name="see-also"></a><span data-ttu-id="904b9-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="904b9-135">See also</span></span>

[<span data-ttu-id="904b9-136">組み込みタブのタイプを設定します。</span><span class="sxs-lookup"><span data-stu-id="904b9-136">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update tab in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/teamstab-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
