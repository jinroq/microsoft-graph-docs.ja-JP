---
title: グループ設定を取得する
description: グループ設定オブジェクトの特定のプロパティを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c577e327534c6c96637a27f74edb40fb0b0a3cf0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373304"
---
# <a name="get-a-group-setting"></a><span data-ttu-id="55a01-103">グループ設定を取得する</span><span class="sxs-lookup"><span data-stu-id="55a01-103">Get a group setting</span></span>

<span data-ttu-id="55a01-104">グループ設定オブジェクトの特定のプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="55a01-104">Retrieve the properties of a specific of group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="55a01-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="55a01-105">Permissions</span></span>

<span data-ttu-id="55a01-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="55a01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="55a01-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="55a01-108">Permission type</span></span>      | <span data-ttu-id="55a01-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="55a01-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55a01-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="55a01-110">Delegated (work or school account)</span></span> | <span data-ttu-id="55a01-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="55a01-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="55a01-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="55a01-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55a01-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="55a01-113">Not supported.</span></span>    |
|<span data-ttu-id="55a01-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="55a01-114">Application</span></span> | <span data-ttu-id="55a01-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55a01-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="55a01-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="55a01-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="55a01-117">特定のテナント全体またはグループ設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="55a01-117">Get a specific tenant-wide or group setting.</span></span>

```http
GET /groupSettings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="55a01-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="55a01-118">Optional query parameters</span></span>
<span data-ttu-id="55a01-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="55a01-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="55a01-120">注: $filter はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="55a01-120">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55a01-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="55a01-121">Request headers</span></span>
| <span data-ttu-id="55a01-122">名前</span><span class="sxs-lookup"><span data-stu-id="55a01-122">Name</span></span> | <span data-ttu-id="55a01-123">説明</span><span class="sxs-lookup"><span data-stu-id="55a01-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="55a01-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="55a01-124">Authorization</span></span> | <span data-ttu-id="55a01-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="55a01-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55a01-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="55a01-127">Request body</span></span>

<span data-ttu-id="55a01-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="55a01-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55a01-129">応答</span><span class="sxs-lookup"><span data-stu-id="55a01-129">Response</span></span>

<span data-ttu-id="55a01-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[groupsetting](../resources/groupsetting.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="55a01-130">If successful, this method returns a `200 OK` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55a01-131">例</span><span class="sxs-lookup"><span data-stu-id="55a01-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="55a01-132">要求</span><span class="sxs-lookup"><span data-stu-id="55a01-132">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="55a01-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="55a01-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsetting"
}-->

```http
GET https://graph.microsoft.com/v1.0/groupSettings/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="55a01-134">C#</span><span class="sxs-lookup"><span data-stu-id="55a01-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="55a01-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55a01-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="55a01-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="55a01-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="55a01-137">Java</span><span class="sxs-lookup"><span data-stu-id="55a01-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="55a01-138">応答</span><span class="sxs-lookup"><span data-stu-id="55a01-138">Response</span></span>

<span data-ttu-id="55a01-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="55a01-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ],
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
