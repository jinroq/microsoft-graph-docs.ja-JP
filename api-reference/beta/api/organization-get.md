---
title: 組織を取得する
description: 現在認証されている組織のプロパティとリレーションシップを取得します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c4f0b325100ac8543e51320609e8c4e39ce130fc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915453"
---
# <a name="get-organization"></a><span data-ttu-id="15193-103">組織を取得する</span><span class="sxs-lookup"><span data-stu-id="15193-103">Get organization</span></span>

> <span data-ttu-id="15193-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="15193-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15193-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15193-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="15193-106">現在認証されている組織のプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="15193-106">Retrieve the properties and relationships of currently authenticated organization.</span></span>

<span data-ttu-id="15193-107">**組織**のリソースは、[拡張機能](/graph/extensibility-overview)をサポートするため使用することも、 `GET` **組織**インスタンスのカスタム プロパティと拡張機能のデータを取得する操作です。</span><span class="sxs-lookup"><span data-stu-id="15193-107">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **organization** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="15193-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="15193-108">Permissions</span></span>

<span data-ttu-id="15193-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="15193-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15193-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="15193-111">Permission type</span></span> | <span data-ttu-id="15193-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="15193-112">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15193-113">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="15193-113">Delegated (work or school account)</span></span> | <span data-ttu-id="15193-114">User.Read、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="15193-114">User.Read, Directory.Read.All</span></span> |
|<span data-ttu-id="15193-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="15193-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15193-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15193-116">Not supported.</span></span> |
|<span data-ttu-id="15193-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="15193-117">Application</span></span> | <span data-ttu-id="15193-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="15193-118">Directory.Read.All</span></span> |

> <span data-ttu-id="15193-119">注: User.Read アクセス許可を付与されたアプリケーションは、組織の *id*、*displayName*、および *verifiedDomains* プロパティのみを読み取ることができます。</span><span class="sxs-lookup"><span data-stu-id="15193-119">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="15193-120">他のすべてのプロパティは `null` 値を返します。</span><span class="sxs-lookup"><span data-stu-id="15193-120">All other properties will return with `null` values.</span></span> <span data-ttu-id="15193-121">すべてのプロパティを読み取るには、Directory.Read.All を使用します。</span><span class="sxs-lookup"><span data-stu-id="15193-121">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="15193-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="15193-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="15193-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="15193-123">Optional query parameters</span></span>

<span data-ttu-id="15193-124">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="15193-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="15193-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="15193-125">Request headers</span></span>

| <span data-ttu-id="15193-126">名前</span><span class="sxs-lookup"><span data-stu-id="15193-126">Name</span></span>       | <span data-ttu-id="15193-127">型</span><span class="sxs-lookup"><span data-stu-id="15193-127">Type</span></span> | <span data-ttu-id="15193-128">説明</span><span class="sxs-lookup"><span data-stu-id="15193-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="15193-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="15193-129">Authorization</span></span>  | <span data-ttu-id="15193-130">string</span><span class="sxs-lookup"><span data-stu-id="15193-130">string</span></span>  | <span data-ttu-id="15193-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="15193-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15193-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="15193-133">Request body</span></span>

<span data-ttu-id="15193-134">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="15193-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15193-135">応答</span><span class="sxs-lookup"><span data-stu-id="15193-135">Response</span></span>

<span data-ttu-id="15193-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [organization](../resources/organization.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="15193-136">If successful, this method returns a `200 OK` response code and [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15193-137">例</span><span class="sxs-lookup"><span data-stu-id="15193-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="15193-138">要求</span><span class="sxs-lookup"><span data-stu-id="15193-138">Request</span></span>

<span data-ttu-id="15193-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="15193-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->

```http
GET https://graph.microsoft.com/beta/organization
```

##### <a name="response"></a><span data-ttu-id="15193-140">応答</span><span class="sxs-lookup"><span data-stu-id="15193-140">Response</span></span>

<span data-ttu-id="15193-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="15193-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="15193-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="15193-144">See also</span></span>

- [<span data-ttu-id="15193-145">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="15193-145">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="15193-146">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="15193-146">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
