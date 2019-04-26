---
title: oauth2PermissionGrants を一覧表示する
description: oauth2PermissionGrant オブジェクトのリストを取得します。
localization_priority: Normal
ms.openlocfilehash: 6f2a9660b740772caa46992764b905f90736c905
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333069"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="7be9a-103">oauth2PermissionGrants を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7be9a-103">List oauth2PermissionGrants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7be9a-104">oauth2PermissionGrant オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="7be9a-104">Retrieve a list of oauth2PermissionGrant objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="7be9a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7be9a-105">Permissions</span></span>

<span data-ttu-id="7be9a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7be9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7be9a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7be9a-108">Permission type</span></span>      | <span data-ttu-id="7be9a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7be9a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7be9a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7be9a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7be9a-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7be9a-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7be9a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7be9a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7be9a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7be9a-113">Not supported.</span></span>    |
|<span data-ttu-id="7be9a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7be9a-114">Application</span></span> | <span data-ttu-id="7be9a-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7be9a-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7be9a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7be9a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /oauth2PermissionGrants
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7be9a-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7be9a-117">Optional query parameters</span></span>
<span data-ttu-id="7be9a-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7be9a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7be9a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7be9a-119">Request headers</span></span>
| <span data-ttu-id="7be9a-120">名前</span><span class="sxs-lookup"><span data-stu-id="7be9a-120">Name</span></span> | <span data-ttu-id="7be9a-121">説明</span><span class="sxs-lookup"><span data-stu-id="7be9a-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="7be9a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7be9a-122">Authorization</span></span>  | <span data-ttu-id="7be9a-123">string</span><span class="sxs-lookup"><span data-stu-id="7be9a-123">string</span></span>  | <span data-ttu-id="7be9a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7be9a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7be9a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7be9a-126">Request body</span></span>
<span data-ttu-id="7be9a-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7be9a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7be9a-128">応答</span><span class="sxs-lookup"><span data-stu-id="7be9a-128">Response</span></span>

<span data-ttu-id="7be9a-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7be9a-129">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7be9a-130">例</span><span class="sxs-lookup"><span data-stu-id="7be9a-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7be9a-131">要求</span><span class="sxs-lookup"><span data-stu-id="7be9a-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_oauth2permissiongrants"
}-->
```http
GET https://graph.microsoft.com/beta/oauth2PermissionGrants
```
##### <a name="response"></a><span data-ttu-id="7be9a-132">応答</span><span class="sxs-lookup"><span data-stu-id="7be9a-132">Response</span></span>

<span data-ttu-id="7be9a-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7be9a-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 259

{
  "value": [
    {
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "expiryTime": "datetime-value",
      "id": "id-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value",
      "scope": "scope-value",
      "startTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oauth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
