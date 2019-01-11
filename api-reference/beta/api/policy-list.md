---
title: リスト ポリシー
description: ディレクトリ内のすべてのポリシー オブジェクトを取得します。
localization_priority: Normal
ms.openlocfilehash: ea97146b646068515ab6fdc7fab4b3cefb16031e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836058"
---
# <a name="list-policies"></a><span data-ttu-id="79b80-103">リスト ポリシー</span><span class="sxs-lookup"><span data-stu-id="79b80-103">List Policies</span></span>

> <span data-ttu-id="79b80-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="79b80-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79b80-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79b80-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="79b80-106">ディレクトリ内のすべての[ポリシー](../resources/policy.md)オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="79b80-106">Retrieve all [policy](../resources/policy.md) objects in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="79b80-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="79b80-107">Permissions</span></span>
<span data-ttu-id="79b80-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79b80-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79b80-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="79b80-110">Permission type</span></span>      | <span data-ttu-id="79b80-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="79b80-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79b80-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="79b80-112">Delegated (work or school account)</span></span> | <span data-ttu-id="79b80-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="79b80-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="79b80-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="79b80-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79b80-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79b80-115">Not supported.</span></span>    |
|<span data-ttu-id="79b80-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="79b80-116">Application</span></span> | <span data-ttu-id="79b80-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79b80-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="79b80-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="79b80-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies
```
## <a name="request-headers"></a><span data-ttu-id="79b80-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79b80-119">Request headers</span></span>
| <span data-ttu-id="79b80-120">名前</span><span class="sxs-lookup"><span data-stu-id="79b80-120">Name</span></span>       | <span data-ttu-id="79b80-121">種類</span><span class="sxs-lookup"><span data-stu-id="79b80-121">Type</span></span> | <span data-ttu-id="79b80-122">説明</span><span class="sxs-lookup"><span data-stu-id="79b80-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="79b80-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="79b80-123">Authorization</span></span>  | <span data-ttu-id="79b80-124">string</span><span class="sxs-lookup"><span data-stu-id="79b80-124">string</span></span>  | <span data-ttu-id="79b80-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="79b80-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="79b80-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="79b80-127">Request body</span></span>
<span data-ttu-id="79b80-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="79b80-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79b80-129">応答</span><span class="sxs-lookup"><span data-stu-id="79b80-129">Response</span></span>

<span data-ttu-id="79b80-130">かどうかは成功すると、このメソッドを返します`200 OK`応答の本体のコードと[ポリシー](../resources/policy.md)オブジェクトを応答します。</span><span class="sxs-lookup"><span data-stu-id="79b80-130">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="79b80-131">それ以外の場合.</span><span class="sxs-lookup"><span data-stu-id="79b80-131">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="79b80-132">例</span><span class="sxs-lookup"><span data-stu-id="79b80-132">Example</span></span>
<span data-ttu-id="79b80-133">次の例では、すべてのポリシーを取得します。</span><span class="sxs-lookup"><span data-stu-id="79b80-133">The following example retrieves all policies.</span></span>

##### <a name="request"></a><span data-ttu-id="79b80-134">要求</span><span class="sxs-lookup"><span data-stu-id="79b80-134">Request</span></span>
<span data-ttu-id="79b80-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="79b80-135">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies
```

##### <a name="response"></a><span data-ttu-id="79b80-136">応答</span><span class="sxs-lookup"><span data-stu-id="79b80-136">Response</span></span>
<span data-ttu-id="79b80-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="79b80-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "value":[
        {
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
