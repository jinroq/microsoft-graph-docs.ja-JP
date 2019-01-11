---
title: verificationDnsRecords を一覧表示する
description: domainDnsRecord オブジェクトの一覧を取得します。
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 335fd90dc56903061f1c5c5bb86672de1a438fcb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874901"
---
# <a name="list-verificationdnsrecords"></a><span data-ttu-id="fbd0e-103">verificationDnsRecords を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="fbd0e-103">List verificationDnsRecords</span></span>

> <span data-ttu-id="fbd0e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fbd0e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fbd0e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fbd0e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fbd0e-106">[domainDnsRecord](../resources/domaindnsrecord.md) オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="fbd0e-106">Retrieve a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects.</span></span>

<span data-ttu-id="fbd0e-p102">所有権を検証しないと、関連するドメインを Azure AD テナントで使用することはできません。ドメインの所有権を検証するには、ドメイン検証レコードを取得し、ドメインのゾーン ファイルに詳細を追加します。この作業は、ドメイン レジストラーによって、または DNS サーバーの構成で行えます。</span><span class="sxs-lookup"><span data-stu-id="fbd0e-p102">You cannot use an associated domain with your Azure AD tenant until ownership is verified. To verify the ownership of the domain, retrieve the domain verification records and add the details to the zone file of the domain. This can be done through the domain registrar or DNS server configuration.</span></span>

<span data-ttu-id="fbd0e-p103">ルート ドメインには検証が必要です。たとえば、contoso.com には検証が必要です。ルート ドメインが検証されると、ルート ドメインのサブドメインが自動的に検証されます。たとえば、contoso.com が検証されると、subdomain.contoso.com が自動的に検証されます。</span><span class="sxs-lookup"><span data-stu-id="fbd0e-p103">Root domains require verification. For example, contoso.com requires verification. If a root domain is verified, subdomains of the root domain are automatically verified. For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="fbd0e-114">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fbd0e-114">Permissions</span></span>

<span data-ttu-id="fbd0e-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fbd0e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fbd0e-117">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fbd0e-117">Permission type</span></span>      | <span data-ttu-id="fbd0e-118">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fbd0e-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fbd0e-119">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fbd0e-119">Delegated (work or school account)</span></span> | <span data-ttu-id="fbd0e-120">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbd0e-120">Directory.Read.All</span></span>    |
|<span data-ttu-id="fbd0e-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fbd0e-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbd0e-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fbd0e-122">Not supported.</span></span>    |
|<span data-ttu-id="fbd0e-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fbd0e-123">Application</span></span> | <span data-ttu-id="fbd0e-124">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbd0e-124">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fbd0e-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fbd0e-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/verificationDnsRecords
```

> <span data-ttu-id="fbd0e-126">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="fbd0e-126">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="fbd0e-127">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="fbd0e-127">Optional query parameters</span></span>

<span data-ttu-id="fbd0e-128">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="fbd0e-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fbd0e-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fbd0e-129">Request headers</span></span>

| <span data-ttu-id="fbd0e-130">名前</span><span class="sxs-lookup"><span data-stu-id="fbd0e-130">Name</span></span>      |<span data-ttu-id="fbd0e-131">説明</span><span class="sxs-lookup"><span data-stu-id="fbd0e-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fbd0e-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbd0e-132">Authorization</span></span>  | <span data-ttu-id="fbd0e-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fbd0e-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fbd0e-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fbd0e-135">Content-Type</span></span>  | <span data-ttu-id="fbd0e-136">application/json</span><span class="sxs-lookup"><span data-stu-id="fbd0e-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="fbd0e-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="fbd0e-137">Request body</span></span>

<span data-ttu-id="fbd0e-138">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fbd0e-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbd0e-139">応答</span><span class="sxs-lookup"><span data-stu-id="fbd0e-139">Response</span></span>

<span data-ttu-id="fbd0e-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [domainDnsRecord](../resources/domaindnsrecord.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="fbd0e-140">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbd0e-141">例</span><span class="sxs-lookup"><span data-stu-id="fbd0e-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fbd0e-142">要求</span><span class="sxs-lookup"><span data-stu-id="fbd0e-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_verificationdnsrecords"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com/verificationDnsRecords
```

##### <a name="response"></a><span data-ttu-id="fbd0e-143">応答</span><span class="sxs-lookup"><span data-stu-id="fbd0e-143">Response</span></span>

<span data-ttu-id="fbd0e-p106">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fbd0e-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domainDnsRecord",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 220

{
  "value": [
    {
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Mx",
      "supportedService": "Email",
      "ttl": 3600,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List verificationDnsRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
