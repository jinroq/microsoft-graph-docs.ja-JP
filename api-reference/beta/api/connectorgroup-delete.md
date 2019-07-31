---
title: コネクタグループの削除
description: コネクタグループを削除します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: e8c7d0dc61338b10451f553421b74ad1b41f628f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943478"
---
# <a name="delete-connectorgroup"></a><span data-ttu-id="73b67-103">コネクタグループの削除</span><span class="sxs-lookup"><span data-stu-id="73b67-103">Delete connectorGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73b67-104">コネクタグループを削除します。</span><span class="sxs-lookup"><span data-stu-id="73b67-104">Delete a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="73b67-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="73b67-105">Permissions</span></span>
<span data-ttu-id="73b67-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="73b67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="73b67-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="73b67-108">Permission type</span></span>      | <span data-ttu-id="73b67-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="73b67-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73b67-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="73b67-110">Delegated (work or school account)</span></span> | <span data-ttu-id="73b67-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="73b67-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="73b67-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="73b67-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73b67-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73b67-113">Not supported.</span></span>    |
|<span data-ttu-id="73b67-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="73b67-114">Application</span></span> | <span data-ttu-id="73b67-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73b67-115">Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="73b67-116">**注:** コネクタグループには、コネクタが関連付けられていてはなりません。</span><span class="sxs-lookup"><span data-stu-id="73b67-116">**Note:** The connector group must not have any connectors associated with it.</span></span>

## <a name="http-request"></a><span data-ttu-id="73b67-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="73b67-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /connectorGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="73b67-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="73b67-118">Request headers</span></span>
| <span data-ttu-id="73b67-119">名前</span><span class="sxs-lookup"><span data-stu-id="73b67-119">Name</span></span>       | <span data-ttu-id="73b67-120">説明</span><span class="sxs-lookup"><span data-stu-id="73b67-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="73b67-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="73b67-121">Authorization</span></span>  | <span data-ttu-id="73b67-122">ベアラー.</span><span class="sxs-lookup"><span data-stu-id="73b67-122">Bearer.</span></span> <span data-ttu-id="73b67-123">必須</span><span class="sxs-lookup"><span data-stu-id="73b67-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="73b67-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="73b67-124">Request body</span></span>
<span data-ttu-id="73b67-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="73b67-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73b67-126">応答</span><span class="sxs-lookup"><span data-stu-id="73b67-126">Response</span></span>

<span data-ttu-id="73b67-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="73b67-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73b67-129">例</span><span class="sxs-lookup"><span data-stu-id="73b67-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73b67-130">要求</span><span class="sxs-lookup"><span data-stu-id="73b67-130">Request</span></span>
<span data-ttu-id="73b67-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="73b67-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_connectorgroup"
}-->
```http
DELETE https://graph.microsoft.com/{ver}/connectorGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="73b67-132">応答</span><span class="sxs-lookup"><span data-stu-id="73b67-132">Response</span></span>
<span data-ttu-id="73b67-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="73b67-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
