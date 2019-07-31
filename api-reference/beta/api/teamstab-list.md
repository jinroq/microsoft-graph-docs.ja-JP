---
title: チャネル内のリストタブ
description: 'チーム内の指定されたチャネルのタブのリストを取得します。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a5521b0f450dc8c05f886a83dcf554f6f3315f68
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987944"
---
# <a name="list-tabs-in-channel"></a><span data-ttu-id="1e2b4-103">チャネル内のリストタブ</span><span class="sxs-lookup"><span data-stu-id="1e2b4-103">List tabs in channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e2b4-104">[チーム](../resources/team.md)内の指定された[チャネル](../resources/channel.md)の[タブ](../resources/teamstab.md)のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="1e2b4-104">Retrieve the list of [tabs](../resources/teamstab.md) in the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="1e2b4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1e2b4-105">Permissions</span></span>
<span data-ttu-id="1e2b4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e2b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e2b4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1e2b4-108">Permission type</span></span>      | <span data-ttu-id="1e2b4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e2b4-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1e2b4-111">グループ読み取り。すべてを取得します。</span><span class="sxs-lookup"><span data-stu-id="1e2b4-111">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="1e2b4-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1e2b4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e2b4-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e2b4-113">Not supported.</span></span>    |
| <span data-ttu-id="1e2b4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1e2b4-114">Application</span></span>                            | <span data-ttu-id="1e2b4-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e2b4-115">Group.Read.All, Group.ReadWrite.All</span></span>         |

> <span data-ttu-id="1e2b4-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1e2b4-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="1e2b4-117">グローバル管理者と Microsoft Teams サービス管理者は、メンバーではないチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="1e2b4-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1e2b4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1e2b4-118">HTTP request</span></span>

```http
GET /teams/{id}/channels/{id}/tabs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1e2b4-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1e2b4-119">Optional query parameters</span></span>

<span data-ttu-id="1e2b4-120">このメソッドは、応答をカスタマイズするための $filter、$select、および $expand [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1e2b4-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1e2b4-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e2b4-121">Request headers</span></span>
| <span data-ttu-id="1e2b4-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e2b4-122">Header</span></span>       | <span data-ttu-id="1e2b4-123">値</span><span class="sxs-lookup"><span data-stu-id="1e2b4-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1e2b4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e2b4-124">Authorization</span></span>  | <span data-ttu-id="1e2b4-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1e2b4-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1e2b4-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1e2b4-127">Request body</span></span>
<span data-ttu-id="1e2b4-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1e2b4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e2b4-129">応答</span><span class="sxs-lookup"><span data-stu-id="1e2b4-129">Response</span></span>
<span data-ttu-id="1e2b4-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[tabs](../resources/teamstab.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1e2b4-130">If successful, this method returns a `200 OK` response code and collection of [tabs](../resources/teamstab.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e2b4-131">例</span><span class="sxs-lookup"><span data-stu-id="1e2b4-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1e2b4-132">要求</span><span class="sxs-lookup"><span data-stu-id="1e2b4-132">Request</span></span>
<span data-ttu-id="1e2b4-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1e2b4-133">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs?$expand=teamsApp
```

#### <a name="response"></a><span data-ttu-id="1e2b4-134">応答</span><span class="sxs-lookup"><span data-stu-id="1e2b4-134">Response</span></span>
<span data-ttu-id="1e2b4-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1e2b4-135">The following is an example of the response.</span></span>
><span data-ttu-id="1e2b4-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1e2b4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 Success
Content-type: application/json

{
  "value": [
    {
      "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
      "displayName": "My Contoso Tab - updated",
      "configuration": {
        "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
        "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
        "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
        "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
      },
      "sortOrderIndex": "20",
      "teamsApp": {
        "id": "06805b9e-77e3-4b93-ac81-525eb87513b8",
        "displayName": "Contoso",
        "distributionMethod": "store"
      },
      "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
    },
    {
      "id": "b5d5f001-0471-49a5-aac4-04ef96683be0",
      "displayName": "My Planner Tab",
      "configuration": null,
      "sortOrderIndex": "21",
      "teamsApp": {
        "id": "com.microsoft.teamspace.tab.planner",
        "displayName": "Microsoft Planner",
        "distributionMethod": "store"
      },
      "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3a3709b35c-a0ba-467c-8001-0f66895fb9d3?label=My%20Planner%Tab"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List all tabs in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
