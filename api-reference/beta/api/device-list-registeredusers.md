---
title: registeredUsers を一覧表示する
description: デバイスの登録ユーザーの一覧を取得します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9c25b9db7577c2fb57d034bac7aa5f9c7e1fd18a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321468"
---
# <a name="list-registeredusers"></a><span data-ttu-id="ade1b-103">registeredUsers を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ade1b-103">List registeredUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ade1b-104">デバイスの登録ユーザーの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="ade1b-104">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="ade1b-105">クラウドに参加済みのデバイスと登録済みの個人用デバイスの場合、登録済みのユーザーは、登録時に登録済み所有者と同じ値に設定されます。</span><span class="sxs-lookup"><span data-stu-id="ade1b-105">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="ade1b-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ade1b-106">Permissions</span></span>
<span data-ttu-id="ade1b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ade1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ade1b-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ade1b-109">Permission type</span></span>      | <span data-ttu-id="ade1b-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ade1b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ade1b-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ade1b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ade1b-112">Directory.accessasuser.all またはすべて、またはすべてのディレクトリを読み取ることができます。</span><span class="sxs-lookup"><span data-stu-id="ade1b-112">Directory.Read.All or Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ade1b-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ade1b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ade1b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ade1b-114">Not supported.</span></span> |
|<span data-ttu-id="ade1b-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ade1b-115">Application</span></span> | <span data-ttu-id="ade1b-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ade1b-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ade1b-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ade1b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```

> <span data-ttu-id="ade1b-118">注:要求内の"id"は、"deviceId"プロパティではなく、デバイスの id プロパティです。</span><span class="sxs-lookup"><span data-stu-id="ade1b-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="ade1b-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ade1b-119">Optional query parameters</span></span>
<span data-ttu-id="ade1b-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ade1b-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ade1b-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ade1b-121">Request headers</span></span>
| <span data-ttu-id="ade1b-122">名前</span><span class="sxs-lookup"><span data-stu-id="ade1b-122">Name</span></span>       | <span data-ttu-id="ade1b-123">型</span><span class="sxs-lookup"><span data-stu-id="ade1b-123">Type</span></span> | <span data-ttu-id="ade1b-124">説明</span><span class="sxs-lookup"><span data-stu-id="ade1b-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ade1b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ade1b-125">Authorization</span></span>  | <span data-ttu-id="ade1b-126">string</span><span class="sxs-lookup"><span data-stu-id="ade1b-126">string</span></span>  | <span data-ttu-id="ade1b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ade1b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ade1b-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="ade1b-129">Request body</span></span>
<span data-ttu-id="ade1b-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ade1b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ade1b-131">応答</span><span class="sxs-lookup"><span data-stu-id="ade1b-131">Response</span></span>

<span data-ttu-id="ade1b-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ade1b-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ade1b-133">例</span><span class="sxs-lookup"><span data-stu-id="ade1b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ade1b-134">要求</span><span class="sxs-lookup"><span data-stu-id="ade1b-134">Request</span></span>
<span data-ttu-id="ade1b-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ade1b-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ade1b-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ade1b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/registeredUsers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ade1b-137">C#</span><span class="sxs-lookup"><span data-stu-id="ade1b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ade1b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ade1b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ade1b-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="ade1b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ade1b-140">Java</span><span class="sxs-lookup"><span data-stu-id="ade1b-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registeredusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ade1b-141">応答</span><span class="sxs-lookup"><span data-stu-id="ade1b-141">Response</span></span>
<span data-ttu-id="ade1b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ade1b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
