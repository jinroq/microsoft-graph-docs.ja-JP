---
title: PrivilegedRoleAssignment を取得します。
description: プロパティと privilegedRoleAssignment オブジェクトの関係を取得します。
localization_priority: Normal
ms.openlocfilehash: 220001f523971adadd80a406b54f16d22f2ef48e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520320"
---
# <a name="get-privilegedroleassignment"></a><span data-ttu-id="4eaba-103">PrivilegedRoleAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="4eaba-103">Get privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4eaba-104">プロパティと privilegedRoleAssignment オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="4eaba-104">Retrieve the properties and relationships of privilegedRoleAssignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4eaba-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4eaba-105">Permissions</span></span>
<span data-ttu-id="4eaba-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4eaba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4eaba-108">リクエスターは、次のロールのいずれかを持つ必要があります:_ロールの権限を持つ管理者_、_グローバル管理者_、_セキュリティ管理者_、または_セキュリティのリーダー_です。</span><span class="sxs-lookup"><span data-stu-id="4eaba-108">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="4eaba-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4eaba-109">Permission type</span></span>      | <span data-ttu-id="4eaba-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4eaba-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4eaba-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4eaba-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4eaba-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4eaba-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4eaba-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4eaba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4eaba-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4eaba-114">Not supported.</span></span>    |
|<span data-ttu-id="4eaba-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4eaba-115">Application</span></span> | <span data-ttu-id="4eaba-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4eaba-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4eaba-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4eaba-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4eaba-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4eaba-118">Optional query parameters</span></span>
<span data-ttu-id="4eaba-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4eaba-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4eaba-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4eaba-120">Request headers</span></span>
| <span data-ttu-id="4eaba-121">名前</span><span class="sxs-lookup"><span data-stu-id="4eaba-121">Name</span></span>      |<span data-ttu-id="4eaba-122">説明</span><span class="sxs-lookup"><span data-stu-id="4eaba-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4eaba-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4eaba-123">Authorization</span></span>  | <span data-ttu-id="4eaba-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4eaba-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4eaba-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4eaba-126">Request body</span></span>
<span data-ttu-id="4eaba-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4eaba-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4eaba-128">応答</span><span class="sxs-lookup"><span data-stu-id="4eaba-128">Response</span></span>

<span data-ttu-id="4eaba-129">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[privilegedRoleAssignment](../resources/privilegedroleassignment.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="4eaba-129">If successful, this method returns a `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="4eaba-130">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="4eaba-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="4eaba-131">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="4eaba-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="4eaba-132">例</span><span class="sxs-lookup"><span data-stu-id="4eaba-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4eaba-133">要求</span><span class="sxs-lookup"><span data-stu-id="4eaba-133">Request</span></span>
<span data-ttu-id="4eaba-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4eaba-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignment"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="4eaba-135">応答</span><span class="sxs-lookup"><span data-stu-id="4eaba-135">Response</span></span>
<span data-ttu-id="4eaba-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4eaba-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignment-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
