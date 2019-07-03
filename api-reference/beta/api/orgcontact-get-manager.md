---
title: 'orgContact: 上司の取得'
description: 連絡先の上司を取得する
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1f23a8e3f58bc4bbdc6404c7b0602c594865b9fd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445402"
---
# <a name="orgcontact-get-manager"></a><span data-ttu-id="b899a-103">orgContact: 上司の取得</span><span class="sxs-lookup"><span data-stu-id="b899a-103">orgContact: Get manager</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b899a-104">連絡先の上司を取得する</span><span class="sxs-lookup"><span data-stu-id="b899a-104">Get the contact's manager</span></span>

## <a name="permissions"></a><span data-ttu-id="b899a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b899a-105">Permissions</span></span>
<span data-ttu-id="b899a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b899a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b899a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b899a-108">Permission type</span></span>      | <span data-ttu-id="b899a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b899a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b899a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b899a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b899a-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b899a-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b899a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b899a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b899a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b899a-113">Not supported.</span></span>    |
|<span data-ttu-id="b899a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b899a-114">Application</span></span> | <span data-ttu-id="b899a-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b899a-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b899a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b899a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /contacts/{id}/manager
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b899a-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b899a-117">Optional query parameters</span></span>
<span data-ttu-id="b899a-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b899a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b899a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b899a-119">Request headers</span></span>
| <span data-ttu-id="b899a-120">名前</span><span class="sxs-lookup"><span data-stu-id="b899a-120">Name</span></span>       | <span data-ttu-id="b899a-121">型</span><span class="sxs-lookup"><span data-stu-id="b899a-121">Type</span></span> | <span data-ttu-id="b899a-122">説明</span><span class="sxs-lookup"><span data-stu-id="b899a-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b899a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b899a-123">Authorization</span></span>  | <span data-ttu-id="b899a-124">string</span><span class="sxs-lookup"><span data-stu-id="b899a-124">string</span></span>  | <span data-ttu-id="b899a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b899a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b899a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b899a-127">Request body</span></span>
<span data-ttu-id="b899a-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b899a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b899a-129">応答</span><span class="sxs-lookup"><span data-stu-id="b899a-129">Response</span></span>

<span data-ttu-id="b899a-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b899a-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b899a-131">例</span><span class="sxs-lookup"><span data-stu-id="b899a-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b899a-132">要求</span><span class="sxs-lookup"><span data-stu-id="b899a-132">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b899a-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b899a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->

```http
GET https://graph.microsoft.com/beta/contacts/{id}/manager
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b899a-134">C#</span><span class="sxs-lookup"><span data-stu-id="b899a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-manager-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b899a-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="b899a-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-manager-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b899a-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="b899a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-manager-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b899a-137">応答</span><span class="sxs-lookup"><span data-stu-id="b899a-137">Response</span></span>

<span data-ttu-id="b899a-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b899a-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
