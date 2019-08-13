---
title: リスト serviceConfigurationRecords
description: ドメインのサービスを有効にするために必要な domainDnsRecord オブジェクトの一覧を取得します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8336344385ffffc4a27666c047607d227dd609d7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324601"
---
# <a name="list-serviceconfigurationrecords"></a><span data-ttu-id="e495c-103">リスト serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="e495c-103">List serviceConfigurationRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e495c-104">ドメインのサービスを有効にするために必要な[Domaindnsrecord](../resources/domaindnsrecord.md)オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="e495c-104">Retrieves a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects needed to enable services for the domain.</span></span>

<span data-ttu-id="e495c-105">返された一覧を使用して、ドメインのゾーンファイルにレコードを追加します。</span><span class="sxs-lookup"><span data-stu-id="e495c-105">Use the returned list to add records to the zone file of the domain.</span></span> <span data-ttu-id="e495c-106">この操作は、ドメインレジストラーまたは DNS サーバーの構成を使用して行うことができます。</span><span class="sxs-lookup"><span data-stu-id="e495c-106">This can be done through the domain registrar or DNS server configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="e495c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e495c-107">Permissions</span></span>

<span data-ttu-id="e495c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e495c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e495c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e495c-110">Permission type</span></span>      | <span data-ttu-id="e495c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e495c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e495c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e495c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e495c-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e495c-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="e495c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e495c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e495c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e495c-115">Not supported.</span></span>    |
|<span data-ttu-id="e495c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e495c-116">Application</span></span> | <span data-ttu-id="e495c-117">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e495c-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e495c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e495c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/contoso.com/serviceConfigurationRecords
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e495c-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e495c-119">Optional query parameters</span></span>

<span data-ttu-id="e495c-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e495c-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e495c-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e495c-121">Request headers</span></span>

| <span data-ttu-id="e495c-122">名前</span><span class="sxs-lookup"><span data-stu-id="e495c-122">Name</span></span>      |<span data-ttu-id="e495c-123">説明</span><span class="sxs-lookup"><span data-stu-id="e495c-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e495c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e495c-124">Authorization</span></span>  | <span data-ttu-id="e495c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e495c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e495c-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e495c-127">Content-Type</span></span>  | <span data-ttu-id="e495c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e495c-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e495c-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="e495c-129">Request body</span></span>

<span data-ttu-id="e495c-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e495c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e495c-131">応答</span><span class="sxs-lookup"><span data-stu-id="e495c-131">Response</span></span>

<span data-ttu-id="e495c-132">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[domaindnsrecord](../resources/domaindnsrecord.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e495c-132">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e495c-133">例</span><span class="sxs-lookup"><span data-stu-id="e495c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e495c-134">要求</span><span class="sxs-lookup"><span data-stu-id="e495c-134">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e495c-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e495c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceconfigurationrecords"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com/serviceConfigurationRecords
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e495c-136">C#</span><span class="sxs-lookup"><span data-stu-id="e495c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceconfigurationrecords-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e495c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e495c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceconfigurationrecords-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e495c-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="e495c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceconfigurationrecords-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e495c-139">Java</span><span class="sxs-lookup"><span data-stu-id="e495c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceconfigurationrecords-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e495c-140">応答</span><span class="sxs-lookup"><span data-stu-id="e495c-140">Response</span></span>
<span data-ttu-id="e495c-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e495c-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
