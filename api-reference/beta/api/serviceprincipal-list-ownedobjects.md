---
title: 'servicePrincipals: ownedObjects を一覧表示'
description: ServicePrincipal が所有するオブジェクトの一覧を取得します。  これには、アプリケーションまたはグループが含まれます。
ms.openlocfilehash: 79ca70c5c86e535a7d8a11598509e7ebf61780a0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072689"
---
# <a name="serviceprincipals-list-ownedobjects"></a><span data-ttu-id="f238d-104">servicePrincipals: ownedObjects を一覧表示</span><span class="sxs-lookup"><span data-stu-id="f238d-104">servicePrincipals: List ownedObjects</span></span>

> <span data-ttu-id="f238d-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f238d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f238d-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f238d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f238d-107">ServicePrincipal が所有するオブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="f238d-107">Retrieve a list of objects owned by the servicePrincipal.</span></span>  <span data-ttu-id="f238d-108">これには、アプリケーションまたはグループが含まれます。</span><span class="sxs-lookup"><span data-stu-id="f238d-108">This could include applications or groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="f238d-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f238d-109">Permissions</span></span>
<span data-ttu-id="f238d-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f238d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f238d-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f238d-112">Permission type</span></span>      | <span data-ttu-id="f238d-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f238d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f238d-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f238d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f238d-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f238d-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f238d-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f238d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f238d-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f238d-117">Not supported.</span></span>    |
|<span data-ttu-id="f238d-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f238d-118">Application</span></span> | <span data-ttu-id="f238d-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f238d-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f238d-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f238d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f238d-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f238d-121">Optional query parameters</span></span>
<span data-ttu-id="f238d-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f238d-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f238d-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f238d-123">Request headers</span></span>
| <span data-ttu-id="f238d-124">名前</span><span class="sxs-lookup"><span data-stu-id="f238d-124">Name</span></span>       | <span data-ttu-id="f238d-125">型</span><span class="sxs-lookup"><span data-stu-id="f238d-125">Type</span></span> | <span data-ttu-id="f238d-126">説明</span><span class="sxs-lookup"><span data-stu-id="f238d-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f238d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f238d-127">Authorization</span></span>  | <span data-ttu-id="f238d-128">string</span><span class="sxs-lookup"><span data-stu-id="f238d-128">string</span></span>  | <span data-ttu-id="f238d-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f238d-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f238d-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="f238d-131">Request body</span></span>
<span data-ttu-id="f238d-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f238d-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f238d-133">応答</span><span class="sxs-lookup"><span data-stu-id="f238d-133">Response</span></span>

<span data-ttu-id="f238d-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f238d-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f238d-135">例</span><span class="sxs-lookup"><span data-stu-id="f238d-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f238d-136">要求</span><span class="sxs-lookup"><span data-stu-id="f238d-136">Request</span></span>
<span data-ttu-id="f238d-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f238d-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/ownedObjects
```
##### <a name="response"></a><span data-ttu-id="f238d-138">応答</span><span class="sxs-lookup"><span data-stu-id="f238d-138">Response</span></span>
<span data-ttu-id="f238d-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f238d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List ownedObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->