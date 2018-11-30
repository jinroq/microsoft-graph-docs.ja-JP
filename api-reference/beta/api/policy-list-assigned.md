---
title: アプリケーションまたはサービス ・ プリンシパルに割り当てられているリストのポリシー
description: アプリケーションまたはサービス ・ プリンシパルに割り当てられているポリシー オブジェクトを取得します。
ms.openlocfilehash: cfdcf3d8e6709080f4c8f7bfc3e2dbc256789f6f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069013"
---
# <a name="list-policies-assigned-to-application-or-service-principal"></a><span data-ttu-id="2978c-103">アプリケーションまたはサービス ・ プリンシパルに割り当てられているリストのポリシー</span><span class="sxs-lookup"><span data-stu-id="2978c-103">List Policies assigned to Application or Service Principal</span></span>

> <span data-ttu-id="2978c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2978c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2978c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2978c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2978c-106">アプリケーションまたはサービス ・ プリンシパルに割り当てられている[ポリシー](../resources/policy.md)オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="2978c-106">Retrieve the [policy](../resources/policy.md) objects assigned to an application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="2978c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2978c-107">Permissions</span></span>
<span data-ttu-id="2978c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2978c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2978c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2978c-110">Permission type</span></span>      | <span data-ttu-id="2978c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2978c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2978c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2978c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2978c-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2978c-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2978c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2978c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2978c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2978c-115">Not supported.</span></span>    |
|<span data-ttu-id="2978c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2978c-116">Application</span></span> | <span data-ttu-id="2978c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2978c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2978c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2978c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/policies
```

> <span data-ttu-id="2978c-119">注意: 要求で"id"は、アプリケーションまたはサービス ・ プリンシパル"appid"プロパティではなく"id"プロパティです。</span><span class="sxs-lookup"><span data-stu-id="2978c-119">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2978c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2978c-120">Request headers</span></span>
| <span data-ttu-id="2978c-121">名前</span><span class="sxs-lookup"><span data-stu-id="2978c-121">Name</span></span>       | <span data-ttu-id="2978c-122">型</span><span class="sxs-lookup"><span data-stu-id="2978c-122">Type</span></span> | <span data-ttu-id="2978c-123">説明</span><span class="sxs-lookup"><span data-stu-id="2978c-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2978c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2978c-124">Authorization</span></span>  | <span data-ttu-id="2978c-125">string</span><span class="sxs-lookup"><span data-stu-id="2978c-125">string</span></span>  | <span data-ttu-id="2978c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2978c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2978c-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="2978c-128">Request body</span></span>
<span data-ttu-id="2978c-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2978c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2978c-130">応答</span><span class="sxs-lookup"><span data-stu-id="2978c-130">Response</span></span>

<span data-ttu-id="2978c-131">かどうかは成功すると、このメソッドを返します`200 OK`応答の本体のコードと[ポリシー](../resources/policy.md)オブジェクトを応答します。</span><span class="sxs-lookup"><span data-stu-id="2978c-131">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="2978c-132">失敗した場合、`4xx`について、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="2978c-132">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="2978c-133">使用例</span><span class="sxs-lookup"><span data-stu-id="2978c-133">Example</span></span>
<span data-ttu-id="2978c-134">次の例では、アプリケーションに割り当てられているポリシーを取得します。</span><span class="sxs-lookup"><span data-stu-id="2978c-134">The following example retrieves the policies assigned to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="2978c-135">要求</span><span class="sxs-lookup"><span data-stu-id="2978c-135">Request</span></span>
<span data-ttu-id="2978c-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2978c-136">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/applications/{id}/policies
```

##### <a name="response"></a><span data-ttu-id="2978c-137">応答</span><span class="sxs-lookup"><span data-stu-id="2978c-137">Response</span></span>
<span data-ttu-id="2978c-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2978c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
