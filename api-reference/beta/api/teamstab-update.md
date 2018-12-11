---
title: '[更新] タブ'
description: 指定したタブのプロパティを更新します。
ms.openlocfilehash: bc25830411f93ed1644b86c1228f987c091db32a
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222563"
---
# <a name="update-tab"></a><span data-ttu-id="b62c2-103">[更新] タブ</span><span class="sxs-lookup"><span data-stu-id="b62c2-103">Update tab</span></span>

> <span data-ttu-id="b62c2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b62c2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b62c2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b62c2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b62c2-106">指定した[タブ](../resources/teamstab.md)のプロパティを更新します。タブのコンテンツを構成するのには、これを使用できます。</span><span class="sxs-lookup"><span data-stu-id="b62c2-106">Update the properties of the specified [tab](../resources/teamstab.md). This can be used to configure the content of the tab.</span></span>

## <a name="permissions"></a><span data-ttu-id="b62c2-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b62c2-107">Permissions</span></span>
<span data-ttu-id="b62c2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b62c2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b62c2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b62c2-110">Permission type</span></span>      | <span data-ttu-id="b62c2-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b62c2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b62c2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b62c2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b62c2-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b62c2-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b62c2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b62c2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b62c2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b62c2-115">Not supported.</span></span>    |
|<span data-ttu-id="b62c2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b62c2-116">Application</span></span>                            | <span data-ttu-id="b62c2-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b62c2-117">Group.ReadWrite.All</span></span>                         |

> <span data-ttu-id="b62c2-118">**注**: この API は、管理者のアクセス許可をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="b62c2-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="b62c2-119">グローバル管理者とサービス管理者のマイクロソフトのチームのメンバーではないことをチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="b62c2-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="b62c2-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b62c2-120">HTTP request</span></span>
```http
PATCH /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b62c2-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b62c2-121">Request headers</span></span>
| <span data-ttu-id="b62c2-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b62c2-122">Header</span></span>       | <span data-ttu-id="b62c2-123">値</span><span class="sxs-lookup"><span data-stu-id="b62c2-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b62c2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b62c2-124">Authorization</span></span>  | <span data-ttu-id="b62c2-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b62c2-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b62c2-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b62c2-127">Content-Type</span></span>  | <span data-ttu-id="b62c2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b62c2-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b62c2-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="b62c2-129">Request body</span></span>
<span data-ttu-id="b62c2-130">要求の本文には、 [tab](../resources/teamstab.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="b62c2-130">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b62c2-131">応答</span><span class="sxs-lookup"><span data-stu-id="b62c2-131">Response</span></span>

<span data-ttu-id="b62c2-132">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="b62c2-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b62c2-133">例</span><span class="sxs-lookup"><span data-stu-id="b62c2-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b62c2-134">要求</span><span class="sxs-lookup"><span data-stu-id="b62c2-134">Request</span></span>
<span data-ttu-id="b62c2-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b62c2-135">The following is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
Content-type: application/json
Content-length: 211

{
  "name": "My Contoso Tab - updated"
}
```
#### <a name="response"></a><span data-ttu-id="b62c2-136">応答</span><span class="sxs-lookup"><span data-stu-id="b62c2-136">Response</span></span>
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

## <a name="see-also"></a><span data-ttu-id="b62c2-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="b62c2-137">See also</span></span>

[<span data-ttu-id="b62c2-138">組み込みタブのタイプを設定します。</span><span class="sxs-lookup"><span data-stu-id="b62c2-138">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tab in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
