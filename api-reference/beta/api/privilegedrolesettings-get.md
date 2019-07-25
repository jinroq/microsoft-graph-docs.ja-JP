---
title: privilegedRoleSettings を取得する
description: 特定の役割の役割設定を取得します。 PrivilegedRoleSettings オブジェクトが返されます。
localization_priority: Normal
ms.openlocfilehash: b4dbb6f378288a727f4c0c97541f9cb3e0eb8eda
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875529"
---
# <a name="get-privilegedrolesettings"></a><span data-ttu-id="86709-104">privilegedRoleSettings を取得する</span><span class="sxs-lookup"><span data-stu-id="86709-104">Get privilegedRoleSettings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86709-105">特定の役割の役割設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="86709-105">Retrieve the role settings for the given role.</span></span> <span data-ttu-id="86709-106">[PrivilegedRoleSettings](../resources/privilegedrolesettings.md)オブジェクトが返されます。</span><span class="sxs-lookup"><span data-stu-id="86709-106">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="86709-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="86709-107">Permissions</span></span>

<span data-ttu-id="86709-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="86709-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="86709-110">リクエスターは、_特権の役割管理者_、_全体管理_者、_セキュリティ管理者_、または_セキュリティ閲覧_者のいずれかの役割を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="86709-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="86709-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="86709-111">Permission type</span></span>      | <span data-ttu-id="86709-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="86709-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86709-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="86709-113">Delegated (work or school account)</span></span> | <span data-ttu-id="86709-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="86709-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="86709-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="86709-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86709-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86709-116">Not supported.</span></span>    |
|<span data-ttu-id="86709-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="86709-117">Application</span></span> | <span data-ttu-id="86709-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86709-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="86709-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="86709-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="86709-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="86709-120">Optional query parameters</span></span>
<span data-ttu-id="86709-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="86709-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="86709-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="86709-122">Request headers</span></span>
| <span data-ttu-id="86709-123">名前</span><span class="sxs-lookup"><span data-stu-id="86709-123">Name</span></span>      |<span data-ttu-id="86709-124">説明</span><span class="sxs-lookup"><span data-stu-id="86709-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="86709-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="86709-125">Authorization</span></span>  | <span data-ttu-id="86709-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="86709-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="86709-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="86709-128">Request body</span></span>
<span data-ttu-id="86709-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="86709-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86709-130">応答</span><span class="sxs-lookup"><span data-stu-id="86709-130">Response</span></span>

<span data-ttu-id="86709-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[privilegedRoleSettings](../resources/privilegedrolesettings.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="86709-131">If successful, this method returns a `200 OK` response code and [privilegedRoleSettings](../resources/privilegedrolesettings.md) object in the response body.</span></span>

<span data-ttu-id="86709-132">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="86709-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="86709-133">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="86709-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="86709-134">例</span><span class="sxs-lookup"><span data-stu-id="86709-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86709-135">要求</span><span class="sxs-lookup"><span data-stu-id="86709-135">Request</span></span>
<span data-ttu-id="86709-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="86709-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="86709-137">プロトコル</span><span class="sxs-lookup"><span data-stu-id="86709-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesettings"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="86709-138">C#</span><span class="sxs-lookup"><span data-stu-id="86709-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedrolesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="86709-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="86709-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedrolesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="86709-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="86709-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedrolesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="86709-141">Java</span><span class="sxs-lookup"><span data-stu-id="86709-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedrolesettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="86709-142">応答</span><span class="sxs-lookup"><span data-stu-id="86709-142">Response</span></span>
<span data-ttu-id="86709-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="86709-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 228

{
  "minElevationDuration": "2016-10-19T10:37:00Z",
  "maxElavationDuration": "2016-10-19T10:37:00Z",
  "elevationDuration": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "notificationToUserOnElevation": true,
  "ticketingInfoOnElevation": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
