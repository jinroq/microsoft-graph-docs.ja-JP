---
title: 既存の同期テンプレートを一覧表示する
description: 特定のアプリケーションまたはサービスプリンシパルに関連付けられている同期テンプレートを一覧表示します。
localization_priority: Normal
ms.openlocfilehash: 01ddd6f02bfab06be6e2111e6bd0169492449b9d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271233"
---
# <a name="list-existing-synchronization-templates"></a><span data-ttu-id="c3eb8-103">既存の同期テンプレートを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c3eb8-103">List existing synchronization templates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3eb8-104">特定のアプリケーションまたはサービスプリンシパルに関連付けられている同期テンプレートを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="c3eb8-104">List the synchronization templates associated with a given application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3eb8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c3eb8-105">Permissions</span></span>
<span data-ttu-id="c3eb8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3eb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3eb8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c3eb8-108">Permission type</span></span>                        | <span data-ttu-id="c3eb8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c3eb8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3eb8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c3eb8-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="c3eb8-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3eb8-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="c3eb8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c3eb8-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="c3eb8-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3eb8-113">Not supported.</span></span>|
|<span data-ttu-id="c3eb8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c3eb8-114">Application</span></span>                            |<span data-ttu-id="c3eb8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3eb8-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="c3eb8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c3eb8-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET servicePrincipals/{id}/synchronization/templates
GET applications/{id}/synchronization/templates
```

## <a name="request-headers"></a><span data-ttu-id="c3eb8-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3eb8-117">Request headers</span></span>

| <span data-ttu-id="c3eb8-118">名前</span><span class="sxs-lookup"><span data-stu-id="c3eb8-118">Name</span></span>           | <span data-ttu-id="c3eb8-119">型</span><span class="sxs-lookup"><span data-stu-id="c3eb8-119">Type</span></span>    | <span data-ttu-id="c3eb8-120">説明</span><span class="sxs-lookup"><span data-stu-id="c3eb8-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="c3eb8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3eb8-121">Authorization</span></span>  | <span data-ttu-id="c3eb8-122">string</span><span class="sxs-lookup"><span data-stu-id="c3eb8-122">string</span></span>  | <span data-ttu-id="c3eb8-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c3eb8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3eb8-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c3eb8-125">Request body</span></span>

<span data-ttu-id="c3eb8-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c3eb8-126">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="c3eb8-127">応答</span><span class="sxs-lookup"><span data-stu-id="c3eb8-127">Response</span></span>

<span data-ttu-id="c3eb8-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[同期テンプレート](../resources/synchronization-synchronizationtemplate.md)オブジェクトの acollection を返します。</span><span class="sxs-lookup"><span data-stu-id="c3eb8-128">If successful, this method returns a `200 OK` response code and acollection of [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) objects in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="c3eb8-129">例</span><span class="sxs-lookup"><span data-stu-id="c3eb8-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c3eb8-130">要求</span><span class="sxs-lookup"><span data-stu-id="c3eb8-130">Request</span></span>
<span data-ttu-id="c3eb8-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c3eb8-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationtemplate"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates
```

##### <a name="response"></a><span data-ttu-id="c3eb8-132">応答</span><span class="sxs-lookup"><span data-stu-id="c3eb8-132">Response</span></span>
<span data-ttu-id="c3eb8-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c3eb8-133">The following is an example of a response.</span></span>
><span data-ttu-id="c3eb8-134">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="c3eb8-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c3eb8-135">実際の呼び出しでは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c3eb8-135">All the properties will be returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
    "value": [
        {
            "id": "Slack",
            "factoryTag": "CustomSCIM",
            "schema": {
                    "directories": [],
                    "synchronizationRules": []
                    }
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c3eb8-136">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="c3eb8-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c3eb8-137">C#</span><span class="sxs-lookup"><span data-stu-id="c3eb8-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_synchronizationtemplate-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c3eb8-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="c3eb8-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_synchronizationtemplate-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c3eb8-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="c3eb8-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_synchronizationtemplate-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
