---
title: privilegedRole を取得する
description: 'PrivilegedRole オブジェクトのプロパティとリレーションシップを取得します。 '
localization_priority: Normal
ms.openlocfilehash: 92991de263ee573ce88d4f87345a32a3ef697d23
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33594896"
---
# <a name="get-privilegedrole"></a><span data-ttu-id="4ff6b-103">privilegedRole を取得する</span><span class="sxs-lookup"><span data-stu-id="4ff6b-103">Get privilegedRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ff6b-104">[PrivilegedRole](../resources/privilegedrole.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="4ff6b-104">Retrieve the properties and relationships of [privilegedRole](../resources/privilegedrole.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="4ff6b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4ff6b-105">Permissions</span></span>
<span data-ttu-id="4ff6b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4ff6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4ff6b-108">リクエスターは、_特権の役割管理者_、_全体管理_者、_セキュリティ管理者_、または_セキュリティ閲覧_者のいずれかの役割を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4ff6b-108">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="4ff6b-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4ff6b-109">Permission type</span></span>      | <span data-ttu-id="4ff6b-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4ff6b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ff6b-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4ff6b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4ff6b-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4ff6b-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4ff6b-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4ff6b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ff6b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ff6b-114">Not supported.</span></span>    |
|<span data-ttu-id="4ff6b-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4ff6b-115">Application</span></span> | <span data-ttu-id="4ff6b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ff6b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ff6b-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4ff6b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}
GET /privilegedRoleAssignments/{id}/roleInfo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4ff6b-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4ff6b-118">Optional query parameters</span></span>
<span data-ttu-id="4ff6b-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4ff6b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ff6b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4ff6b-120">Request headers</span></span>
| <span data-ttu-id="4ff6b-121">名前</span><span class="sxs-lookup"><span data-stu-id="4ff6b-121">Name</span></span>      |<span data-ttu-id="4ff6b-122">説明</span><span class="sxs-lookup"><span data-stu-id="4ff6b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4ff6b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ff6b-123">Authorization</span></span>  | <span data-ttu-id="4ff6b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4ff6b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ff6b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4ff6b-126">Request body</span></span>
<span data-ttu-id="4ff6b-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4ff6b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ff6b-128">応答</span><span class="sxs-lookup"><span data-stu-id="4ff6b-128">Response</span></span>

<span data-ttu-id="4ff6b-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[privilegedRole](../resources/privilegedrole.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4ff6b-129">If successful, this method returns a `200 OK` response code and [privilegedRole](../resources/privilegedrole.md) object in the response body.</span></span>

<span data-ttu-id="4ff6b-130">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="4ff6b-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="4ff6b-131">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="4ff6b-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="4ff6b-132">例</span><span class="sxs-lookup"><span data-stu-id="4ff6b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ff6b-133">要求</span><span class="sxs-lookup"><span data-stu-id="4ff6b-133">Request</span></span>
<span data-ttu-id="4ff6b-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4ff6b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrole"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}
```
##### <a name="response"></a><span data-ttu-id="4ff6b-135">応答</span><span class="sxs-lookup"><span data-stu-id="4ff6b-135">Response</span></span>
<span data-ttu-id="4ff6b-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4ff6b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 46

{
  "id": "id-value",
  "name": "name-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4ff6b-139">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="4ff6b-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4ff6b-140">Visual</span><span class="sxs-lookup"><span data-stu-id="4ff6b-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_privilegedrole-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4ff6b-141">Java</span><span class="sxs-lookup"><span data-stu-id="4ff6b-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_privilegedrole-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrole-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedrole-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
