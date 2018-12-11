---
title: タブを取得します。
description: 'プロパティと指定したタブの関係を取得します。 '
ms.openlocfilehash: 7bef495fbb37a878a291f2aac6004d386e932cbd
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222409"
---
# <a name="get-tab"></a><span data-ttu-id="9f750-103">タブを取得します。</span><span class="sxs-lookup"><span data-stu-id="9f750-103">Get tab</span></span>

> <span data-ttu-id="9f750-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9f750-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f750-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f750-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9f750-106">プロパティと、指定した[タブ](../resources/teamstab.md)の関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="9f750-106">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="9f750-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9f750-107">Permissions</span></span>
<span data-ttu-id="9f750-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9f750-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f750-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9f750-110">Permission type</span></span>      | <span data-ttu-id="9f750-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9f750-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f750-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9f750-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9f750-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f750-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9f750-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9f750-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f750-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f750-115">Not supported.</span></span>    |
|<span data-ttu-id="9f750-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9f750-116">Application</span></span> | <span data-ttu-id="9f750-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f750-117">Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="9f750-118">**注**: この API は、管理者のアクセス許可をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="9f750-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="9f750-119">グローバル管理者とサービス管理者のマイクロソフトのチームのメンバーではないことをチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="9f750-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="9f750-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9f750-120">HTTP request</span></span>
```http
GET /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9f750-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9f750-121">Optional query parameters</span></span>

<span data-ttu-id="9f750-122">このメソッドは、$select をサポートし、$ は、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)を展開します。</span><span class="sxs-lookup"><span data-stu-id="9f750-122">This method supports the $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f750-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9f750-123">Request headers</span></span>
| <span data-ttu-id="9f750-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9f750-124">Header</span></span>       | <span data-ttu-id="9f750-125">値</span><span class="sxs-lookup"><span data-stu-id="9f750-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9f750-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f750-126">Authorization</span></span>  | <span data-ttu-id="9f750-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9f750-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9f750-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="9f750-129">Request body</span></span>
<span data-ttu-id="9f750-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9f750-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f750-131">応答</span><span class="sxs-lookup"><span data-stu-id="9f750-131">Response</span></span>

<span data-ttu-id="9f750-132">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の[tab](../resources/teamstab.md)オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="9f750-132">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9f750-133">例</span><span class="sxs-lookup"><span data-stu-id="9f750-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9f750-134">要求</span><span class="sxs-lookup"><span data-stu-id="9f750-134">Request</span></span>
<span data-ttu-id="9f750-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9f750-135">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="9f750-136">応答</span><span class="sxs-lookup"><span data-stu-id="9f750-136">Response</span></span>
<span data-ttu-id="9f750-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9f750-137">The following is an example of the response.</span></span> 

><span data-ttu-id="9f750-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9f750-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get a channel tab",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
