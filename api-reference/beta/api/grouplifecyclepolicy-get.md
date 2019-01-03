---
title: Get groupLifecyclePolicy
description: groupLifecyclePolicies オブジェクトのプロパティとリレーションシップを取得します。
author: dkershaw10
ms.openlocfilehash: ef239385766b33c4a03576200c6c9abf3938c25a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312524"
---
# <a name="get-grouplifecyclepolicy"></a><span data-ttu-id="8e54e-103">Get groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="8e54e-103">Get groupLifecyclePolicy</span></span>

> <span data-ttu-id="8e54e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8e54e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e54e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e54e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8e54e-106">[groupLifecyclePolicies](../resources/grouplifecyclepolicy.md) オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="8e54e-106">Retrieve the properties and relationships of a [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e54e-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8e54e-107">Permissions</span></span>

<span data-ttu-id="8e54e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8e54e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8e54e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8e54e-110">Permission type</span></span>      | <span data-ttu-id="8e54e-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8e54e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e54e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8e54e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8e54e-113">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e54e-113">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="8e54e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8e54e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e54e-115">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="8e54e-115">Not supported</span></span> |
|<span data-ttu-id="8e54e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8e54e-116">Application</span></span> | <span data-ttu-id="8e54e-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e54e-117">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e54e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8e54e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8e54e-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8e54e-119">Optional query parameters</span></span>
<span data-ttu-id="8e54e-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8e54e-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e54e-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8e54e-121">Request headers</span></span>
| <span data-ttu-id="8e54e-122">名前</span><span class="sxs-lookup"><span data-stu-id="8e54e-122">Name</span></span> | <span data-ttu-id="8e54e-123">説明</span><span class="sxs-lookup"><span data-stu-id="8e54e-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="8e54e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e54e-124">Authorization</span></span> | <span data-ttu-id="8e54e-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8e54e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e54e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8e54e-127">Request body</span></span>
<span data-ttu-id="8e54e-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8e54e-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8e54e-129">応答</span><span class="sxs-lookup"><span data-stu-id="8e54e-129">Response</span></span>
<span data-ttu-id="8e54e-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8e54e-130">If successful, this method returns a `200 OK` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8e54e-131">例</span><span class="sxs-lookup"><span data-stu-id="8e54e-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8e54e-132">要求</span><span class="sxs-lookup"><span data-stu-id="8e54e-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```http
GET https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="8e54e-133">応答</span><span class="sxs-lookup"><span data-stu-id="8e54e-133">Response</span></span>

<span data-ttu-id="8e54e-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8e54e-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 174

{
  "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->