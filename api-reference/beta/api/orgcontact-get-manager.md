---
title: 'orgContact: Get のマネージャー'
description: 連絡先のマネージャーを取得します。
localization_priority: Normal
ms.openlocfilehash: 18839c2184bb92dae1e23f125885541408696c98
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826545"
---
# <a name="orgcontact-get-manager"></a><span data-ttu-id="84e02-103">orgContact: Get のマネージャー</span><span class="sxs-lookup"><span data-stu-id="84e02-103">orgContact: Get manager</span></span>

> <span data-ttu-id="84e02-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="84e02-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84e02-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84e02-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="84e02-106">連絡先のマネージャーを取得します。</span><span class="sxs-lookup"><span data-stu-id="84e02-106">Get the contact's manager</span></span>

## <a name="permissions"></a><span data-ttu-id="84e02-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="84e02-107">Permissions</span></span>
<span data-ttu-id="84e02-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="84e02-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84e02-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="84e02-110">Permission type</span></span>      | <span data-ttu-id="84e02-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="84e02-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84e02-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="84e02-112">Delegated (work or school account)</span></span> | <span data-ttu-id="84e02-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="84e02-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="84e02-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="84e02-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84e02-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84e02-115">Not supported.</span></span>    |
|<span data-ttu-id="84e02-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="84e02-116">Application</span></span> | <span data-ttu-id="84e02-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84e02-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="84e02-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="84e02-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /contacts/{id}/manager
```

## <a name="optional-query-parameters"></a><span data-ttu-id="84e02-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="84e02-119">Optional query parameters</span></span>
<span data-ttu-id="84e02-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="84e02-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84e02-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="84e02-121">Request headers</span></span>
| <span data-ttu-id="84e02-122">名前</span><span class="sxs-lookup"><span data-stu-id="84e02-122">Name</span></span>       | <span data-ttu-id="84e02-123">種類</span><span class="sxs-lookup"><span data-stu-id="84e02-123">Type</span></span> | <span data-ttu-id="84e02-124">説明</span><span class="sxs-lookup"><span data-stu-id="84e02-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="84e02-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="84e02-125">Authorization</span></span>  | <span data-ttu-id="84e02-126">string</span><span class="sxs-lookup"><span data-stu-id="84e02-126">string</span></span>  | <span data-ttu-id="84e02-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="84e02-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="84e02-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="84e02-129">Request body</span></span>
<span data-ttu-id="84e02-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="84e02-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84e02-131">応答</span><span class="sxs-lookup"><span data-stu-id="84e02-131">Response</span></span>

<span data-ttu-id="84e02-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="84e02-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="84e02-133">例</span><span class="sxs-lookup"><span data-stu-id="84e02-133">Example</span></span>

#### <a name="request"></a><span data-ttu-id="84e02-134">要求</span><span class="sxs-lookup"><span data-stu-id="84e02-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->

```http
GET https://graph.microsoft.com/beta/contacts/{id}/manager
```

#### <a name="response"></a><span data-ttu-id="84e02-135">応答</span><span class="sxs-lookup"><span data-stu-id="84e02-135">Response</span></span>

<span data-ttu-id="84e02-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="84e02-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get manager",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
