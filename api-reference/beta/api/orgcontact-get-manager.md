---
title: 'orgcontact: 上司の取得'
description: 連絡先の上司を取得する
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 96833e9b38b2d988a3843e097a11fe38a247c0b6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539845"
---
# <a name="orgcontact-get-manager"></a><span data-ttu-id="cc056-103">orgcontact: 上司の取得</span><span class="sxs-lookup"><span data-stu-id="cc056-103">orgContact: Get manager</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc056-104">連絡先の上司を取得する</span><span class="sxs-lookup"><span data-stu-id="cc056-104">Get the contact's manager</span></span>

## <a name="permissions"></a><span data-ttu-id="cc056-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cc056-105">Permissions</span></span>
<span data-ttu-id="cc056-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc056-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc056-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cc056-108">Permission type</span></span>      | <span data-ttu-id="cc056-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cc056-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc056-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cc056-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cc056-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cc056-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cc056-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cc056-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc056-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc056-113">Not supported.</span></span>    |
|<span data-ttu-id="cc056-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cc056-114">Application</span></span> | <span data-ttu-id="cc056-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc056-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc056-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cc056-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /contacts/{id}/manager
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cc056-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="cc056-117">Optional query parameters</span></span>
<span data-ttu-id="cc056-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="cc056-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc056-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc056-119">Request headers</span></span>
| <span data-ttu-id="cc056-120">名前</span><span class="sxs-lookup"><span data-stu-id="cc056-120">Name</span></span>       | <span data-ttu-id="cc056-121">型</span><span class="sxs-lookup"><span data-stu-id="cc056-121">Type</span></span> | <span data-ttu-id="cc056-122">説明</span><span class="sxs-lookup"><span data-stu-id="cc056-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cc056-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc056-123">Authorization</span></span>  | <span data-ttu-id="cc056-124">string</span><span class="sxs-lookup"><span data-stu-id="cc056-124">string</span></span>  | <span data-ttu-id="cc056-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cc056-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc056-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="cc056-127">Request body</span></span>
<span data-ttu-id="cc056-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cc056-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc056-129">応答</span><span class="sxs-lookup"><span data-stu-id="cc056-129">Response</span></span>

<span data-ttu-id="cc056-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="cc056-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cc056-131">例</span><span class="sxs-lookup"><span data-stu-id="cc056-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="cc056-132">要求</span><span class="sxs-lookup"><span data-stu-id="cc056-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->

```http
GET https://graph.microsoft.com/beta/contacts/{id}/manager
```

#### <a name="response"></a><span data-ttu-id="cc056-133">応答</span><span class="sxs-lookup"><span data-stu-id="cc056-133">Response</span></span>

<span data-ttu-id="cc056-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="cc056-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 455

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
    "@odata.type": "#microsoft.graph.user",
    "id": "24fcbca3-c3e2-48bf-9ffc-c7f81b81483d",
    "businessPhones": [
        "+1 205 555 0108"
    ],
    "displayName": "Diego Siciliani",
    "givenName": "Diego",
    "jobTitle": "CVP Finance",
    "mail": "DiegoS@contoso.com",
    "mobilePhone": null,
    "officeLocation": "14/1108",
    "preferredLanguage": "en-US",
    "surname": "Siciliani",
    "userPrincipalName": "DiegoS@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get manager",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-get-manager.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
