---
title: リスト verificationDnsRecords
description: DomainDnsRecord オブジェクトの一覧を取得します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ce414fe23c00e0b4c1254bab968fff1418d881e0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33589281"
---
# <a name="list-verificationdnsrecords"></a><span data-ttu-id="f0434-103">リスト verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="f0434-103">List verificationDnsRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0434-104">[Domaindnsrecord](../resources/domaindnsrecord.md)オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="f0434-104">Retrieve a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects.</span></span>

<span data-ttu-id="f0434-105">所有権が確認されるまで、Azure AD テナントと関連付けられているドメインを使用することはできません。</span><span class="sxs-lookup"><span data-stu-id="f0434-105">You cannot use an associated domain with your Azure AD tenant until ownership is verified.</span></span> <span data-ttu-id="f0434-106">ドメインの所有権を確認するには、ドメインの検証レコードを取得し、ドメインのゾーンファイルに詳細を追加します。</span><span class="sxs-lookup"><span data-stu-id="f0434-106">To verify the ownership of the domain, retrieve the domain verification records and add the details to the zone file of the domain.</span></span> <span data-ttu-id="f0434-107">この操作は、ドメインレジストラーまたは DNS サーバーの構成を使用して行うことができます。</span><span class="sxs-lookup"><span data-stu-id="f0434-107">This can be done through the domain registrar or DNS server configuration.</span></span>

<span data-ttu-id="f0434-108">ルートドメインは検証する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f0434-108">Root domains require verification.</span></span> <span data-ttu-id="f0434-109">たとえば、contoso.com は検証を必要とします。</span><span class="sxs-lookup"><span data-stu-id="f0434-109">For example, contoso.com requires verification.</span></span> <span data-ttu-id="f0434-110">ルートドメインが確認されると、ルートドメインのサブドメインが自動的に確認されます。</span><span class="sxs-lookup"><span data-stu-id="f0434-110">If a root domain is verified, subdomains of the root domain are automatically verified.</span></span> <span data-ttu-id="f0434-111">たとえば、contoso.com が確認されている場合、subdomain.contoso.com は自動的に確認されます。</span><span class="sxs-lookup"><span data-stu-id="f0434-111">For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0434-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f0434-112">Permissions</span></span>

<span data-ttu-id="f0434-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f0434-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f0434-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f0434-115">Permission type</span></span>      | <span data-ttu-id="f0434-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f0434-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0434-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f0434-117">Delegated (work or school account)</span></span> | <span data-ttu-id="f0434-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0434-118">Directory.Read.All</span></span>    |
|<span data-ttu-id="f0434-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f0434-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0434-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0434-120">Not supported.</span></span>    |
|<span data-ttu-id="f0434-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f0434-121">Application</span></span> | <span data-ttu-id="f0434-122">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0434-122">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0434-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f0434-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/verificationDnsRecords
```

> <span data-ttu-id="f0434-124">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="f0434-124">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="f0434-125">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f0434-125">Optional query parameters</span></span>

<span data-ttu-id="f0434-126">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f0434-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f0434-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f0434-127">Request headers</span></span>

| <span data-ttu-id="f0434-128">名前</span><span class="sxs-lookup"><span data-stu-id="f0434-128">Name</span></span>      |<span data-ttu-id="f0434-129">説明</span><span class="sxs-lookup"><span data-stu-id="f0434-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f0434-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0434-130">Authorization</span></span>  | <span data-ttu-id="f0434-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f0434-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f0434-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f0434-133">Content-Type</span></span>  | <span data-ttu-id="f0434-134">application/json</span><span class="sxs-lookup"><span data-stu-id="f0434-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0434-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="f0434-135">Request body</span></span>

<span data-ttu-id="f0434-136">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f0434-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0434-137">応答</span><span class="sxs-lookup"><span data-stu-id="f0434-137">Response</span></span>

<span data-ttu-id="f0434-138">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[domaindnsrecord](../resources/domaindnsrecord.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f0434-138">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0434-139">例</span><span class="sxs-lookup"><span data-stu-id="f0434-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0434-140">要求</span><span class="sxs-lookup"><span data-stu-id="f0434-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_verificationdnsrecords"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com/verificationDnsRecords
```

##### <a name="response"></a><span data-ttu-id="f0434-141">応答</span><span class="sxs-lookup"><span data-stu-id="f0434-141">Response</span></span>

<span data-ttu-id="f0434-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f0434-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f0434-144">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="f0434-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f0434-145">C#</span><span class="sxs-lookup"><span data-stu-id="f0434-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_verificationdnsrecords-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f0434-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="f0434-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_verificationdnsrecords-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List verificationDnsRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-list-verificationdnsrecords.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/domain-list-verificationdnsrecords.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
