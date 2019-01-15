---
title: タブを取得します。
description: 'プロパティと指定したタブの関係を取得します。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: dd23ffc6bcfdeb8821e2227331e2be801f348ce8
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016675"
---
# <a name="get-tab"></a><span data-ttu-id="59b5f-103">タブを取得します。</span><span class="sxs-lookup"><span data-stu-id="59b5f-103">Get tab</span></span>



<span data-ttu-id="59b5f-104">プロパティと、指定した[タブ](../resources/teamstab.md)の関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="59b5f-104">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="59b5f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="59b5f-105">Permissions</span></span>
<span data-ttu-id="59b5f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="59b5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59b5f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="59b5f-108">Permission type</span></span>      | <span data-ttu-id="59b5f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="59b5f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59b5f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="59b5f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="59b5f-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59b5f-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="59b5f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="59b5f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59b5f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="59b5f-113">Not supported.</span></span>    |
|<span data-ttu-id="59b5f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="59b5f-114">Application</span></span> | <span data-ttu-id="59b5f-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59b5f-115">Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="59b5f-116">**注**: この API は、管理者のアクセス許可をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="59b5f-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="59b5f-117">グローバル管理者とサービス管理者のマイクロソフトのチームのメンバーではないことをチームにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="59b5f-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="59b5f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="59b5f-118">HTTP request</span></span>
```http
GET /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="59b5f-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="59b5f-119">Optional query parameters</span></span>

<span data-ttu-id="59b5f-120">このメソッドは、$select をサポートし、$ は、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)を展開します。</span><span class="sxs-lookup"><span data-stu-id="59b5f-120">This method supports the $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="59b5f-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="59b5f-121">Request headers</span></span>
| <span data-ttu-id="59b5f-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="59b5f-122">Header</span></span>       | <span data-ttu-id="59b5f-123">値</span><span class="sxs-lookup"><span data-stu-id="59b5f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="59b5f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="59b5f-124">Authorization</span></span>  | <span data-ttu-id="59b5f-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="59b5f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="59b5f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="59b5f-127">Request body</span></span>
<span data-ttu-id="59b5f-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="59b5f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59b5f-129">応答</span><span class="sxs-lookup"><span data-stu-id="59b5f-129">Response</span></span>

<span data-ttu-id="59b5f-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の[tab](../resources/teamstab.md)オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="59b5f-130">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="59b5f-131">例</span><span class="sxs-lookup"><span data-stu-id="59b5f-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="59b5f-132">要求</span><span class="sxs-lookup"><span data-stu-id="59b5f-132">Request</span></span>
<span data-ttu-id="59b5f-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="59b5f-133">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="59b5f-134">応答</span><span class="sxs-lookup"><span data-stu-id="59b5f-134">Response</span></span>
<span data-ttu-id="59b5f-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="59b5f-135">The following is an example of the response.</span></span> 

><span data-ttu-id="59b5f-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="59b5f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
