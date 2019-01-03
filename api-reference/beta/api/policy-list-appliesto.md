---
title: アプリケーションとサービス ・ プリンシパルに割り当てられている特定のポリシーを一覧表示します。
description: 割り当てられている指定されたポリシーを使用して、アプリケーションとサービスのプリンシパル オブジェクトを取得します。
ms.openlocfilehash: 3f281d7c60a506676a78637ad71f1ce26de35e34
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072913"
---
# <a name="list-applications-and-service-principals-with-specific-policy-assigned"></a><span data-ttu-id="966b1-103">アプリケーションとサービス ・ プリンシパルに割り当てられている特定のポリシーを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="966b1-103">List Applications and Service Principals with specific Policy assigned</span></span>

> <span data-ttu-id="966b1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="966b1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="966b1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="966b1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="966b1-106">割り当てられている指定されたポリシーを使用して、[アプリケーション](../resources/application.md)と[サービス ・ プリンシパル](../resources/serviceprincipal.md)オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="966b1-106">Retrieve the [application](../resources/application.md) and [service principal](../resources/serviceprincipal.md) objects with the specified policy assigned.</span></span>

## <a name="permissions"></a><span data-ttu-id="966b1-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="966b1-107">Permissions</span></span>
<span data-ttu-id="966b1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="966b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="966b1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="966b1-110">Permission type</span></span>      | <span data-ttu-id="966b1-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="966b1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="966b1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="966b1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="966b1-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="966b1-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="966b1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="966b1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="966b1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="966b1-115">Not supported.</span></span>    |
|<span data-ttu-id="966b1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="966b1-116">Application</span></span> | <span data-ttu-id="966b1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="966b1-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="966b1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="966b1-118">HTTP request</span></span>
```http
GET /policies/{id}/appliesTo
```

## <a name="request-headers"></a><span data-ttu-id="966b1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="966b1-119">Request headers</span></span>
| <span data-ttu-id="966b1-120">名前</span><span class="sxs-lookup"><span data-stu-id="966b1-120">Name</span></span>       | <span data-ttu-id="966b1-121">型</span><span class="sxs-lookup"><span data-stu-id="966b1-121">Type</span></span> | <span data-ttu-id="966b1-122">説明</span><span class="sxs-lookup"><span data-stu-id="966b1-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="966b1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="966b1-123">Authorization</span></span>  | <span data-ttu-id="966b1-124">string</span><span class="sxs-lookup"><span data-stu-id="966b1-124">string</span></span>  | <span data-ttu-id="966b1-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="966b1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="966b1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="966b1-127">Request body</span></span>
<span data-ttu-id="966b1-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="966b1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="966b1-129">応答</span><span class="sxs-lookup"><span data-stu-id="966b1-129">Response</span></span>

<span data-ttu-id="966b1-130">かどうかは成功すると、このメソッドを返します`200 OK`応答本体に応答コードおよび[アプリケーション](../resources/application.md)と[サービス ・ プリンシパル](../resources/serviceprincipal.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="966b1-130">If successful, this method returns `200 OK` response code and [application](../resources/application.md) and [service principal](../resources/serviceprincipal.md) objects in the response body.</span></span> <span data-ttu-id="966b1-131">失敗した場合、`4xx`について、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="966b1-131">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="966b1-132">使用例</span><span class="sxs-lookup"><span data-stu-id="966b1-132">Example</span></span>
<span data-ttu-id="966b1-133">次の使用例は、割り当てられている特定のポリシーを使用して、アプリケーションとサービス ・ プリンシパルを取得します。</span><span class="sxs-lookup"><span data-stu-id="966b1-133">The following example retrieves the applications and service principals with a specific policy assigned.</span></span>

##### <a name="request"></a><span data-ttu-id="966b1-134">要求</span><span class="sxs-lookup"><span data-stu-id="966b1-134">Request</span></span>
<span data-ttu-id="966b1-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="966b1-135">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}/appliesTo
```

##### <a name="response"></a><span data-ttu-id="966b1-136">応答</span><span class="sxs-lookup"><span data-stu-id="966b1-136">Response</span></span>
<span data-ttu-id="966b1-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="966b1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value":[
        {
            "@odata.type"="#microsoft.graph.application",
            "appId":"appId-value",
            "displayName":"displayName-value",
            "errorUrl":"errorUrl-value",
            "groupMembershipClaims":"groupMembershipClaims-value",
            "homepage":"homepage-value",
            "id":"id-value",
            "keyCredentials":[key-credentials],
            "logoutUrl":"logoutUrl-value",
            "replyUrls":["replyUrls-value"]
        }
    ]
}
```