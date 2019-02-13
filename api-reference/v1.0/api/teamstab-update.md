---
title: タブを更新する
description: 指定したタブのプロパティを更新します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9aff620ce98b729d428ff15f303025d20a21caa3
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967005"
---
# <a name="update-tab"></a><span data-ttu-id="be2e8-103">タブを更新する</span><span class="sxs-lookup"><span data-stu-id="be2e8-103">Update tab</span></span>


<span data-ttu-id="be2e8-104">指定した[タブ](../resources/teamstab.md)のプロパティを更新します。タブのコンテンツを構成するのには、これを使用できます。</span><span class="sxs-lookup"><span data-stu-id="be2e8-104">Update the properties of the specified [tab](../resources/teamstab.md). This can be used to configure the content of the tab.</span></span>

## <a name="permissions"></a><span data-ttu-id="be2e8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="be2e8-105">Permissions</span></span>
<span data-ttu-id="be2e8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be2e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="be2e8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="be2e8-108">Permission type</span></span>      | <span data-ttu-id="be2e8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="be2e8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be2e8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="be2e8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="be2e8-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be2e8-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="be2e8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="be2e8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be2e8-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be2e8-113">Not supported.</span></span>    |
|<span data-ttu-id="be2e8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="be2e8-114">Application</span></span>                            | <span data-ttu-id="be2e8-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be2e8-115">Group.ReadWrite.All</span></span>                         |

> <span data-ttu-id="be2e8-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="be2e8-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="be2e8-117">グローバル管理者と Microsoft Teams サービス管理者は、メンバーではないチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="be2e8-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="be2e8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="be2e8-118">HTTP request</span></span>
```http
PATCH /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="be2e8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="be2e8-119">Request headers</span></span>
| <span data-ttu-id="be2e8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="be2e8-120">Header</span></span>       | <span data-ttu-id="be2e8-121">値</span><span class="sxs-lookup"><span data-stu-id="be2e8-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="be2e8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="be2e8-122">Authorization</span></span>  | <span data-ttu-id="be2e8-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="be2e8-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="be2e8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="be2e8-125">Content-Type</span></span>  | <span data-ttu-id="be2e8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="be2e8-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="be2e8-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="be2e8-127">Request body</span></span>
<span data-ttu-id="be2e8-128">要求の本文には、 [tab](../resources/teamstab.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="be2e8-128">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="be2e8-129">応答</span><span class="sxs-lookup"><span data-stu-id="be2e8-129">Response</span></span>

<span data-ttu-id="be2e8-130">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="be2e8-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="be2e8-131">例</span><span class="sxs-lookup"><span data-stu-id="be2e8-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="be2e8-132">要求</span><span class="sxs-lookup"><span data-stu-id="be2e8-132">Request</span></span>
<span data-ttu-id="be2e8-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="be2e8-133">The following is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/tabs/{id}
Content-type: application/json
Content-length: 211

{
  "displayName": "My Contoso Tab - updated"
}
```
#### <a name="response"></a><span data-ttu-id="be2e8-134">応答</span><span class="sxs-lookup"><span data-stu-id="be2e8-134">Response</span></span>
```http
HTTP/1.1 200 Success
Content-type: application/json

{
  "id": "tabId",
  "displayName": "My Contoso Tab - updated",
  "teamsAppId": "06805b9e-77e3-4b93-ac81-525eb87513b8",
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

## <a name="see-also"></a><span data-ttu-id="be2e8-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="be2e8-135">See also</span></span>

[<span data-ttu-id="be2e8-136">組み込みタブ タイプの構成</span><span class="sxs-lookup"><span data-stu-id="be2e8-136">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update tab in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
