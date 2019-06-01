---
title: 組織を取得する
description: 現在認証されている組織のプロパティとリレーションシップを取得します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 54e5db4b3c8c0c279ef618e27911b8460a5669eb
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657302"
---
# <a name="get-organization"></a><span data-ttu-id="7223d-103">組織を取得する</span><span class="sxs-lookup"><span data-stu-id="7223d-103">Get organization</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7223d-104">現在認証されている組織のプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="7223d-104">Retrieve the properties and relationships of currently authenticated organization.</span></span>

<span data-ttu-id="7223d-105">**組織**のリソースは[拡張機能](/graph/extensibility-overview)をサポートしているため`GET` 、この操作を使用して、**組織**のインスタンスでカスタムプロパティと拡張機能データを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="7223d-105">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **organization** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="7223d-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7223d-106">Permissions</span></span>

<span data-ttu-id="7223d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7223d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7223d-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7223d-109">Permission type</span></span> | <span data-ttu-id="7223d-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7223d-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7223d-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7223d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7223d-112">User. 読み取り、ディレクトリ</span><span class="sxs-lookup"><span data-stu-id="7223d-112">User.Read, Directory.Read.All</span></span> |
|<span data-ttu-id="7223d-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7223d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7223d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7223d-114">Not supported.</span></span> |
|<span data-ttu-id="7223d-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7223d-115">Application</span></span> | <span data-ttu-id="7223d-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7223d-116">Directory.Read.All</span></span> |

> <span data-ttu-id="7223d-117">注: User.Read アクセス許可を付与されたアプリケーションは、組織の *id*、*displayName*、および *verifiedDomains* プロパティのみを読み取ることができます。</span><span class="sxs-lookup"><span data-stu-id="7223d-117">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="7223d-118">他のすべてのプロパティは `null` 値を返します。</span><span class="sxs-lookup"><span data-stu-id="7223d-118">All other properties will return with `null` values.</span></span> <span data-ttu-id="7223d-119">すべてのプロパティを読み取るには、Directory.Read.All を使用します。</span><span class="sxs-lookup"><span data-stu-id="7223d-119">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="7223d-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7223d-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7223d-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7223d-121">Optional query parameters</span></span>

<span data-ttu-id="7223d-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7223d-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7223d-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7223d-123">Request headers</span></span>

| <span data-ttu-id="7223d-124">名前</span><span class="sxs-lookup"><span data-stu-id="7223d-124">Name</span></span>       | <span data-ttu-id="7223d-125">型</span><span class="sxs-lookup"><span data-stu-id="7223d-125">Type</span></span> | <span data-ttu-id="7223d-126">説明</span><span class="sxs-lookup"><span data-stu-id="7223d-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7223d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="7223d-127">Authorization</span></span>  | <span data-ttu-id="7223d-128">string</span><span class="sxs-lookup"><span data-stu-id="7223d-128">string</span></span>  | <span data-ttu-id="7223d-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7223d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7223d-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="7223d-131">Request body</span></span>

<span data-ttu-id="7223d-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7223d-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7223d-133">応答</span><span class="sxs-lookup"><span data-stu-id="7223d-133">Response</span></span>

<span data-ttu-id="7223d-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [organization](../resources/organization.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7223d-134">If successful, this method returns a `200 OK` response code and [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7223d-135">例</span><span class="sxs-lookup"><span data-stu-id="7223d-135">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7223d-136">要求</span><span class="sxs-lookup"><span data-stu-id="7223d-136">Request</span></span>

<span data-ttu-id="7223d-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7223d-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->

```http
GET https://graph.microsoft.com/beta/organization
```

##### <a name="response"></a><span data-ttu-id="7223d-138">応答</span><span class="sxs-lookup"><span data-stu-id="7223d-138">Response</span></span>

<span data-ttu-id="7223d-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7223d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 411

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#organization",
  "value": [
    {
      "assignedPlans": [
        {
          "assignedDateTime": "datetime-value",
          "capabilityStatus": "capabilityStatus-value",
          "service": "service-value",
          "servicePlanId": "servicePlanId-value"
        }
      ],
      "businessPhones": [
        "businessPhones-value"
      ],
      "city": "city-value",
      "country": "country-value",
      "countryLetterCode": "countryLetterCode-value",
      "displayName": "displayName-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7223d-142">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="7223d-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7223d-143">C#</span><span class="sxs-lookup"><span data-stu-id="7223d-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_organization-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7223d-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="7223d-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_organization-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="7223d-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="7223d-145">See also</span></span>

- [<span data-ttu-id="7223d-146">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="7223d-146">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="7223d-147">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="7223d-147">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/organization-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/organization-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
