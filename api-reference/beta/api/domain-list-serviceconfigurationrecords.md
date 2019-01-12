---
title: serviceConfigurationRecords の一覧表示
description: ドメインのサービスを有効にするために必要な domainDnsRecord オブジェクトの一覧を取得します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2880a8336d15b675cd5debc6008d8de8f4d191f7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965538"
---
# <a name="list-serviceconfigurationrecords"></a><span data-ttu-id="87856-103">serviceConfigurationRecords の一覧表示</span><span class="sxs-lookup"><span data-stu-id="87856-103">List serviceConfigurationRecords</span></span>

> <span data-ttu-id="87856-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="87856-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87856-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87856-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="87856-106">ドメインのサービスを有効にするために必要な [domainDnsRecord](../resources/domaindnsrecord.md) オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="87856-106">Retrieves a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects needed to enable services for the domain.</span></span>

<span data-ttu-id="87856-p102">返される一覧を使用して、ドメインのゾーン ファイルにレコードを追加します。この作業は、ドメイン レジストラーによって、または DNS サーバーの構成で行えます。</span><span class="sxs-lookup"><span data-stu-id="87856-p102">Use the returned list to add records to the zone file of the domain. This can be done through the domain registrar or DNS server configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="87856-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="87856-109">Permissions</span></span>

<span data-ttu-id="87856-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="87856-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="87856-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="87856-112">Permission type</span></span>      | <span data-ttu-id="87856-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="87856-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87856-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="87856-114">Delegated (work or school account)</span></span> | <span data-ttu-id="87856-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="87856-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="87856-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="87856-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87856-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87856-117">Not supported.</span></span>    |
|<span data-ttu-id="87856-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="87856-118">Application</span></span> | <span data-ttu-id="87856-119">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87856-119">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="87856-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="87856-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/contoso.com/serviceConfigurationRecords
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87856-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="87856-121">Optional query parameters</span></span>

<span data-ttu-id="87856-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="87856-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87856-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="87856-123">Request headers</span></span>

| <span data-ttu-id="87856-124">名前</span><span class="sxs-lookup"><span data-stu-id="87856-124">Name</span></span>      |<span data-ttu-id="87856-125">説明</span><span class="sxs-lookup"><span data-stu-id="87856-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="87856-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="87856-126">Authorization</span></span>  | <span data-ttu-id="87856-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="87856-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="87856-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="87856-129">Content-Type</span></span>  | <span data-ttu-id="87856-130">application/json</span><span class="sxs-lookup"><span data-stu-id="87856-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="87856-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="87856-131">Request body</span></span>

<span data-ttu-id="87856-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="87856-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87856-133">応答</span><span class="sxs-lookup"><span data-stu-id="87856-133">Response</span></span>

<span data-ttu-id="87856-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [domainDnsRecord](../resources/domaindnsrecord.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="87856-134">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87856-135">例</span><span class="sxs-lookup"><span data-stu-id="87856-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="87856-136">要求</span><span class="sxs-lookup"><span data-stu-id="87856-136">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceconfigurationrecords"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com/serviceConfigurationRecords
```
##### <a name="response"></a><span data-ttu-id="87856-137">応答</span><span class="sxs-lookup"><span data-stu-id="87856-137">Response</span></span>
<span data-ttu-id="87856-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="87856-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "mailExchange": "contoso-com.mail.protection.outlook.com",
      "preference": 0
    },
    {
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Txt",
      "supportedServices": "Email",
      "ttl": 3600,
      "text": "v=spf1 include: spf.protection.outlook.com ~all"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List serviceConfigurationRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
