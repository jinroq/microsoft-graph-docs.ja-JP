---
title: ポリシーを取得します。
description: ポリシーのプロパティを取得します。
localization_priority: Normal
ms.openlocfilehash: 9b3e23639bdeea673ccbe56bbce0c74443a99480
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870596"
---
# <a name="get-policy"></a><span data-ttu-id="0582c-103">ポリシーを取得します。</span><span class="sxs-lookup"><span data-stu-id="0582c-103">Get Policy</span></span>

> <span data-ttu-id="0582c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0582c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0582c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0582c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0582c-106">[ポリシー](../resources/policy.md)のプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="0582c-106">Retrieve the properties of a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0582c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0582c-107">Permissions</span></span>
<span data-ttu-id="0582c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0582c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0582c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0582c-110">Permission type</span></span>      | <span data-ttu-id="0582c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0582c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0582c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0582c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0582c-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0582c-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0582c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0582c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0582c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0582c-115">Not supported.</span></span>    |
|<span data-ttu-id="0582c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0582c-116">Application</span></span> | <span data-ttu-id="0582c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0582c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0582c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0582c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0582c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0582c-119">Request headers</span></span>
| <span data-ttu-id="0582c-120">名前</span><span class="sxs-lookup"><span data-stu-id="0582c-120">Name</span></span>       | <span data-ttu-id="0582c-121">種類</span><span class="sxs-lookup"><span data-stu-id="0582c-121">Type</span></span> | <span data-ttu-id="0582c-122">説明</span><span class="sxs-lookup"><span data-stu-id="0582c-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0582c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0582c-123">Authorization</span></span>  | <span data-ttu-id="0582c-124">string</span><span class="sxs-lookup"><span data-stu-id="0582c-124">string</span></span>  | <span data-ttu-id="0582c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0582c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0582c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0582c-127">Request body</span></span>
<span data-ttu-id="0582c-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0582c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0582c-129">応答</span><span class="sxs-lookup"><span data-stu-id="0582c-129">Response</span></span>

<span data-ttu-id="0582c-130">かどうかは成功すると、このメソッドを返します`200 OK`応答コードおよび応答の本文の[ポリシー](../resources/policy.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="0582c-130">If successful, this method returns `200 OK` response code and a [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="0582c-131">場合 unsucccessful.</span><span class="sxs-lookup"><span data-stu-id="0582c-131">If unsucccessful...</span></span>

## <a name="example"></a><span data-ttu-id="0582c-132">例</span><span class="sxs-lookup"><span data-stu-id="0582c-132">Example</span></span>
<span data-ttu-id="0582c-133">次の例では、特定のポリシーを取得します。</span><span class="sxs-lookup"><span data-stu-id="0582c-133">The following example retrieves a specific policy.</span></span>

##### <a name="request"></a><span data-ttu-id="0582c-134">要求</span><span class="sxs-lookup"><span data-stu-id="0582c-134">Request</span></span>
<span data-ttu-id="0582c-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0582c-135">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="0582c-136">応答</span><span class="sxs-lookup"><span data-stu-id="0582c-136">Response</span></span>
<span data-ttu-id="0582c-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0582c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#policies/$entity",
    "id":"id-value",
    "alternativeIdentifier":null,
    "definition":["policy-definition"],
    "displayName":"name-value",
    "isOrganizationDefault":boolean-value,
    "keyCredentials":[key-credentials],
    "type":"type-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
