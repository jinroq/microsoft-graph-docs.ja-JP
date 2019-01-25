---
title: IdentityProvider を取得します。
description: 既存の identityProvider のプロパティを取得します。
localization_priority: Normal
ms.openlocfilehash: 8315c43bcd99b9ea96b408cd2feb61a59369e4c1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523072"
---
# <a name="get-identityprovider"></a><span data-ttu-id="b0c5a-103">IdentityProvider を取得します。</span><span class="sxs-lookup"><span data-stu-id="b0c5a-103">Get identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0c5a-104">既存の[identityProvider](../resources/identityprovider.md)のプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="b0c5a-104">Retrieve the properties of an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b0c5a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b0c5a-105">Permissions</span></span>

<span data-ttu-id="b0c5a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0c5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0c5a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b0c5a-108">Permission type</span></span>      | <span data-ttu-id="b0c5a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b0c5a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0c5a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b0c5a-110">Delegated (work or school account)</span></span>|<span data-ttu-id="b0c5a-111">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0c5a-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="b0c5a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b0c5a-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="b0c5a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0c5a-113">Not supported.</span></span>|
|<span data-ttu-id="b0c5a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b0c5a-114">Application</span></span>|<span data-ttu-id="b0c5a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0c5a-115">Not supported.</span></span>|

<span data-ttu-id="b0c5a-116">職場または学校のアカウントは、テナントのグローバル ・ アドミニストレーターである必要があります。</span><span class="sxs-lookup"><span data-stu-id="b0c5a-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="b0c5a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b0c5a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b0c5a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b0c5a-118">Request headers</span></span>

|<span data-ttu-id="b0c5a-119">名前</span><span class="sxs-lookup"><span data-stu-id="b0c5a-119">Name</span></span>|<span data-ttu-id="b0c5a-120">説明</span><span class="sxs-lookup"><span data-stu-id="b0c5a-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="b0c5a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0c5a-121">Authorization</span></span>|<span data-ttu-id="b0c5a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b0c5a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0c5a-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="b0c5a-124">Request body</span></span>

<span data-ttu-id="b0c5a-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b0c5a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0c5a-126">応答</span><span class="sxs-lookup"><span data-stu-id="b0c5a-126">Response</span></span>

<span data-ttu-id="b0c5a-127">かどうかは成功すると、このメソッドを返します`200 OK`応答コードおよび応答の本文に[identityProvider](../resources/identityprovider.md)の JSON 形式です。</span><span class="sxs-lookup"><span data-stu-id="b0c5a-127">If successful, this method returns `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0c5a-128">例</span><span class="sxs-lookup"><span data-stu-id="b0c5a-128">Example</span></span>

<span data-ttu-id="b0c5a-129">次の例では、特定の**identityProvider**を取得します。</span><span class="sxs-lookup"><span data-stu-id="b0c5a-129">The following example retrieves a specific **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="b0c5a-130">要求</span><span class="sxs-lookup"><span data-stu-id="b0c5a-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="b0c5a-131">応答</span><span class="sxs-lookup"><span data-stu-id="b0c5a-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "type": "Amazon",
    "name": "Login with Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/identityprovider-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
