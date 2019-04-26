---
title: directoryRoleTemplates を一覧表示する
description: directoryRoleTemplate オブジェクトのリストを取得します
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0e52cb3a32c54833395722f0368d01cb49965402
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562532"
---
# <a name="list-directoryroletemplates"></a><span data-ttu-id="674e7-103">directoryRoleTemplates を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="674e7-103">List directoryRoleTemplates</span></span>

<span data-ttu-id="674e7-104">directoryRoleTemplate オブジェクトのリストを取得します</span><span class="sxs-lookup"><span data-stu-id="674e7-104">Retrieve a list of directoryRoleTemplate objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="674e7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="674e7-105">Permissions</span></span>
<span data-ttu-id="674e7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="674e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="674e7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="674e7-108">Permission type</span></span>      | <span data-ttu-id="674e7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="674e7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="674e7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="674e7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="674e7-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="674e7-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="674e7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="674e7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="674e7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="674e7-113">Not supported.</span></span>    |
|<span data-ttu-id="674e7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="674e7-114">Application</span></span> | <span data-ttu-id="674e7-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="674e7-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="674e7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="674e7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="674e7-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="674e7-117">Optional query parameters</span></span>
<span data-ttu-id="674e7-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポート**していません** (例: $filter はここではサポートされていません)。</span><span class="sxs-lookup"><span data-stu-id="674e7-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="674e7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="674e7-119">Request headers</span></span>
| <span data-ttu-id="674e7-120">名前</span><span class="sxs-lookup"><span data-stu-id="674e7-120">Name</span></span>       | <span data-ttu-id="674e7-121">型</span><span class="sxs-lookup"><span data-stu-id="674e7-121">Type</span></span> | <span data-ttu-id="674e7-122">説明</span><span class="sxs-lookup"><span data-stu-id="674e7-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="674e7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="674e7-123">Authorization</span></span>  | <span data-ttu-id="674e7-124">string</span><span class="sxs-lookup"><span data-stu-id="674e7-124">string</span></span>  | <span data-ttu-id="674e7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="674e7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="674e7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="674e7-127">Request body</span></span>
<span data-ttu-id="674e7-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="674e7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="674e7-129">応答</span><span class="sxs-lookup"><span data-stu-id="674e7-129">Response</span></span>

<span data-ttu-id="674e7-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryRoleTemplate](../resources/directoryroletemplate.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="674e7-130">If successful, this method returns a `200 OK` response code and collection of [directoryRoleTemplate](../resources/directoryroletemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="674e7-131">例</span><span class="sxs-lookup"><span data-stu-id="674e7-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="674e7-132">要求</span><span class="sxs-lookup"><span data-stu-id="674e7-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplates"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoleTemplates
```
##### <a name="response"></a><span data-ttu-id="674e7-133">応答</span><span class="sxs-lookup"><span data-stu-id="674e7-133">Response</span></span>
<span data-ttu-id="674e7-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="674e7-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "description": "description-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryRoleTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
