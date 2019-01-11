---
title: PrivilegedRoleSettings を取得します。
description: 指定したロールのロールの設定を取得します。 PrivilegedRoleSettings オブジェクトが返されます。
localization_priority: Normal
ms.openlocfilehash: a80c4027ace009292e7a57b8104e94e114175f1d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879815"
---
# <a name="get-privilegedrolesettings"></a><span data-ttu-id="4ba68-104">PrivilegedRoleSettings を取得します。</span><span class="sxs-lookup"><span data-stu-id="4ba68-104">Get privilegedRoleSettings</span></span>

> <span data-ttu-id="4ba68-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4ba68-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ba68-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ba68-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4ba68-107">指定したロールのロールの設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="4ba68-107">Retrieve the role settings for the given role.</span></span> <span data-ttu-id="4ba68-108">[PrivilegedRoleSettings](../resources/privilegedrolesettings.md)オブジェクトが返されます。</span><span class="sxs-lookup"><span data-stu-id="4ba68-108">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="4ba68-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4ba68-109">Permissions</span></span>

<span data-ttu-id="4ba68-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4ba68-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4ba68-112">リクエスターは、次のロールのいずれかを持つ必要があります:_ロールの権限を持つ管理者_、_グローバル管理者_、_セキュリティ管理者_、または_セキュリティのリーダー_です。</span><span class="sxs-lookup"><span data-stu-id="4ba68-112">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="4ba68-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4ba68-113">Permission type</span></span>      | <span data-ttu-id="4ba68-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4ba68-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ba68-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4ba68-115">Delegated (work or school account)</span></span> | <span data-ttu-id="4ba68-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4ba68-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4ba68-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4ba68-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ba68-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ba68-118">Not supported.</span></span>    |
|<span data-ttu-id="4ba68-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4ba68-119">Application</span></span> | <span data-ttu-id="4ba68-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ba68-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ba68-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4ba68-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4ba68-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4ba68-122">Optional query parameters</span></span>
<span data-ttu-id="4ba68-123">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4ba68-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ba68-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4ba68-124">Request headers</span></span>
| <span data-ttu-id="4ba68-125">名前</span><span class="sxs-lookup"><span data-stu-id="4ba68-125">Name</span></span>      |<span data-ttu-id="4ba68-126">説明</span><span class="sxs-lookup"><span data-stu-id="4ba68-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4ba68-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ba68-127">Authorization</span></span>  | <span data-ttu-id="4ba68-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4ba68-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ba68-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="4ba68-130">Request body</span></span>
<span data-ttu-id="4ba68-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4ba68-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ba68-132">応答</span><span class="sxs-lookup"><span data-stu-id="4ba68-132">Response</span></span>

<span data-ttu-id="4ba68-133">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[privilegedRoleSettings](../resources/privilegedrolesettings.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="4ba68-133">If successful, this method returns a `200 OK` response code and [privilegedRoleSettings](../resources/privilegedrolesettings.md) object in the response body.</span></span>

<span data-ttu-id="4ba68-134">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="4ba68-134">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="4ba68-135">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="4ba68-135">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="4ba68-136">例</span><span class="sxs-lookup"><span data-stu-id="4ba68-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ba68-137">要求</span><span class="sxs-lookup"><span data-stu-id="4ba68-137">Request</span></span>
<span data-ttu-id="4ba68-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4ba68-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesettings"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
```
##### <a name="response"></a><span data-ttu-id="4ba68-139">応答</span><span class="sxs-lookup"><span data-stu-id="4ba68-139">Response</span></span>
<span data-ttu-id="4ba68-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4ba68-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
