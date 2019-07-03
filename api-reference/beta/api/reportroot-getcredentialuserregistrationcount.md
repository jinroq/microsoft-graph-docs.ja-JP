---
title: 'reportRoot: getCredentialUserRegistrationCount'
description: 組織内のユーザーのうち、セルフサービスのパスワードのリセットおよび多要素認証 (MFA) の機能を使用するために登録されているユーザー数の現在の状態を報告します。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: b5e14b293447e585451f343a1c130e7d3d323a59
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504569"
---
# <a name="reportroot-getcredentialuserregistrationcount"></a><span data-ttu-id="257e3-103">reportRoot: getCredentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="257e3-103">reportRoot: getCredentialUserRegistrationCount</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="257e3-104">組織内のユーザーのうち、セルフサービスのパスワードのリセットおよび多要素認証 (MFA) の機能を使用するために登録されているユーザー数の現在の状態を報告します。</span><span class="sxs-lookup"><span data-stu-id="257e3-104">Report the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication (MFA) capabilities.</span></span>

## <a name="permissions"></a><span data-ttu-id="257e3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="257e3-105">Permissions</span></span>

<span data-ttu-id="257e3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="257e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="257e3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="257e3-108">Permission type</span></span>                        | <span data-ttu-id="257e3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="257e3-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="257e3-110">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="257e3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="257e3-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="257e3-111">Reports.Read.All</span></span> |
| <span data-ttu-id="257e3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="257e3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="257e3-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="257e3-113">Not supported.</span></span> |
| <span data-ttu-id="257e3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="257e3-114">Application</span></span>                            | <span data-ttu-id="257e3-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="257e3-115">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="257e3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="257e3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getCredentialsUserRegistrationCount
```

## <a name="request-headers"></a><span data-ttu-id="257e3-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="257e3-117">Request headers</span></span>

| <span data-ttu-id="257e3-118">名前</span><span class="sxs-lookup"><span data-stu-id="257e3-118">Name</span></span>          | <span data-ttu-id="257e3-119">説明</span><span class="sxs-lookup"><span data-stu-id="257e3-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="257e3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="257e3-120">Authorization</span></span> | <span data-ttu-id="257e3-121">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="257e3-121">Bearer {token}</span></span> |
| <span data-ttu-id="257e3-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="257e3-122">Content-Type</span></span> | <span data-ttu-id="257e3-123">application/json</span><span class="sxs-lookup"><span data-stu-id="257e3-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="257e3-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="257e3-124">Request body</span></span>

<span data-ttu-id="257e3-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="257e3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="257e3-126">応答</span><span class="sxs-lookup"><span data-stu-id="257e3-126">Response</span></span>

<span data-ttu-id="257e3-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で新しい[Credentialuserregistrationcount](../resources/credentialuserregistrationcount.md)コレクションオブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="257e3-127">If successful, this method returns a `200 OK` response code and a new [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="257e3-128">例</span><span class="sxs-lookup"><span data-stu-id="257e3-128">Examples</span></span>

<span data-ttu-id="257e3-129">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="257e3-129">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="257e3-130">要求</span><span class="sxs-lookup"><span data-stu-id="257e3-130">Request</span></span>

<span data-ttu-id="257e3-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="257e3-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "reportroot_getcredentialuserregistrationcount"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getCredentialUserRegistrationCount
```

### <a name="response"></a><span data-ttu-id="257e3-132">応答</span><span class="sxs-lookup"><span data-stu-id="257e3-132">Response</span></span>

<span data-ttu-id="257e3-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="257e3-133">The following is an example of the response.</span></span>

> <span data-ttu-id="257e3-134">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="257e3-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="257e3-135">すべてのプロパティは、実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="257e3-135">All the properties are returned from an actual call.</span></span>

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
