---
title: アプリケーションまたはサービスプリンシパルに割り当てられているポリシーの一覧
description: アプリケーションまたはサービスプリンシパルに割り当てられているポリシーオブジェクトを取得します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 06eb805b6983c72c14c86780f081554611906181
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992053"
---
# <a name="list-policies-assigned-to-application-or-service-principal"></a><span data-ttu-id="e2fd7-103">アプリケーションまたはサービスプリンシパルに割り当てられているポリシーの一覧</span><span class="sxs-lookup"><span data-stu-id="e2fd7-103">List Policies assigned to Application or Service Principal</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2fd7-104">アプリケーションまたはサービスプリンシパルに割り当てられている[ポリシー](../resources/policy.md)オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="e2fd7-104">Retrieve the [policy](../resources/policy.md) objects assigned to an application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2fd7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e2fd7-105">Permissions</span></span>
<span data-ttu-id="e2fd7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2fd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2fd7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e2fd7-108">Permission type</span></span>      | <span data-ttu-id="e2fd7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e2fd7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2fd7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e2fd7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e2fd7-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e2fd7-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e2fd7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e2fd7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2fd7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2fd7-113">Not supported.</span></span>    |
|<span data-ttu-id="e2fd7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e2fd7-114">Application</span></span> | <span data-ttu-id="e2fd7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2fd7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2fd7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e2fd7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/policies
```

> <span data-ttu-id="e2fd7-117">注: 要求の "id" は、"appid" プロパティではなく、アプリケーションまたはサービスプリンシパルの "id" プロパティです。</span><span class="sxs-lookup"><span data-stu-id="e2fd7-117">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2fd7-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e2fd7-118">Request headers</span></span>
| <span data-ttu-id="e2fd7-119">名前</span><span class="sxs-lookup"><span data-stu-id="e2fd7-119">Name</span></span>       | <span data-ttu-id="e2fd7-120">型</span><span class="sxs-lookup"><span data-stu-id="e2fd7-120">Type</span></span> | <span data-ttu-id="e2fd7-121">説明</span><span class="sxs-lookup"><span data-stu-id="e2fd7-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e2fd7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2fd7-122">Authorization</span></span>  | <span data-ttu-id="e2fd7-123">string</span><span class="sxs-lookup"><span data-stu-id="e2fd7-123">string</span></span>  | <span data-ttu-id="e2fd7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e2fd7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2fd7-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e2fd7-126">Request body</span></span>
<span data-ttu-id="e2fd7-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e2fd7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2fd7-128">応答</span><span class="sxs-lookup"><span data-stu-id="e2fd7-128">Response</span></span>

<span data-ttu-id="e2fd7-129">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[ポリシー](../resources/policy.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e2fd7-129">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="e2fd7-130">失敗した場合、`4xx` エラーが詳細情報とともに返されます。</span><span class="sxs-lookup"><span data-stu-id="e2fd7-130">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="e2fd7-131">例</span><span class="sxs-lookup"><span data-stu-id="e2fd7-131">Example</span></span>
<span data-ttu-id="e2fd7-132">次の例では、アプリケーションに割り当てられているポリシーを取得します。</span><span class="sxs-lookup"><span data-stu-id="e2fd7-132">The following example retrieves the policies assigned to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="e2fd7-133">要求</span><span class="sxs-lookup"><span data-stu-id="e2fd7-133">Request</span></span>
<span data-ttu-id="e2fd7-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e2fd7-134">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/applications/{id}/policies
```

##### <a name="response"></a><span data-ttu-id="e2fd7-135">応答</span><span class="sxs-lookup"><span data-stu-id="e2fd7-135">Response</span></span>
<span data-ttu-id="e2fd7-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e2fd7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Cache-Control: private
Content-Type: application/json

{
    "value":[
        {
            "@odata.type":"#microsoft.graph.policy",
            "id":"id-value",
            "alternativeIdentifier":null,
            "definition":["policy-definition"],
            "displayName":"name-value",
            "isOrganizationDefault":boolean-value,
            "keyCredentials":[key-credentials],
            "type":"type-value"
        }
    ]
}
```
