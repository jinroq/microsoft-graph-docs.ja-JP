---
title: リスト ポリシー
description: ディレクトリ内のすべてのポリシー オブジェクトを取得します。
ms.openlocfilehash: 5abff0973a53dc3bddfd256dbc43faad519e20e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073608"
---
# <a name="list-policies"></a><span data-ttu-id="12da4-103">リスト ポリシー</span><span class="sxs-lookup"><span data-stu-id="12da4-103">List Policies</span></span>

> <span data-ttu-id="12da4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="12da4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12da4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12da4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="12da4-106">ディレクトリ内のすべての[ポリシー](../resources/policy.md)オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="12da4-106">Retrieve all [policy](../resources/policy.md) objects in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="12da4-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="12da4-107">Permissions</span></span>
<span data-ttu-id="12da4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="12da4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12da4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="12da4-110">Permission type</span></span>      | <span data-ttu-id="12da4-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="12da4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12da4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="12da4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="12da4-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="12da4-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="12da4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="12da4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12da4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12da4-115">Not supported.</span></span>    |
|<span data-ttu-id="12da4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="12da4-116">Application</span></span> | <span data-ttu-id="12da4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12da4-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="12da4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="12da4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies
```
## <a name="request-headers"></a><span data-ttu-id="12da4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="12da4-119">Request headers</span></span>
| <span data-ttu-id="12da4-120">名前</span><span class="sxs-lookup"><span data-stu-id="12da4-120">Name</span></span>       | <span data-ttu-id="12da4-121">型</span><span class="sxs-lookup"><span data-stu-id="12da4-121">Type</span></span> | <span data-ttu-id="12da4-122">説明</span><span class="sxs-lookup"><span data-stu-id="12da4-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="12da4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="12da4-123">Authorization</span></span>  | <span data-ttu-id="12da4-124">string</span><span class="sxs-lookup"><span data-stu-id="12da4-124">string</span></span>  | <span data-ttu-id="12da4-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="12da4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12da4-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="12da4-127">Request body</span></span>
<span data-ttu-id="12da4-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="12da4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12da4-129">応答</span><span class="sxs-lookup"><span data-stu-id="12da4-129">Response</span></span>

<span data-ttu-id="12da4-130">かどうかは成功すると、このメソッドを返します`200 OK`応答の本体のコードと[ポリシー](../resources/policy.md)オブジェクトを応答します。</span><span class="sxs-lookup"><span data-stu-id="12da4-130">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="12da4-131">それ以外の場合.</span><span class="sxs-lookup"><span data-stu-id="12da4-131">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="12da4-132">使用例</span><span class="sxs-lookup"><span data-stu-id="12da4-132">Example</span></span>
<span data-ttu-id="12da4-133">次の例では、すべてのポリシーを取得します。</span><span class="sxs-lookup"><span data-stu-id="12da4-133">The following example retrieves all policies.</span></span>

##### <a name="request"></a><span data-ttu-id="12da4-134">要求</span><span class="sxs-lookup"><span data-stu-id="12da4-134">Request</span></span>
<span data-ttu-id="12da4-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="12da4-135">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies
```

##### <a name="response"></a><span data-ttu-id="12da4-136">応答</span><span class="sxs-lookup"><span data-stu-id="12da4-136">Response</span></span>
<span data-ttu-id="12da4-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="12da4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
