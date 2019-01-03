---
title: ディレクトリの役割] ボックスの一覧 scopedMembers
description: ディレクトリの役割の scopedRoleMembership オブジェクトのリストを取得します。
author: lleonard-msft
ms.openlocfilehash: b3d0e8bc67b6ab670b7dc8a149bad0f031b03762
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311719"
---
# <a name="list-scopedmembers-for-a-directory-role"></a><span data-ttu-id="88b2c-103">ディレクトリの役割] ボックスの一覧 scopedMembers</span><span class="sxs-lookup"><span data-stu-id="88b2c-103">List scopedMembers for a directory role</span></span>

> <span data-ttu-id="88b2c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="88b2c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="88b2c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="88b2c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="88b2c-106">ディレクトリの役割の[scopedRoleMembership](../resources/scopedrolemembership.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="88b2c-106">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) objects for a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="88b2c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="88b2c-107">Permissions</span></span>
<span data-ttu-id="88b2c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="88b2c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88b2c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="88b2c-110">Permission type</span></span>      | <span data-ttu-id="88b2c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="88b2c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88b2c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="88b2c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="88b2c-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="88b2c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="88b2c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="88b2c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88b2c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="88b2c-115">Not supported.</span></span>    |
|<span data-ttu-id="88b2c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="88b2c-116">Application</span></span> | <span data-ttu-id="88b2c-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88b2c-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="88b2c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="88b2c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryroles/{id}/scopedMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="88b2c-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="88b2c-119">Optional query parameters</span></span>
<span data-ttu-id="88b2c-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="88b2c-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="88b2c-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="88b2c-121">Request headers</span></span>
| <span data-ttu-id="88b2c-122">名前</span><span class="sxs-lookup"><span data-stu-id="88b2c-122">Name</span></span>      |<span data-ttu-id="88b2c-123">説明</span><span class="sxs-lookup"><span data-stu-id="88b2c-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="88b2c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="88b2c-124">Authorization</span></span>  | <span data-ttu-id="88b2c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="88b2c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="88b2c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="88b2c-127">Request body</span></span>
<span data-ttu-id="88b2c-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="88b2c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88b2c-129">応答</span><span class="sxs-lookup"><span data-stu-id="88b2c-129">Response</span></span>

<span data-ttu-id="88b2c-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[scopedRoleMembership](../resources/scopedrolemembership.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="88b2c-130">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="88b2c-131">例</span><span class="sxs-lookup"><span data-stu-id="88b2c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88b2c-132">要求</span><span class="sxs-lookup"><span data-stu-id="88b2c-132">Request</span></span>
<span data-ttu-id="88b2c-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="88b2c-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_scopedmembers_directoryrole"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/{id}/scopedMembers
```
##### <a name="response"></a><span data-ttu-id="88b2c-134">応答</span><span class="sxs-lookup"><span data-stu-id="88b2c-134">Response</span></span>
<span data-ttu-id="88b2c-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="88b2c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedrolemembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "value": [
    {
      "id": "id-value",
      "roleId": "roleId-value",
      "administrativeUnitId": "administrativeUnitId-value",
      "roleMemberInfo": {
        "id": "id-value",
        "displayName": "displayName-value",
        "userPrincipalName": "userPrincipalName-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List scopedmembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->