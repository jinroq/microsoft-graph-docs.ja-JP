---
title: privilegedRoleSummary を取得する
description: PrivilegedRoleSummary オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 1604159671ff18ab3456c15b611ec426d9982282
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978664"
---
# <a name="get-privilegedrolesummary"></a><span data-ttu-id="941b6-103">privilegedRoleSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="941b6-103">Get privilegedRoleSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="941b6-104">[PrivilegedRoleSummary](../resources/privilegedrolesummary.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="941b6-104">Retrieve the properties and relationships of [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="941b6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="941b6-105">Permissions</span></span>
<span data-ttu-id="941b6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="941b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="941b6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="941b6-108">Permission type</span></span>      | <span data-ttu-id="941b6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="941b6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="941b6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="941b6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="941b6-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="941b6-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="941b6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="941b6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="941b6-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="941b6-113">Not supported.</span></span>    |
|<span data-ttu-id="941b6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="941b6-114">Application</span></span> | <span data-ttu-id="941b6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="941b6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="941b6-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="941b6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}?$expand=summary
```
## <a name="optional-query-parameters"></a><span data-ttu-id="941b6-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="941b6-117">Optional query parameters</span></span>
<span data-ttu-id="941b6-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="941b6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="941b6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="941b6-119">Request headers</span></span>
| <span data-ttu-id="941b6-120">名前</span><span class="sxs-lookup"><span data-stu-id="941b6-120">Name</span></span>      |<span data-ttu-id="941b6-121">説明</span><span class="sxs-lookup"><span data-stu-id="941b6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="941b6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="941b6-122">Authorization</span></span>  | <span data-ttu-id="941b6-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="941b6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="941b6-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="941b6-125">Request body</span></span>
<span data-ttu-id="941b6-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="941b6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="941b6-127">応答</span><span class="sxs-lookup"><span data-stu-id="941b6-127">Response</span></span>

<span data-ttu-id="941b6-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[privilegedRoleSummary](../resources/privilegedrolesummary.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="941b6-128">If successful, this method returns a `200 OK` response code and [privilegedRoleSummary](../resources/privilegedrolesummary.md) object in the response body.</span></span>

<span data-ttu-id="941b6-129">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="941b6-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="941b6-130">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="941b6-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="941b6-131">例</span><span class="sxs-lookup"><span data-stu-id="941b6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="941b6-132">要求</span><span class="sxs-lookup"><span data-stu-id="941b6-132">Request</span></span>
<span data-ttu-id="941b6-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="941b6-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="941b6-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="941b6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesummary"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/summary
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="941b6-135">C#</span><span class="sxs-lookup"><span data-stu-id="941b6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedrolesummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="941b6-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="941b6-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedrolesummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="941b6-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="941b6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedrolesummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="941b6-138">Java</span><span class="sxs-lookup"><span data-stu-id="941b6-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedrolesummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="941b6-139">応答</span><span class="sxs-lookup"><span data-stu-id="941b6-139">Response</span></span>
<span data-ttu-id="941b6-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="941b6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleSummary"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 137

{
  "id": "id-value",
  "status": "status-value",
  "usersCount": 99,
  "managedCount": 99,
  "elevatedCount": 99,
  "mfaEnabled": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRoleSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
