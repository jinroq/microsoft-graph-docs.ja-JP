---
title: PrivilegedRoleSettings を取得します。
description: 指定したロールのロールの設定を取得します。 PrivilegedRoleSettings オブジェクトが返されます。
localization_priority: Normal
ms.openlocfilehash: 7ecebad77acf2e090263878aacc29f00a9215fc7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508105"
---
# <a name="get-privilegedrolesettings"></a><span data-ttu-id="f74a6-104">PrivilegedRoleSettings を取得します。</span><span class="sxs-lookup"><span data-stu-id="f74a6-104">Get privilegedRoleSettings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f74a6-105">指定したロールのロールの設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="f74a6-105">Retrieve the role settings for the given role.</span></span> <span data-ttu-id="f74a6-106">[PrivilegedRoleSettings](../resources/privilegedrolesettings.md)オブジェクトが返されます。</span><span class="sxs-lookup"><span data-stu-id="f74a6-106">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="f74a6-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f74a6-107">Permissions</span></span>

<span data-ttu-id="f74a6-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f74a6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f74a6-110">リクエスターは、次のロールのいずれかを持つ必要があります:_ロールの権限を持つ管理者_、_グローバル管理者_、_セキュリティ管理者_、または_セキュリティのリーダー_です。</span><span class="sxs-lookup"><span data-stu-id="f74a6-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="f74a6-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f74a6-111">Permission type</span></span>      | <span data-ttu-id="f74a6-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f74a6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f74a6-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f74a6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f74a6-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f74a6-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f74a6-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f74a6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f74a6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f74a6-116">Not supported.</span></span>    |
|<span data-ttu-id="f74a6-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f74a6-117">Application</span></span> | <span data-ttu-id="f74a6-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f74a6-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f74a6-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f74a6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f74a6-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f74a6-120">Optional query parameters</span></span>
<span data-ttu-id="f74a6-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f74a6-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f74a6-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f74a6-122">Request headers</span></span>
| <span data-ttu-id="f74a6-123">名前</span><span class="sxs-lookup"><span data-stu-id="f74a6-123">Name</span></span>      |<span data-ttu-id="f74a6-124">説明</span><span class="sxs-lookup"><span data-stu-id="f74a6-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f74a6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f74a6-125">Authorization</span></span>  | <span data-ttu-id="f74a6-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f74a6-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f74a6-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="f74a6-128">Request body</span></span>
<span data-ttu-id="f74a6-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f74a6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f74a6-130">応答</span><span class="sxs-lookup"><span data-stu-id="f74a6-130">Response</span></span>

<span data-ttu-id="f74a6-131">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[privilegedRoleSettings](../resources/privilegedrolesettings.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f74a6-131">If successful, this method returns a `200 OK` response code and [privilegedRoleSettings](../resources/privilegedrolesettings.md) object in the response body.</span></span>

<span data-ttu-id="f74a6-132">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="f74a6-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="f74a6-133">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="f74a6-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="f74a6-134">例</span><span class="sxs-lookup"><span data-stu-id="f74a6-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f74a6-135">要求</span><span class="sxs-lookup"><span data-stu-id="f74a6-135">Request</span></span>
<span data-ttu-id="f74a6-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f74a6-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesettings"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
```
##### <a name="response"></a><span data-ttu-id="f74a6-137">応答</span><span class="sxs-lookup"><span data-stu-id="f74a6-137">Response</span></span>
<span data-ttu-id="f74a6-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f74a6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/privilegedrolesettings-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
