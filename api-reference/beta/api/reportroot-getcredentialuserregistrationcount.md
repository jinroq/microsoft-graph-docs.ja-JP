---
title: 'reportRoot: getCredentialUserRegistrationCount'
description: 組織内のユーザーのうち、セルフサービスのパスワードのリセットおよび多要素認証 (MFA) の機能を使用するために登録されているユーザー数の現在の状態を報告します。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 1ec286eb86b3dbeeb5f7687b2af00a36b76348b4
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36411922"
---
# <a name="reportroot-getcredentialuserregistrationcount"></a><span data-ttu-id="0b398-103">reportRoot: getCredentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="0b398-103">reportRoot: getCredentialUserRegistrationCount</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b398-104">組織内のユーザーのうち、セルフサービスのパスワードのリセットおよび多要素認証 (MFA) の機能を使用するために登録されているユーザー数の現在の状態を報告します。</span><span class="sxs-lookup"><span data-stu-id="0b398-104">Report the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication (MFA) capabilities.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b398-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0b398-105">Permissions</span></span>

<span data-ttu-id="0b398-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0b398-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0b398-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0b398-108">Permission type</span></span>                        | <span data-ttu-id="0b398-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0b398-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0b398-110">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="0b398-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0b398-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b398-111">Reports.Read.All</span></span> |
| <span data-ttu-id="0b398-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0b398-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b398-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b398-113">Not supported.</span></span> |
| <span data-ttu-id="0b398-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0b398-114">Application</span></span>                            | <span data-ttu-id="0b398-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b398-115">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b398-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0b398-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getCredentialUserRegistrationCount
```

## <a name="request-headers"></a><span data-ttu-id="0b398-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0b398-117">Request headers</span></span>

| <span data-ttu-id="0b398-118">名前</span><span class="sxs-lookup"><span data-stu-id="0b398-118">Name</span></span>          | <span data-ttu-id="0b398-119">説明</span><span class="sxs-lookup"><span data-stu-id="0b398-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0b398-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b398-120">Authorization</span></span> | <span data-ttu-id="0b398-121">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="0b398-121">Bearer {token}</span></span> |
| <span data-ttu-id="0b398-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0b398-122">Content-Type</span></span> | <span data-ttu-id="0b398-123">application/json</span><span class="sxs-lookup"><span data-stu-id="0b398-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b398-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="0b398-124">Request body</span></span>

<span data-ttu-id="0b398-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0b398-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b398-126">応答</span><span class="sxs-lookup"><span data-stu-id="0b398-126">Response</span></span>

<span data-ttu-id="0b398-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で新しい[Credentialuserregistrationcount](../resources/credentialuserregistrationcount.md)コレクションオブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0b398-127">If successful, this method returns a `200 OK` response code and a new [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0b398-128">例</span><span class="sxs-lookup"><span data-stu-id="0b398-128">Examples</span></span>

<span data-ttu-id="0b398-129">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="0b398-129">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="0b398-130">要求</span><span class="sxs-lookup"><span data-stu-id="0b398-130">Request</span></span>

<span data-ttu-id="0b398-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0b398-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0b398-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0b398-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getcredentialuserregistrationcount"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getCredentialUserRegistrationCount
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0b398-133">C#</span><span class="sxs-lookup"><span data-stu-id="0b398-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getcredentialuserregistrationcount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b398-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b398-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getcredentialuserregistrationcount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0b398-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="0b398-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getcredentialuserregistrationcount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0b398-136">応答</span><span class="sxs-lookup"><span data-stu-id="0b398-136">Response</span></span>

<span data-ttu-id="0b398-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0b398-137">The following is an example of the response.</span></span>

> <span data-ttu-id="0b398-138">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="0b398-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0b398-139">すべてのプロパティは、実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0b398-139">All the properties are returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.credentialUserRegistrationCount",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.credentialUserRegistrationCount)",
  "value": [
    {
      "id" : "id-value",
      "totalUserCount" : 23123,
      "userRegistrationCounts" :
      [
        { "userRegistrationStatus":"registered", 
          "userRegistationCount": 23423 }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reportRoot: getCredentialUserRegistrationCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
