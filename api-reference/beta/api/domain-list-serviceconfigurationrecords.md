---
title: serviceConfigurationRecords の一覧表示
description: ドメインのサービスを有効にするために必要な domainDnsRecord オブジェクトの一覧を取得します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1aead8505135347826c4cbca9c758de689549ff1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516995"
---
# <a name="list-serviceconfigurationrecords"></a><span data-ttu-id="220ec-103">serviceConfigurationRecords の一覧表示</span><span class="sxs-lookup"><span data-stu-id="220ec-103">List serviceConfigurationRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="220ec-104">ドメインのサービスを有効にするために必要な [domainDnsRecord](../resources/domaindnsrecord.md) オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="220ec-104">Retrieves a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects needed to enable services for the domain.</span></span>

<span data-ttu-id="220ec-p101">返される一覧を使用して、ドメインのゾーン ファイルにレコードを追加します。この作業は、ドメイン レジストラーによって、または DNS サーバーの構成で行えます。</span><span class="sxs-lookup"><span data-stu-id="220ec-p101">Use the returned list to add records to the zone file of the domain. This can be done through the domain registrar or DNS server configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="220ec-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="220ec-107">Permissions</span></span>

<span data-ttu-id="220ec-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="220ec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="220ec-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="220ec-110">Permission type</span></span>      | <span data-ttu-id="220ec-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="220ec-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="220ec-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="220ec-112">Delegated (work or school account)</span></span> | <span data-ttu-id="220ec-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="220ec-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="220ec-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="220ec-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="220ec-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="220ec-115">Not supported.</span></span>    |
|<span data-ttu-id="220ec-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="220ec-116">Application</span></span> | <span data-ttu-id="220ec-117">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="220ec-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="220ec-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="220ec-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/contoso.com/serviceConfigurationRecords
```

## <a name="optional-query-parameters"></a><span data-ttu-id="220ec-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="220ec-119">Optional query parameters</span></span>

<span data-ttu-id="220ec-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="220ec-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="220ec-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="220ec-121">Request headers</span></span>

| <span data-ttu-id="220ec-122">名前</span><span class="sxs-lookup"><span data-stu-id="220ec-122">Name</span></span>      |<span data-ttu-id="220ec-123">説明</span><span class="sxs-lookup"><span data-stu-id="220ec-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="220ec-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="220ec-124">Authorization</span></span>  | <span data-ttu-id="220ec-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="220ec-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="220ec-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="220ec-127">Content-Type</span></span>  | <span data-ttu-id="220ec-128">application/json</span><span class="sxs-lookup"><span data-stu-id="220ec-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="220ec-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="220ec-129">Request body</span></span>

<span data-ttu-id="220ec-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="220ec-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="220ec-131">応答</span><span class="sxs-lookup"><span data-stu-id="220ec-131">Response</span></span>

<span data-ttu-id="220ec-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [domainDnsRecord](../resources/domaindnsrecord.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="220ec-132">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="220ec-133">例</span><span class="sxs-lookup"><span data-stu-id="220ec-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="220ec-134">要求</span><span class="sxs-lookup"><span data-stu-id="220ec-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceconfigurationrecords"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com/serviceConfigurationRecords
```
##### <a name="response"></a><span data-ttu-id="220ec-135">応答</span><span class="sxs-lookup"><span data-stu-id="220ec-135">Response</span></span>
<span data-ttu-id="220ec-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="220ec-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List serviceConfigurationRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-list-serviceconfigurationrecords.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
