---
title: セキュリティアクションを一覧表示する
description: securityaction オブジェクトのリストを取得します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 54330bcf2116d0a9c715649bcd19bc0553579c4e
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366904"
---
# <a name="list-security-actions"></a><span data-ttu-id="d7fc4-103">セキュリティアクションを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d7fc4-103">List security actions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7fc4-104">[securityAction](../resources/securityaction.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="d7fc4-104">Retrieve a list of [securityAction](../resources/securityaction.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7fc4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d7fc4-105">Permissions</span></span>

<span data-ttu-id="d7fc4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7fc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d7fc4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d7fc4-108">Permission type</span></span>                        | <span data-ttu-id="d7fc4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d7fc4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d7fc4-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d7fc4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d7fc4-111">securityactions. all、securityactions. すべて</span><span class="sxs-lookup"><span data-stu-id="d7fc4-111">SecurityActions.Read.All, SecurityActions.ReadWrite.All</span></span> |
| <span data-ttu-id="d7fc4-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d7fc4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7fc4-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7fc4-113">Not supported.</span></span> |
| <span data-ttu-id="d7fc4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d7fc4-114">Application</span></span>                            | <span data-ttu-id="d7fc4-115">securityactions. all、securityactions. すべて</span><span class="sxs-lookup"><span data-stu-id="d7fc4-115">SecurityActions.Read.All, SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7fc4-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d7fc4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/securityActions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d7fc4-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d7fc4-117">Optional query parameters</span></span>

<span data-ttu-id="d7fc4-118">このメソッドは、応答をカスタマイズするための OData クエリパラメーターの一部をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="d7fc4-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d7fc4-119">一般的な情報については、「 [OData クエリパラメーター](/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7fc4-119">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d7fc4-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d7fc4-120">Request headers</span></span>

| <span data-ttu-id="d7fc4-121">名前</span><span class="sxs-lookup"><span data-stu-id="d7fc4-121">Name</span></span>      |<span data-ttu-id="d7fc4-122">説明</span><span class="sxs-lookup"><span data-stu-id="d7fc4-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d7fc4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7fc4-123">Authorization</span></span> | <span data-ttu-id="d7fc4-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d7fc4-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7fc4-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d7fc4-125">Request body</span></span>

<span data-ttu-id="d7fc4-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d7fc4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7fc4-127">応答</span><span class="sxs-lookup"><span data-stu-id="d7fc4-127">Response</span></span>

<span data-ttu-id="d7fc4-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[securityAction](../resources/securityaction.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d7fc4-128">If successful, this method returns a `200 OK` response code and a collection of [securityAction](../resources/securityaction.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d7fc4-129">例</span><span class="sxs-lookup"><span data-stu-id="d7fc4-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d7fc4-130">要求</span><span class="sxs-lookup"><span data-stu-id="d7fc4-130">Request</span></span>

<span data-ttu-id="d7fc4-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d7fc4-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_securityactions"
}-->

```http
GET https://graph.microsoft.com/beta/security/securityActions
```

### <a name="response"></a><span data-ttu-id="d7fc4-132">応答</span><span class="sxs-lookup"><span data-stu-id="d7fc4-132">Response</span></span>

<span data-ttu-id="d7fc4-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d7fc4-133">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="d7fc4-134">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="d7fc4-134">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d7fc4-135">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d7fc4-135">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securityAction",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "actionReason": "actionReason-value",
      "appId": "appId-value",
      "azureTenantId": "azureTenantId-value",
      "clientContext": "clientContext-value",
      "completedDateTime": "datetime-value",
      "createdDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List securityActions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
