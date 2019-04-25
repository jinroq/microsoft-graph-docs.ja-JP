---
title: securityAction を取得する
description: securityAction オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: fcbecbd0c15efc493164929f769a79deb3cbd98a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545510"
---
# <a name="get-securityaction"></a><span data-ttu-id="67fae-103">securityAction を取得する</span><span class="sxs-lookup"><span data-stu-id="67fae-103">Get securityAction</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67fae-104">[securityAction](../resources/securityaction.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="67fae-104">Retrieve the properties and relationships of a [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="67fae-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="67fae-105">Permissions</span></span>

<span data-ttu-id="67fae-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67fae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="67fae-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="67fae-108">Permission type</span></span>                        | <span data-ttu-id="67fae-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="67fae-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="67fae-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="67fae-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="67fae-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67fae-111">Not supported.</span></span> |
| <span data-ttu-id="67fae-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="67fae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67fae-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67fae-113">Not supported.</span></span> |
| <span data-ttu-id="67fae-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="67fae-114">Application</span></span>                            | <span data-ttu-id="67fae-115">securityactions. all、securityactions. すべて</span><span class="sxs-lookup"><span data-stu-id="67fae-115">SecurityActions.Read.All, SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="67fae-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="67fae-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/securityActions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="67fae-117">省略可能なクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="67fae-117">Optional query parameters</span></span>

<span data-ttu-id="67fae-118">このメソッドは、応答をカスタマイズするための OData クエリパラメーターの一部をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="67fae-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="67fae-119">一般的な情報については、「 [OData クエリパラメーター](/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67fae-119">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="67fae-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67fae-120">Request headers</span></span>

| <span data-ttu-id="67fae-121">名前</span><span class="sxs-lookup"><span data-stu-id="67fae-121">Name</span></span>      |<span data-ttu-id="67fae-122">説明</span><span class="sxs-lookup"><span data-stu-id="67fae-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="67fae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="67fae-123">Authorization</span></span> | <span data-ttu-id="67fae-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="67fae-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="67fae-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="67fae-125">Request body</span></span>

<span data-ttu-id="67fae-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="67fae-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67fae-127">応答</span><span class="sxs-lookup"><span data-stu-id="67fae-127">Response</span></span>

<span data-ttu-id="67fae-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[securityAction](../resources/securityaction.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="67fae-128">If successful, this method returns a `200 OK` response code and a [securityAction](../resources/securityaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="67fae-129">例</span><span class="sxs-lookup"><span data-stu-id="67fae-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="67fae-130">要求</span><span class="sxs-lookup"><span data-stu-id="67fae-130">Request</span></span>

<span data-ttu-id="67fae-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="67fae-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_securityaction"
}-->

```http
GET https://graph.microsoft.com/beta/security/securityActions/{id}
```

### <a name="response"></a><span data-ttu-id="67fae-132">応答</span><span class="sxs-lookup"><span data-stu-id="67fae-132">Response</span></span>

<span data-ttu-id="67fae-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="67fae-133">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="67fae-134">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="67fae-134">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="67fae-135">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="67fae-135">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securityAction"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "actionReason": "actionReason-value",
  "appId": "appId-value",
  "azureTenantId": "azureTenantId-value",
  "clientContext": "clientContext-value",
  "completedDateTime": "datetime-value",
  "createdDateTime": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get securityAction",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
