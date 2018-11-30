---
title: 'orgContact: Get のマネージャー'
description: 連絡先のマネージャーを取得します。
ms.openlocfilehash: 7fe4c61422eb83bb4501fbb521f301ec6f9afaa5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067631"
---
# <a name="orgcontact-get-manager"></a><span data-ttu-id="a2caa-103">orgContact: Get のマネージャー</span><span class="sxs-lookup"><span data-stu-id="a2caa-103">orgContact: Get manager</span></span>

> <span data-ttu-id="a2caa-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a2caa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2caa-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2caa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a2caa-106">連絡先のマネージャーを取得します。</span><span class="sxs-lookup"><span data-stu-id="a2caa-106">Get the contact's manager</span></span>

## <a name="permissions"></a><span data-ttu-id="a2caa-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a2caa-107">Permissions</span></span>
<span data-ttu-id="a2caa-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2caa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2caa-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a2caa-110">Permission type</span></span>      | <span data-ttu-id="a2caa-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a2caa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2caa-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a2caa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a2caa-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a2caa-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a2caa-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a2caa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2caa-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2caa-115">Not supported.</span></span>    |
|<span data-ttu-id="a2caa-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a2caa-116">Application</span></span> | <span data-ttu-id="a2caa-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2caa-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2caa-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a2caa-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /contacts/{id}/manager
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a2caa-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a2caa-119">Optional query parameters</span></span>
<span data-ttu-id="a2caa-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a2caa-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2caa-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2caa-121">Request headers</span></span>
| <span data-ttu-id="a2caa-122">名前</span><span class="sxs-lookup"><span data-stu-id="a2caa-122">Name</span></span>       | <span data-ttu-id="a2caa-123">型</span><span class="sxs-lookup"><span data-stu-id="a2caa-123">Type</span></span> | <span data-ttu-id="a2caa-124">説明</span><span class="sxs-lookup"><span data-stu-id="a2caa-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a2caa-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2caa-125">Authorization</span></span>  | <span data-ttu-id="a2caa-126">string</span><span class="sxs-lookup"><span data-stu-id="a2caa-126">string</span></span>  | <span data-ttu-id="a2caa-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a2caa-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2caa-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="a2caa-129">Request body</span></span>
<span data-ttu-id="a2caa-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a2caa-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2caa-131">応答</span><span class="sxs-lookup"><span data-stu-id="a2caa-131">Response</span></span>

<span data-ttu-id="a2caa-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a2caa-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a2caa-133">例</span><span class="sxs-lookup"><span data-stu-id="a2caa-133">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a2caa-134">要求</span><span class="sxs-lookup"><span data-stu-id="a2caa-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->

```http
GET https://graph.microsoft.com/beta/contacts/{id}/manager
```

#### <a name="response"></a><span data-ttu-id="a2caa-135">応答</span><span class="sxs-lookup"><span data-stu-id="a2caa-135">Response</span></span>

<span data-ttu-id="a2caa-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a2caa-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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