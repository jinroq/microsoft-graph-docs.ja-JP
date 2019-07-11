---
title: 既存の同期テンプレートを一覧表示する
description: 特定のアプリケーションまたはサービスプリンシパルに関連付けられている同期テンプレートを一覧表示します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4542352e4edf704ff8c3c8575d8a999b113582d0
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620424"
---
# <a name="list-existing-synchronization-templates"></a><span data-ttu-id="14a19-103">既存の同期テンプレートを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="14a19-103">List existing synchronization templates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14a19-104">特定のアプリケーションまたはサービスプリンシパルに関連付けられている同期テンプレートを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="14a19-104">List the synchronization templates associated with a given application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="14a19-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="14a19-105">Permissions</span></span>
<span data-ttu-id="14a19-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="14a19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14a19-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="14a19-108">Permission type</span></span>                        | <span data-ttu-id="14a19-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="14a19-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="14a19-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="14a19-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="14a19-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14a19-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="14a19-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="14a19-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="14a19-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14a19-113">Not supported.</span></span>|
|<span data-ttu-id="14a19-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="14a19-114">Application</span></span>                            |<span data-ttu-id="14a19-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14a19-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="14a19-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="14a19-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET servicePrincipals/{id}/synchronization/templates
GET applications/{id}/synchronization/templates
```

## <a name="request-headers"></a><span data-ttu-id="14a19-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="14a19-117">Request headers</span></span>

| <span data-ttu-id="14a19-118">名前</span><span class="sxs-lookup"><span data-stu-id="14a19-118">Name</span></span>           | <span data-ttu-id="14a19-119">型</span><span class="sxs-lookup"><span data-stu-id="14a19-119">Type</span></span>    | <span data-ttu-id="14a19-120">説明</span><span class="sxs-lookup"><span data-stu-id="14a19-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="14a19-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="14a19-121">Authorization</span></span>  | <span data-ttu-id="14a19-122">string</span><span class="sxs-lookup"><span data-stu-id="14a19-122">string</span></span>  | <span data-ttu-id="14a19-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="14a19-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14a19-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="14a19-125">Request body</span></span>

<span data-ttu-id="14a19-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="14a19-126">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="14a19-127">応答</span><span class="sxs-lookup"><span data-stu-id="14a19-127">Response</span></span>

<span data-ttu-id="14a19-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[同期テンプレート](../resources/synchronization-synchronizationtemplate.md)オブジェクトの acollection を返します。</span><span class="sxs-lookup"><span data-stu-id="14a19-128">If successful, this method returns a `200 OK` response code and acollection of [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) objects in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="14a19-129">例</span><span class="sxs-lookup"><span data-stu-id="14a19-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="14a19-130">要求</span><span class="sxs-lookup"><span data-stu-id="14a19-130">Request</span></span>
<span data-ttu-id="14a19-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="14a19-131">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="14a19-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="14a19-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationtemplate"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="14a19-133">C#</span><span class="sxs-lookup"><span data-stu-id="14a19-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="14a19-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="14a19-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="14a19-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="14a19-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="14a19-136">応答</span><span class="sxs-lookup"><span data-stu-id="14a19-136">Response</span></span>
<span data-ttu-id="14a19-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="14a19-137">The following is an example of a response.</span></span>
><span data-ttu-id="14a19-138">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="14a19-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="14a19-139">実際の呼び出しでは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="14a19-139">All the properties will be returned in an actual call.</span></span>
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
  ]
}
-->
