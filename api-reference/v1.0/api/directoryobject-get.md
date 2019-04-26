---
title: directoryObject を取得する
description: directoryObject オブジェクトのプロパティとリレーションシップを取得します。
author: lleonard-msft
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 79cf534fc154257a952bef6494c3aa0124dfb928
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571948"
---
# <a name="get-directoryobject"></a><span data-ttu-id="a904a-103">directoryObject を取得する</span><span class="sxs-lookup"><span data-stu-id="a904a-103">Get directoryObject</span></span>

<span data-ttu-id="a904a-104">directoryObject オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="a904a-104">Retrieve the properties and relationships of directoryObject object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a904a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a904a-105">Permissions</span></span>
<span data-ttu-id="a904a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a904a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a904a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a904a-108">Permission type</span></span>      | <span data-ttu-id="a904a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a904a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a904a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a904a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a904a-111">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a904a-111">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a904a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a904a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a904a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a904a-113">Not supported.</span></span>    |
|<span data-ttu-id="a904a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a904a-114">Application</span></span> | <span data-ttu-id="a904a-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a904a-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a904a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a904a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryObjects/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a904a-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a904a-117">Optional query parameters</span></span>
<span data-ttu-id="a904a-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a904a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a904a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a904a-119">Request headers</span></span>
| <span data-ttu-id="a904a-120">名前</span><span class="sxs-lookup"><span data-stu-id="a904a-120">Name</span></span>       | <span data-ttu-id="a904a-121">型</span><span class="sxs-lookup"><span data-stu-id="a904a-121">Type</span></span> | <span data-ttu-id="a904a-122">説明</span><span class="sxs-lookup"><span data-stu-id="a904a-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a904a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a904a-123">Authorization</span></span>  | <span data-ttu-id="a904a-124">string</span><span class="sxs-lookup"><span data-stu-id="a904a-124">string</span></span>  | <span data-ttu-id="a904a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a904a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a904a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a904a-127">Request body</span></span>
<span data-ttu-id="a904a-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a904a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a904a-129">応答</span><span class="sxs-lookup"><span data-stu-id="a904a-129">Response</span></span>

<span data-ttu-id="a904a-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a904a-130">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a904a-131">例</span><span class="sxs-lookup"><span data-stu-id="a904a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a904a-132">要求</span><span class="sxs-lookup"><span data-stu-id="a904a-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
##### <a name="response"></a><span data-ttu-id="a904a-133">応答</span><span class="sxs-lookup"><span data-stu-id="a904a-133">Response</span></span>
<span data-ttu-id="a904a-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a904a-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
