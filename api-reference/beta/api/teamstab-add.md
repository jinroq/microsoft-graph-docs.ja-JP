---
title: チャネルにタブを追加します。
description: '(ピン) を追加、チーム内で指定したチャンネルをタブします。 '
ms.openlocfilehash: be246b0308be83e0b411fa89fe16034018756829
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068057"
---
# <a name="add-tab-to-channel"></a><span data-ttu-id="0acb7-103">チャネルにタブを追加します。</span><span class="sxs-lookup"><span data-stu-id="0acb7-103">Add tab to channel</span></span>

> <span data-ttu-id="0acb7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0acb7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0acb7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0acb7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0acb7-106">(ピン) を追加する[チーム](../resources/team.md)内で指定された[チャネル](../resources/channel.md)を[タブ](../resources/teamstab.md)します。</span><span class="sxs-lookup"><span data-stu-id="0acb7-106">Adds (pins) a [tab](../resources/teamstab.md) to the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="0acb7-107">対応するアプリケーションでは、[チームにインストールされている](../api/teamsappinstallation-add.md)ある必要があります。</span><span class="sxs-lookup"><span data-stu-id="0acb7-107">The corresponding app must already be [installed in the team](../api/teamsappinstallation-add.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0acb7-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0acb7-108">Permissions</span></span>
<span data-ttu-id="0acb7-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0acb7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0acb7-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0acb7-111">Permission type</span></span>      | <span data-ttu-id="0acb7-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0acb7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0acb7-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0acb7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0acb7-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0acb7-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0acb7-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0acb7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0acb7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0acb7-116">Not supported.</span></span>    |
| <span data-ttu-id="0acb7-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0acb7-117">Application</span></span>                            | <span data-ttu-id="0acb7-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0acb7-118">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0acb7-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0acb7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/tabs
```

## <a name="request-headers"></a><span data-ttu-id="0acb7-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0acb7-120">Request headers</span></span>
| <span data-ttu-id="0acb7-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0acb7-121">Header</span></span>       | <span data-ttu-id="0acb7-122">値</span><span class="sxs-lookup"><span data-stu-id="0acb7-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0acb7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0acb7-123">Authorization</span></span>  | <span data-ttu-id="0acb7-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0acb7-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0acb7-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0acb7-126">Request body</span></span>

<span data-ttu-id="0acb7-127">[TeamsTab](../resources/teamstab.md)。</span><span class="sxs-lookup"><span data-stu-id="0acb7-127">A [teamsTab](../resources/teamstab.md).</span></span>

## <a name="response"></a><span data-ttu-id="0acb7-128">応答</span><span class="sxs-lookup"><span data-stu-id="0acb7-128">Response</span></span>

<span data-ttu-id="0acb7-129">成功した場合、このメソッドは `201 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="0acb7-129">If successful, this method returns a `201 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0acb7-130">例</span><span class="sxs-lookup"><span data-stu-id="0acb7-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0acb7-131">要求</span><span class="sxs-lookup"><span data-stu-id="0acb7-131">Request</span></span>

<span data-ttu-id="0acb7-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0acb7-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs
{
  "name": "My Contoso Tab",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  }
}
```

#### <a name="response"></a><span data-ttu-id="0acb7-133">応答</span><span class="sxs-lookup"><span data-stu-id="0acb7-133">Response</span></span>

<span data-ttu-id="0acb7-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0acb7-134">The following is an example of the response.</span></span> <span data-ttu-id="0acb7-135">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="0acb7-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0acb7-136">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0acb7-136">All of the properties will be returned from an actual call.</span></span>
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
  "name": "My Contoso Tab",
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

## <a name="see-also"></a><span data-ttu-id="0acb7-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="0acb7-137">See also</span></span>

[<span data-ttu-id="0acb7-138">組み込みタブのタイプを設定します。</span><span class="sxs-lookup"><span data-stu-id="0acb7-138">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Add tab to channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
