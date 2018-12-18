---
title: verificationDnsRecords を一覧表示する
description: domainDnsRecord オブジェクトの一覧を取得します。
author: lleonard-msft
ms.openlocfilehash: 9f9fd611b590c3ace61394309637340288cf7bb5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353103"
---
# <a name="list-verificationdnsrecords"></a><span data-ttu-id="bbdaa-103">verificationDnsRecords を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="bbdaa-103">List verificationDnsRecords</span></span>

<span data-ttu-id="bbdaa-104">[domainDnsRecord](../resources/domaindnsrecord.md) オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="bbdaa-104">Retrieve a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects.</span></span>

<span data-ttu-id="bbdaa-p101">所有権を検証しないと、関連するドメインを Azure AD テナントで使用することはできません。ドメインの所有権を検証するには、ドメイン検証レコードを取得し、ドメインのゾーン ファイルに詳細を追加します。この作業は、ドメイン レジストラーによって、または DNS サーバーの構成で行えます。</span><span class="sxs-lookup"><span data-stu-id="bbdaa-p101">You cannot use an associated domain with your Azure AD tenant until ownership is verified. To verify the ownership of the domain, retrieve the domain verification records and add the details to the zone file of the domain. This can be done through the domain registrar or DNS server configuration.</span></span>

<span data-ttu-id="bbdaa-p102">ルート ドメインには検証が必要です。たとえば、contoso.com には検証が必要です。ルート ドメインが検証されると、ルート ドメインのサブドメインが自動的に検証されます。たとえば、contoso.com が検証されると、subdomain.contoso.com が自動的に検証されます。</span><span class="sxs-lookup"><span data-stu-id="bbdaa-p102">Root domains require verification. For example, contoso.com requires verification. If a root domain is verified, subdomains of the root domain are automatically verified. For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbdaa-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bbdaa-112">Permissions</span></span>

<span data-ttu-id="bbdaa-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bbdaa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bbdaa-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bbdaa-115">Permission type</span></span>      | <span data-ttu-id="bbdaa-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bbdaa-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bbdaa-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bbdaa-117">Delegated (work or school account)</span></span> | <span data-ttu-id="bbdaa-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbdaa-118">Directory.Read.All</span></span>    |
|<span data-ttu-id="bbdaa-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bbdaa-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbdaa-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bbdaa-120">Not supported.</span></span>    |
|<span data-ttu-id="bbdaa-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bbdaa-121">Application</span></span> | <span data-ttu-id="bbdaa-122">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbdaa-122">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbdaa-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bbdaa-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/verificationDnsRecords
```

> <span data-ttu-id="bbdaa-124">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="bbdaa-124">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="bbdaa-125">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="bbdaa-125">Optional query parameters</span></span>

<span data-ttu-id="bbdaa-126">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="bbdaa-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bbdaa-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bbdaa-127">Request headers</span></span>

| <span data-ttu-id="bbdaa-128">名前</span><span class="sxs-lookup"><span data-stu-id="bbdaa-128">Name</span></span>      |<span data-ttu-id="bbdaa-129">説明</span><span class="sxs-lookup"><span data-stu-id="bbdaa-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bbdaa-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbdaa-130">Authorization</span></span>  | <span data-ttu-id="bbdaa-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bbdaa-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bbdaa-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bbdaa-133">Content-Type</span></span>  | <span data-ttu-id="bbdaa-134">application/json</span><span class="sxs-lookup"><span data-stu-id="bbdaa-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bbdaa-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="bbdaa-135">Request body</span></span>

<span data-ttu-id="bbdaa-136">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bbdaa-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbdaa-137">応答</span><span class="sxs-lookup"><span data-stu-id="bbdaa-137">Response</span></span>

<span data-ttu-id="bbdaa-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [domainDnsRecord](../resources/domaindnsrecord.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="bbdaa-138">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbdaa-139">例</span><span class="sxs-lookup"><span data-stu-id="bbdaa-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bbdaa-140">要求</span><span class="sxs-lookup"><span data-stu-id="bbdaa-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_verificationdnsrecords"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/verificationDnsRecords
```

##### <a name="response"></a><span data-ttu-id="bbdaa-141">応答</span><span class="sxs-lookup"><span data-stu-id="bbdaa-141">Response</span></span>

<span data-ttu-id="bbdaa-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bbdaa-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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