---
title: privilegedRoleSettings を取得する
description: 特定の役割の役割設定を取得します。 privilegedRoleSettings オブジェクトが返されます。
localization_priority: Normal
ms.openlocfilehash: f3287939d14b54dfc3218802ae48049db8512cd1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337192"
---
# <a name="get-privilegedrolesettings"></a><span data-ttu-id="ee507-104">privilegedRoleSettings を取得する</span><span class="sxs-lookup"><span data-stu-id="ee507-104">Get privilegedRoleSettings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee507-105">特定の役割の役割設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="ee507-105">Retrieve the role settings for the given role.</span></span> <span data-ttu-id="ee507-106">[privilegedRoleSettings](../resources/privilegedrolesettings.md)オブジェクトが返されます。</span><span class="sxs-lookup"><span data-stu-id="ee507-106">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="ee507-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ee507-107">Permissions</span></span>

<span data-ttu-id="ee507-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee507-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ee507-110">リクエスターは、_特権の役割管理者_、_全体管理_者、_セキュリティ管理者_、または_セキュリティ閲覧_者のいずれかの役割を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ee507-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="ee507-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ee507-111">Permission type</span></span>      | <span data-ttu-id="ee507-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ee507-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee507-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ee507-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ee507-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ee507-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ee507-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ee507-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee507-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee507-116">Not supported.</span></span>    |
|<span data-ttu-id="ee507-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ee507-117">Application</span></span> | <span data-ttu-id="ee507-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee507-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee507-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ee507-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ee507-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ee507-120">Optional query parameters</span></span>
<span data-ttu-id="ee507-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ee507-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee507-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee507-122">Request headers</span></span>
| <span data-ttu-id="ee507-123">名前</span><span class="sxs-lookup"><span data-stu-id="ee507-123">Name</span></span>      |<span data-ttu-id="ee507-124">説明</span><span class="sxs-lookup"><span data-stu-id="ee507-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ee507-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee507-125">Authorization</span></span>  | <span data-ttu-id="ee507-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ee507-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee507-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="ee507-128">Request body</span></span>
<span data-ttu-id="ee507-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ee507-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee507-130">応答</span><span class="sxs-lookup"><span data-stu-id="ee507-130">Response</span></span>

<span data-ttu-id="ee507-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[privilegedRoleSettings](../resources/privilegedrolesettings.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ee507-131">If successful, this method returns a `200 OK` response code and [privilegedRoleSettings](../resources/privilegedrolesettings.md) object in the response body.</span></span>

<span data-ttu-id="ee507-132">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="ee507-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="ee507-133">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="ee507-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="ee507-134">例</span><span class="sxs-lookup"><span data-stu-id="ee507-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ee507-135">要求</span><span class="sxs-lookup"><span data-stu-id="ee507-135">Request</span></span>
<span data-ttu-id="ee507-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ee507-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesettings"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
```
##### <a name="response"></a><span data-ttu-id="ee507-137">応答</span><span class="sxs-lookup"><span data-stu-id="ee507-137">Response</span></span>
<span data-ttu-id="ee507-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ee507-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
