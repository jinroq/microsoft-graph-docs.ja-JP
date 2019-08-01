---
title: チャネルへのタブの追加
description: 'チーム内で指定されたチャネルにタブを追加 (ピン留め) します。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3a4eefc52f97b2d405f0f42b61d8e7163e8f812f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027231"
---
# <a name="add-tab-to-channel"></a><span data-ttu-id="02903-103">チャネルへのタブの追加</span><span class="sxs-lookup"><span data-stu-id="02903-103">Add tab to channel</span></span>



<span data-ttu-id="02903-104">[チーム内](../resources/team.md)で指定された[チャネル](../resources/channel.md)に[タブ](../resources/teamstab.md)を追加 (ピン留め) します。</span><span class="sxs-lookup"><span data-stu-id="02903-104">Adds (pins) a [tab](../resources/teamstab.md) to the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="02903-105">対応するアプリは、既に[チーム内にインストールされている](../api/teamsappinstallation-add.md)はずです。</span><span class="sxs-lookup"><span data-stu-id="02903-105">The corresponding app must already be [installed in the team](../api/teamsappinstallation-add.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="02903-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="02903-106">Permissions</span></span>
<span data-ttu-id="02903-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="02903-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02903-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="02903-109">Permission type</span></span>      | <span data-ttu-id="02903-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="02903-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02903-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="02903-111">Delegated (work or school account)</span></span> | <span data-ttu-id="02903-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02903-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="02903-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="02903-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02903-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02903-114">Not supported.</span></span>    |
| <span data-ttu-id="02903-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="02903-115">Application</span></span>                            | <span data-ttu-id="02903-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02903-116">Group.ReadWrite.All</span></span>                         |

> <span data-ttu-id="02903-117">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="02903-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="02903-118">グローバル管理者と Microsoft Teams サービス管理者は、メンバーではないチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="02903-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="02903-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="02903-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/tabs
```

## <a name="request-headers"></a><span data-ttu-id="02903-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="02903-120">Request headers</span></span>
| <span data-ttu-id="02903-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="02903-121">Header</span></span>       | <span data-ttu-id="02903-122">値</span><span class="sxs-lookup"><span data-stu-id="02903-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="02903-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="02903-123">Authorization</span></span>  | <span data-ttu-id="02903-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="02903-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="02903-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="02903-126">Request body</span></span>

<span data-ttu-id="02903-127">[teamsTab](../resources/teamstab.md)。</span><span class="sxs-lookup"><span data-stu-id="02903-127">A [teamsTab](../resources/teamstab.md).</span></span>

## <a name="response"></a><span data-ttu-id="02903-128">応答</span><span class="sxs-lookup"><span data-stu-id="02903-128">Response</span></span>

<span data-ttu-id="02903-129">成功した場合、このメソッドは `201 Created` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="02903-129">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="example"></a><span data-ttu-id="02903-130">例</span><span class="sxs-lookup"><span data-stu-id="02903-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="02903-131">要求</span><span class="sxs-lookup"><span data-stu-id="02903-131">Request</span></span>

<span data-ttu-id="02903-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="02903-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/tabs
{
  "displayName": "My Contoso Tab",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  }
}
```

#### <a name="response"></a><span data-ttu-id="02903-133">応答</span><span class="sxs-lookup"><span data-stu-id="02903-133">Response</span></span>

<span data-ttu-id="02903-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="02903-134">The following is an example of the response.</span></span> <span data-ttu-id="02903-135">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="02903-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="02903-136">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="02903-136">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
  "displayName": "My Contoso Tab",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "sortOrderIndex": "20",
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```

## <a name="see-also"></a><span data-ttu-id="02903-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="02903-137">See also</span></span>

[<span data-ttu-id="02903-138">組み込みタブ タイプの構成</span><span class="sxs-lookup"><span data-stu-id="02903-138">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add tab to channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
