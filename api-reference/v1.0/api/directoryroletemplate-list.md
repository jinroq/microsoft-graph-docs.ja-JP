---
title: directoryRoleTemplates を一覧表示する
description: directoryRoleTemplate オブジェクトのリストを取得します。
author: lleonard-msft
ms.openlocfilehash: 0e43bdb3217827c8369ebe226a9aacea54996be2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301527"
---
# <a name="list-directoryroletemplates"></a><span data-ttu-id="e8a21-103">directoryRoleTemplates を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e8a21-103">List directoryRoleTemplates</span></span>

<span data-ttu-id="e8a21-104">directoryRoleTemplate オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="e8a21-104">Retrieve a list of directoryRoleTemplate objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8a21-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e8a21-105">Permissions</span></span>
<span data-ttu-id="e8a21-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e8a21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e8a21-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e8a21-108">Permission type</span></span>      | <span data-ttu-id="e8a21-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e8a21-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8a21-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e8a21-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e8a21-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e8a21-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e8a21-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e8a21-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8a21-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8a21-113">Not supported.</span></span>    |
|<span data-ttu-id="e8a21-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e8a21-114">Application</span></span> | <span data-ttu-id="e8a21-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8a21-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8a21-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e8a21-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e8a21-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e8a21-117">Optional query parameters</span></span>
<span data-ttu-id="e8a21-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポート**していません** (例: $filter はここではサポートされていません)。</span><span class="sxs-lookup"><span data-stu-id="e8a21-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8a21-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e8a21-119">Request headers</span></span>
| <span data-ttu-id="e8a21-120">名前</span><span class="sxs-lookup"><span data-stu-id="e8a21-120">Name</span></span>       | <span data-ttu-id="e8a21-121">種類</span><span class="sxs-lookup"><span data-stu-id="e8a21-121">Type</span></span> | <span data-ttu-id="e8a21-122">説明</span><span class="sxs-lookup"><span data-stu-id="e8a21-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e8a21-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8a21-123">Authorization</span></span>  | <span data-ttu-id="e8a21-124">string</span><span class="sxs-lookup"><span data-stu-id="e8a21-124">string</span></span>  | <span data-ttu-id="e8a21-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e8a21-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8a21-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e8a21-127">Request body</span></span>
<span data-ttu-id="e8a21-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e8a21-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8a21-129">応答</span><span class="sxs-lookup"><span data-stu-id="e8a21-129">Response</span></span>

<span data-ttu-id="e8a21-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryRoleTemplate](../resources/directoryroletemplate.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e8a21-130">If successful, this method returns a `200 OK` response code and collection of [directoryRoleTemplate](../resources/directoryroletemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e8a21-131">例</span><span class="sxs-lookup"><span data-stu-id="e8a21-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8a21-132">要求</span><span class="sxs-lookup"><span data-stu-id="e8a21-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplates"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoleTemplates
```
##### <a name="response"></a><span data-ttu-id="e8a21-133">応答</span><span class="sxs-lookup"><span data-stu-id="e8a21-133">Response</span></span>
<span data-ttu-id="e8a21-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e8a21-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
