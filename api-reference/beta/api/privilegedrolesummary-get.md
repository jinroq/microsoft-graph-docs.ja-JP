---
title: PrivilegedRoleSummary を取得します。
description: プロパティと privilegedRoleSummary オブジェクトの関係を取得します。
localization_priority: Normal
ms.openlocfilehash: 3778ddcc297607b062354dcdf44727a0f57375dc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508231"
---
# <a name="get-privilegedrolesummary"></a><span data-ttu-id="22109-103">PrivilegedRoleSummary を取得します。</span><span class="sxs-lookup"><span data-stu-id="22109-103">Get privilegedRoleSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22109-104">プロパティと[privilegedRoleSummary](../resources/privilegedrolesummary.md)オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="22109-104">Retrieve the properties and relationships of [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="22109-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="22109-105">Permissions</span></span>
<span data-ttu-id="22109-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="22109-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="22109-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="22109-108">Permission type</span></span>      | <span data-ttu-id="22109-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="22109-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22109-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="22109-110">Delegated (work or school account)</span></span> | <span data-ttu-id="22109-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="22109-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="22109-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="22109-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22109-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22109-113">Not supported.</span></span>    |
|<span data-ttu-id="22109-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="22109-114">Application</span></span> | <span data-ttu-id="22109-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22109-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="22109-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="22109-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}?$expand=summary
```
## <a name="optional-query-parameters"></a><span data-ttu-id="22109-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="22109-117">Optional query parameters</span></span>
<span data-ttu-id="22109-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="22109-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22109-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22109-119">Request headers</span></span>
| <span data-ttu-id="22109-120">名前</span><span class="sxs-lookup"><span data-stu-id="22109-120">Name</span></span>      |<span data-ttu-id="22109-121">説明</span><span class="sxs-lookup"><span data-stu-id="22109-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="22109-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="22109-122">Authorization</span></span>  | <span data-ttu-id="22109-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="22109-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22109-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="22109-125">Request body</span></span>
<span data-ttu-id="22109-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="22109-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22109-127">応答</span><span class="sxs-lookup"><span data-stu-id="22109-127">Response</span></span>

<span data-ttu-id="22109-128">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[privilegedRoleSummary](../resources/privilegedrolesummary.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="22109-128">If successful, this method returns a `200 OK` response code and [privilegedRoleSummary](../resources/privilegedrolesummary.md) object in the response body.</span></span>

<span data-ttu-id="22109-129">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="22109-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="22109-130">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="22109-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="22109-131">例</span><span class="sxs-lookup"><span data-stu-id="22109-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="22109-132">要求</span><span class="sxs-lookup"><span data-stu-id="22109-132">Request</span></span>
<span data-ttu-id="22109-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="22109-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesummary"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/summary
```
##### <a name="response"></a><span data-ttu-id="22109-134">応答</span><span class="sxs-lookup"><span data-stu-id="22109-134">Response</span></span>
<span data-ttu-id="22109-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="22109-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleSummary"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 137

{
  "id": "id-value",
  "status": "status-value",
  "usersCount": 99,
  "managedCount": 99,
  "elevatedCount": 99,
  "mfaEnabled": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRoleSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrolesummary-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
