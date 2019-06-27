---
title: グループ設定を取得する
description: グループ設定オブジェクトの特定のプロパティを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 393d45863183a860417a2066f8b6502df59eff05
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272283"
---
# <a name="get-a-group-setting"></a><span data-ttu-id="7307a-103">グループ設定を取得する</span><span class="sxs-lookup"><span data-stu-id="7307a-103">Get a group setting</span></span>

<span data-ttu-id="7307a-104">グループ設定オブジェクトの特定のプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="7307a-104">Retrieve the properties of a specific of group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7307a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7307a-105">Permissions</span></span>

<span data-ttu-id="7307a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7307a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7307a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7307a-108">Permission type</span></span>      | <span data-ttu-id="7307a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7307a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7307a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7307a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7307a-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7307a-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7307a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7307a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7307a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7307a-113">Not supported.</span></span>    |
|<span data-ttu-id="7307a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7307a-114">Application</span></span> | <span data-ttu-id="7307a-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7307a-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7307a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7307a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="7307a-117">特定のテナント全体またはグループ設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="7307a-117">Get a specific tenant-wide or group setting.</span></span>

```http
GET /groupSettings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7307a-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7307a-118">Optional query parameters</span></span>
<span data-ttu-id="7307a-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7307a-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="7307a-120">注: $filter はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7307a-120">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7307a-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7307a-121">Request headers</span></span>
| <span data-ttu-id="7307a-122">名前</span><span class="sxs-lookup"><span data-stu-id="7307a-122">Name</span></span> | <span data-ttu-id="7307a-123">説明</span><span class="sxs-lookup"><span data-stu-id="7307a-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="7307a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7307a-124">Authorization</span></span> | <span data-ttu-id="7307a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7307a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7307a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7307a-127">Request body</span></span>

<span data-ttu-id="7307a-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7307a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7307a-129">応答</span><span class="sxs-lookup"><span data-stu-id="7307a-129">Response</span></span>

<span data-ttu-id="7307a-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[groupsetting](../resources/groupsetting.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7307a-130">If successful, this method returns a `200 OK` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7307a-131">例</span><span class="sxs-lookup"><span data-stu-id="7307a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7307a-132">要求</span><span class="sxs-lookup"><span data-stu-id="7307a-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsetting"
}-->

```http
GET https://graph.microsoft.com/v1.0/groupSettings/{id}
```
##### <a name="response"></a><span data-ttu-id="7307a-133">応答</span><span class="sxs-lookup"><span data-stu-id="7307a-133">Response</span></span>

<span data-ttu-id="7307a-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7307a-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7307a-136">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="7307a-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7307a-137">C#</span><span class="sxs-lookup"><span data-stu-id="7307a-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_groupsetting-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7307a-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="7307a-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_groupsetting-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7307a-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="7307a-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_groupsetting-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/groupsetting-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/groupsetting-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/groupsetting-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
