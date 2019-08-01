---
title: タブを取得する
description: '指定したタブのプロパティとリレーションシップを取得します。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3d630bcaddd46aaf1428a49035c5502f43be0bfc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027203"
---
# <a name="get-tab"></a><span data-ttu-id="16b72-103">タブを取得する</span><span class="sxs-lookup"><span data-stu-id="16b72-103">Get tab</span></span>



<span data-ttu-id="16b72-104">指定した[タブ](../resources/teamstab.md)のプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="16b72-104">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="16b72-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="16b72-105">Permissions</span></span>
<span data-ttu-id="16b72-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="16b72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16b72-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="16b72-108">Permission type</span></span>      | <span data-ttu-id="16b72-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="16b72-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16b72-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="16b72-110">Delegated (work or school account)</span></span> | <span data-ttu-id="16b72-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16b72-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="16b72-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="16b72-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16b72-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16b72-113">Not supported.</span></span>    |
|<span data-ttu-id="16b72-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="16b72-114">Application</span></span> | <span data-ttu-id="16b72-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16b72-115">Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="16b72-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="16b72-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="16b72-117">グローバル管理者と Microsoft Teams サービス管理者は、メンバーではないチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="16b72-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="16b72-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="16b72-118">HTTP request</span></span>
```http
GET /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="16b72-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="16b72-119">Optional query parameters</span></span>

<span data-ttu-id="16b72-120">このメソッドは、応答をカスタマイズするための $select、および $expand [OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="16b72-120">This method supports the $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16b72-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16b72-121">Request headers</span></span>
| <span data-ttu-id="16b72-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16b72-122">Header</span></span>       | <span data-ttu-id="16b72-123">値</span><span class="sxs-lookup"><span data-stu-id="16b72-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="16b72-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="16b72-124">Authorization</span></span>  | <span data-ttu-id="16b72-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="16b72-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="16b72-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="16b72-127">Request body</span></span>
<span data-ttu-id="16b72-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="16b72-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16b72-129">応答</span><span class="sxs-lookup"><span data-stu-id="16b72-129">Response</span></span>

<span data-ttu-id="16b72-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[tab](../resources/teamstab.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="16b72-130">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="16b72-131">例</span><span class="sxs-lookup"><span data-stu-id="16b72-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="16b72-132">要求</span><span class="sxs-lookup"><span data-stu-id="16b72-132">Request</span></span>
<span data-ttu-id="16b72-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="16b72-133">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/tabs/{id}?$expand=teamsApp
```
#### <a name="response"></a><span data-ttu-id="16b72-134">応答</span><span class="sxs-lookup"><span data-stu-id="16b72-134">Response</span></span>
<span data-ttu-id="16b72-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="16b72-135">The following is an example of the response.</span></span> 

><span data-ttu-id="16b72-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="16b72-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "tabId",
  "displayName": "My Contoso Tab - updated",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "teamsApp": {
      "id": "0d820ecd-def2-4297-adad-78056cde7c78",
      "externalId": null,
      "displayName": "Contoso",
      "distributionMethod": "store"
  },
  "sortOrderIndex": "20",
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a channel tab",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
