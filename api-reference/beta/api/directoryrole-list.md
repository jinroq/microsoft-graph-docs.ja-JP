---
title: directoryRoles を一覧表示する
description: テナントでアクティブになっているディレクトリ ロールを一覧表示します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b50af15f6bce8bb6d6fdb4072df71edbf19a9cf7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956158"
---
# <a name="list-directoryroles"></a><span data-ttu-id="a3936-103">directoryRoles を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a3936-103">List directoryRoles</span></span>

> <span data-ttu-id="a3936-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a3936-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3936-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3936-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a3936-106">テナントでアクティブになっているディレクトリ ロールを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="a3936-106">List the directory roles that are activated in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="a3936-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a3936-107">Permissions</span></span>
<span data-ttu-id="a3936-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a3936-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3936-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a3936-110">Permission type</span></span>      | <span data-ttu-id="a3936-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a3936-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3936-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a3936-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a3936-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a3936-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a3936-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a3936-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3936-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3936-115">Not supported.</span></span>    |
|<span data-ttu-id="a3936-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a3936-116">Application</span></span> | <span data-ttu-id="a3936-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3936-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3936-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a3936-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a3936-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a3936-119">Optional query parameters</span></span>
<span data-ttu-id="a3936-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポート**していません** (例: $filter はここではサポートされていません)。</span><span class="sxs-lookup"><span data-stu-id="a3936-120">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3936-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3936-121">Request headers</span></span>
| <span data-ttu-id="a3936-122">名前</span><span class="sxs-lookup"><span data-stu-id="a3936-122">Name</span></span>       | <span data-ttu-id="a3936-123">型</span><span class="sxs-lookup"><span data-stu-id="a3936-123">Type</span></span> | <span data-ttu-id="a3936-124">説明</span><span class="sxs-lookup"><span data-stu-id="a3936-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a3936-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3936-125">Authorization</span></span>  | <span data-ttu-id="a3936-126">string</span><span class="sxs-lookup"><span data-stu-id="a3936-126">string</span></span>  | <span data-ttu-id="a3936-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a3936-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3936-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="a3936-129">Request body</span></span>
<span data-ttu-id="a3936-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a3936-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3936-131">応答</span><span class="sxs-lookup"><span data-stu-id="a3936-131">Response</span></span>

<span data-ttu-id="a3936-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryRole](../resources/directoryrole.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a3936-132">If successful, this method returns a `200 OK` response code and collection of [directoryRole](../resources/directoryrole.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a3936-133">例</span><span class="sxs-lookup"><span data-stu-id="a3936-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a3936-134">要求</span><span class="sxs-lookup"><span data-stu-id="a3936-134">Request</span></span>
<span data-ttu-id="a3936-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a3936-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directoryroles"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles
```
##### <a name="response"></a><span data-ttu-id="a3936-136">応答</span><span class="sxs-lookup"><span data-stu-id="a3936-136">Response</span></span>
<span data-ttu-id="a3936-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a3936-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 187

{
  "value": [
    {
      "description": "description-value",
      "displayName": "displayName-value",
      "roleTemplateId": "roleTemplateId-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
