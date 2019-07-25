---
title: registeredOwners を一覧表示する
description: デバイスの登録済み所有者の一覧を取得します。 登録済み所有者は、デバイスがクラウドに参加済みか、または個人用デバイスが登録済みのユーザーです。 登録済み所有者は、登録時に設定されます。 現在、所有者は 1 人しかいることができません。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 479901336f2f38b57aff268e90e0fcd3b7a96f5f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862728"
---
# <a name="list-registeredowners"></a><span data-ttu-id="d2656-106">registeredOwners を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d2656-106">List registeredOwners</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2656-107">デバイスの登録済み所有者の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="d2656-107">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="d2656-108">登録済み所有者は、デバイスがクラウドに参加済みか、または個人用デバイスが登録済みのユーザーです。</span><span class="sxs-lookup"><span data-stu-id="d2656-108">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="d2656-109">登録済み所有者は、登録時に設定されます。</span><span class="sxs-lookup"><span data-stu-id="d2656-109">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="d2656-110">現在、所有者は 1 人しかいることができません。</span><span class="sxs-lookup"><span data-stu-id="d2656-110">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2656-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d2656-111">Permissions</span></span>

<span data-ttu-id="d2656-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2656-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2656-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d2656-114">Permission type</span></span>      | <span data-ttu-id="d2656-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d2656-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2656-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d2656-116">Delegated (work or school account)</span></span> | <span data-ttu-id="d2656-117">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d2656-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d2656-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d2656-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2656-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2656-119">Not supported.</span></span>    |
|<span data-ttu-id="d2656-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d2656-120">Application</span></span> | <span data-ttu-id="d2656-121">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2656-121">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2656-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d2656-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```

> <span data-ttu-id="d2656-123">注:要求内の"id"は、"deviceId"プロパティではなく、デバイスの id プロパティです。</span><span class="sxs-lookup"><span data-stu-id="d2656-123">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="d2656-124">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d2656-124">Optional query parameters</span></span>
<span data-ttu-id="d2656-125">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d2656-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d2656-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2656-126">Request headers</span></span>
| <span data-ttu-id="d2656-127">名前</span><span class="sxs-lookup"><span data-stu-id="d2656-127">Name</span></span>       | <span data-ttu-id="d2656-128">型</span><span class="sxs-lookup"><span data-stu-id="d2656-128">Type</span></span> | <span data-ttu-id="d2656-129">説明</span><span class="sxs-lookup"><span data-stu-id="d2656-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d2656-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2656-130">Authorization</span></span>  | <span data-ttu-id="d2656-131">string</span><span class="sxs-lookup"><span data-stu-id="d2656-131">string</span></span>  | <span data-ttu-id="d2656-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d2656-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2656-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="d2656-134">Request body</span></span>
<span data-ttu-id="d2656-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d2656-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2656-136">応答</span><span class="sxs-lookup"><span data-stu-id="d2656-136">Response</span></span>

<span data-ttu-id="d2656-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d2656-137">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d2656-138">例</span><span class="sxs-lookup"><span data-stu-id="d2656-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2656-139">要求</span><span class="sxs-lookup"><span data-stu-id="d2656-139">Request</span></span>
<span data-ttu-id="d2656-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d2656-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d2656-141">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d2656-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/registeredOwners
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d2656-142">C#</span><span class="sxs-lookup"><span data-stu-id="d2656-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredowners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d2656-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="d2656-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredowners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d2656-144">目的-C</span><span class="sxs-lookup"><span data-stu-id="d2656-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredowners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d2656-145">Java</span><span class="sxs-lookup"><span data-stu-id="d2656-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registeredowners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d2656-146">応答</span><span class="sxs-lookup"><span data-stu-id="d2656-146">Response</span></span>
<span data-ttu-id="d2656-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d2656-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
