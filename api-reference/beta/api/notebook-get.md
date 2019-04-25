---
title: ノートブックを取得する
description: ノートブックオブジェクトのプロパティとリレーションシップを取得します。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: af8d358a7f05ed60b48e6df6a3cc60319e009e34
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540335"
---
# <a name="get-notebook"></a><span data-ttu-id="0297b-103">ノートブックを取得する</span><span class="sxs-lookup"><span data-stu-id="0297b-103">Get notebook</span></span>

<span data-ttu-id="0297b-104">[ノートブック](../resources/notebook.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="0297b-104">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0297b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0297b-105">Permissions</span></span>
<span data-ttu-id="0297b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0297b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0297b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0297b-108">Permission type</span></span>      | <span data-ttu-id="0297b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0297b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0297b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0297b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0297b-111">メモ作成、メモ読み取り、メモ (すべて)、メモ書き込み、メモ (すべて)</span><span class="sxs-lookup"><span data-stu-id="0297b-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="0297b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0297b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0297b-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0297b-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="0297b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0297b-114">Application</span></span> | <span data-ttu-id="0297b-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0297b-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0297b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0297b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}
GET /groups/{id}/onenote/notebooks/{id}
GET /sites/{id}/onenote/notebooks/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0297b-117">省略可能なクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0297b-117">Optional query parameters</span></span>
<span data-ttu-id="0297b-118">このメソッドは、 `select`応答`expand`をカスタマイズするためのおよび[OData クエリパラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0297b-118">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="0297b-119">ノートブック`expand`の有効な値`sections`は`sectionGroups`、とです。</span><span class="sxs-lookup"><span data-stu-id="0297b-119">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0297b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0297b-120">Request headers</span></span>
| <span data-ttu-id="0297b-121">名前</span><span class="sxs-lookup"><span data-stu-id="0297b-121">Name</span></span>       | <span data-ttu-id="0297b-122">型</span><span class="sxs-lookup"><span data-stu-id="0297b-122">Type</span></span> | <span data-ttu-id="0297b-123">説明</span><span class="sxs-lookup"><span data-stu-id="0297b-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0297b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0297b-124">Authorization</span></span>  | <span data-ttu-id="0297b-125">string</span><span class="sxs-lookup"><span data-stu-id="0297b-125">string</span></span>  | <span data-ttu-id="0297b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0297b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0297b-128">承諾</span><span class="sxs-lookup"><span data-stu-id="0297b-128">Accept</span></span> | <span data-ttu-id="0297b-129">string</span><span class="sxs-lookup"><span data-stu-id="0297b-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="0297b-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="0297b-130">Request body</span></span>
<span data-ttu-id="0297b-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0297b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0297b-132">応答</span><span class="sxs-lookup"><span data-stu-id="0297b-132">Response</span></span>

<span data-ttu-id="0297b-133">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[notebook](../resources/notebook.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0297b-133">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0297b-134">例</span><span class="sxs-lookup"><span data-stu-id="0297b-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0297b-135">要求</span><span class="sxs-lookup"><span data-stu-id="0297b-135">Request</span></span>
<span data-ttu-id="0297b-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0297b-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebook"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}
```
##### <a name="response"></a><span data-ttu-id="0297b-137">応答</span><span class="sxs-lookup"><span data-stu-id="0297b-137">Response</span></span>
<span data-ttu-id="0297b-p103">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0297b-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 284

{
  "isDefault": true,
  "userRole": {
  },
  "isShared": true,
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
