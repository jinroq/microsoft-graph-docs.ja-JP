---
title: ドメインを作成する
description: テナントにドメインを追加します。
author: lleonard-msft
ms.openlocfilehash: c7b64f2d6df2279f248fe41ad23e3bfc0d9636de
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324830"
---
# <a name="create-domain"></a><span data-ttu-id="b7f1e-103">ドメインを作成する</span><span class="sxs-lookup"><span data-stu-id="b7f1e-103">Create domain</span></span>

<span data-ttu-id="b7f1e-104">テナントにドメインを追加します。</span><span class="sxs-lookup"><span data-stu-id="b7f1e-104">Adds a domain to the tenant.</span></span>

<span data-ttu-id="b7f1e-p101">**重要**:所有権を検証しないと、関連するドメインを Azure AD テナントで使用することはできません。詳細については、「[verificationDnsRecords の一覧](domain-list-verificationdnsrecords.md)」を参照してください。ルート ドメインには検証が必要です。たとえば、contoso.com には検証が必要です。ルート ドメインが検証されると、ルート ドメインのサブドメインが自動的に検証されます。たとえば、contoso.com が検証されると、subdomain.contoso.com が自動的に検証されます。</span><span class="sxs-lookup"><span data-stu-id="b7f1e-p101">**Important**: You cannot use an associated domain with your Azure AD tenant until ownership is verified. See [List verificationDnsRecords](domain-list-verificationdnsrecords.md) for details. Root domains require verification. For example, contoso.com requires verification. If a root domain is verified, subdomains of the root domain are automatically verified. For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7f1e-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b7f1e-111">Permissions</span></span>

<span data-ttu-id="b7f1e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7f1e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b7f1e-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b7f1e-114">Permission type</span></span>      | <span data-ttu-id="b7f1e-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b7f1e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7f1e-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b7f1e-116">Delegated (work or school account)</span></span> | <span data-ttu-id="b7f1e-117">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b7f1e-117">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b7f1e-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b7f1e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7f1e-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7f1e-119">Not supported.</span></span>    |
|<span data-ttu-id="b7f1e-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b7f1e-120">Application</span></span> | <span data-ttu-id="b7f1e-121">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7f1e-121">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7f1e-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b7f1e-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains
```
## <a name="request-headers"></a><span data-ttu-id="b7f1e-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b7f1e-123">Request headers</span></span>
| <span data-ttu-id="b7f1e-124">名前</span><span class="sxs-lookup"><span data-stu-id="b7f1e-124">Name</span></span>       | <span data-ttu-id="b7f1e-125">説明</span><span class="sxs-lookup"><span data-stu-id="b7f1e-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b7f1e-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7f1e-126">Authorization</span></span>  | <span data-ttu-id="b7f1e-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b7f1e-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="b7f1e-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b7f1e-129">Content-Type</span></span>  | <span data-ttu-id="b7f1e-130">application/json</span><span class="sxs-lookup"><span data-stu-id="b7f1e-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7f1e-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="b7f1e-131">Request body</span></span>
<span data-ttu-id="b7f1e-132">要求本文で、[domain](../resources/domain.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b7f1e-132">In the request body, supply a JSON representation of [domain](../resources/domain.md) object.</span></span>

> <span data-ttu-id="b7f1e-p104">要求本文には、新しいドメインの id プロパティが含まれます。id は指定できる唯一のプロパティで、必須です。id プロパティ値は、作成する完全修飾ドメイン名です。</span><span class="sxs-lookup"><span data-stu-id="b7f1e-p104">The request body contains the id property for the new domain. Id is the only property that can be specified and it is required. The id property value is the fully qualified domain name to create.</span></span>

## <a name="response"></a><span data-ttu-id="b7f1e-136">応答</span><span class="sxs-lookup"><span data-stu-id="b7f1e-136">Response</span></span>

<span data-ttu-id="b7f1e-137">成功した場合、このメソッドは応答本文で `201 Created` 応答コードと [domain](../resources/domain.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b7f1e-137">If successful, this method returns `201 Created` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7f1e-138">例</span><span class="sxs-lookup"><span data-stu-id="b7f1e-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b7f1e-139">要求</span><span class="sxs-lookup"><span data-stu-id="b7f1e-139">Request</span></span>

<span data-ttu-id="b7f1e-140">要求本文で、[domain](../resources/domain.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b7f1e-140">In the request body, supply a JSON representation of [domain](../resources/domain.md) object.</span></span>

<!-- {
  "blockType": "request",
  "id": "create_domain_from_domains"
}-->
```http
POST https://graph.microsoft.com/v1.0/domains
Content-type: application/json
Content-length: 192

{
  "id": "contoso.com"
}
```

##### <a name="response"></a><span data-ttu-id="b7f1e-141">応答</span><span class="sxs-lookup"><span data-stu-id="b7f1e-141">Response</span></span>
<span data-ttu-id="b7f1e-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b7f1e-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->