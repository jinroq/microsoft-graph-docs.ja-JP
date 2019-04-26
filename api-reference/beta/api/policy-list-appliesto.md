---
title: 特定のポリシーが割り当てられたアプリケーションとサービスプリンシパルを一覧表示する
description: 指定したポリシーが割り当てられているアプリケーションおよびサービスプリンシパルオブジェクトを取得します。
localization_priority: Normal
ms.openlocfilehash: c58822e5e3c90f5774721e425af62b40422d3db2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337400"
---
# <a name="list-applications-and-service-principals-with-specific-policy-assigned"></a><span data-ttu-id="46720-103">特定のポリシーが割り当てられたアプリケーションとサービスプリンシパルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="46720-103">List applications and service principals with specific policy assigned</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46720-104">指定したポリシーが割り当てられている[アプリケーション](../resources/application.md)および[サービスプリンシパル](../resources/serviceprincipal.md)オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="46720-104">Retrieve the [application](../resources/application.md) and [service principal](../resources/serviceprincipal.md) objects with the specified policy assigned.</span></span>

## <a name="permissions"></a><span data-ttu-id="46720-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="46720-105">Permissions</span></span>
<span data-ttu-id="46720-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="46720-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46720-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="46720-108">Permission type</span></span>      | <span data-ttu-id="46720-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="46720-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46720-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="46720-110">Delegated (work or school account)</span></span> | <span data-ttu-id="46720-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="46720-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="46720-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="46720-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46720-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46720-113">Not supported.</span></span>    |
|<span data-ttu-id="46720-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="46720-114">Application</span></span> | <span data-ttu-id="46720-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46720-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="46720-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="46720-116">HTTP request</span></span>
```http
GET /policies/{id}/appliesTo
```

## <a name="request-headers"></a><span data-ttu-id="46720-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="46720-117">Request headers</span></span>
| <span data-ttu-id="46720-118">名前</span><span class="sxs-lookup"><span data-stu-id="46720-118">Name</span></span>       | <span data-ttu-id="46720-119">型</span><span class="sxs-lookup"><span data-stu-id="46720-119">Type</span></span> | <span data-ttu-id="46720-120">説明</span><span class="sxs-lookup"><span data-stu-id="46720-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="46720-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="46720-121">Authorization</span></span>  | <span data-ttu-id="46720-122">string</span><span class="sxs-lookup"><span data-stu-id="46720-122">string</span></span>  | <span data-ttu-id="46720-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="46720-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="46720-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="46720-125">Request body</span></span>
<span data-ttu-id="46720-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="46720-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46720-127">応答</span><span class="sxs-lookup"><span data-stu-id="46720-127">Response</span></span>

<span data-ttu-id="46720-128">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[application](../resources/application.md)と[serviceprincipal](../resources/serviceprincipal.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="46720-128">If successful, this method returns `200 OK` response code and [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span> <span data-ttu-id="46720-129">失敗した場合、`4xx` エラーが詳細情報とともに返されます。</span><span class="sxs-lookup"><span data-stu-id="46720-129">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="46720-130">例</span><span class="sxs-lookup"><span data-stu-id="46720-130">Example</span></span>
<span data-ttu-id="46720-131">次の例では、特定のポリシーが割り当てられたアプリケーションとサービスプリンシパルを取得します。</span><span class="sxs-lookup"><span data-stu-id="46720-131">The following example retrieves the applications and service principals with a specific policy assigned.</span></span>

##### <a name="request"></a><span data-ttu-id="46720-132">要求</span><span class="sxs-lookup"><span data-stu-id="46720-132">Request</span></span>
<span data-ttu-id="46720-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="46720-133">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}/appliesTo
```

##### <a name="response"></a><span data-ttu-id="46720-134">応答</span><span class="sxs-lookup"><span data-stu-id="46720-134">Response</span></span>
<span data-ttu-id="46720-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="46720-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
