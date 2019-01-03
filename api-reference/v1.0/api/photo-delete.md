---
title: 写真を削除する
description: 写真を削除します。
ms.openlocfilehash: 8d00eb3685d349efaa88981c6a725faa97896bb2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023098"
---
# <a name="delete-photo"></a><span data-ttu-id="b2c63-103">写真を削除する</span><span class="sxs-lookup"><span data-stu-id="b2c63-103">Delete photo</span></span>

<span data-ttu-id="b2c63-104">写真を削除します。</span><span class="sxs-lookup"><span data-stu-id="b2c63-104">Delete a photo.</span></span>
## <a name="permissions"></a><span data-ttu-id="b2c63-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b2c63-105">Permissions</span></span>
<span data-ttu-id="b2c63-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b2c63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2c63-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b2c63-108">Permission type</span></span>      | <span data-ttu-id="b2c63-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b2c63-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2c63-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b2c63-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b2c63-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b2c63-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b2c63-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b2c63-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2c63-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b2c63-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b2c63-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b2c63-114">Application</span></span> | <span data-ttu-id="b2c63-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b2c63-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2c63-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b2c63-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="b2c63-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b2c63-117">Request headers</span></span>
| <span data-ttu-id="b2c63-118">名前</span><span class="sxs-lookup"><span data-stu-id="b2c63-118">Name</span></span>       | <span data-ttu-id="b2c63-119">型</span><span class="sxs-lookup"><span data-stu-id="b2c63-119">Type</span></span> | <span data-ttu-id="b2c63-120">説明</span><span class="sxs-lookup"><span data-stu-id="b2c63-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b2c63-121">if-match</span><span class="sxs-lookup"><span data-stu-id="b2c63-121">if-match</span></span>  | <span data-ttu-id="b2c63-122">文字列</span><span class="sxs-lookup"><span data-stu-id="b2c63-122">string</span></span>  | <span data-ttu-id="b2c63-123">この要求ヘッダーが含まれていて、指定された eTag (または cTag) が項目の現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、項目は削除されません。</span><span class="sxs-lookup"><span data-stu-id="b2c63-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="b2c63-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2c63-124">Authorization</span></span>  | <span data-ttu-id="b2c63-125">string</span><span class="sxs-lookup"><span data-stu-id="b2c63-125">string</span></span>  | <span data-ttu-id="b2c63-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b2c63-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b2c63-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="b2c63-128">Request body</span></span>
<span data-ttu-id="b2c63-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b2c63-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2c63-130">応答</span><span class="sxs-lookup"><span data-stu-id="b2c63-130">Response</span></span>

<span data-ttu-id="b2c63-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="b2c63-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2c63-133">例</span><span class="sxs-lookup"><span data-stu-id="b2c63-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b2c63-134">要求</span><span class="sxs-lookup"><span data-stu-id="b2c63-134">Request</span></span>
<span data-ttu-id="b2c63-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b2c63-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
"name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="b2c63-136">応答</span><span class="sxs-lookup"><span data-stu-id="b2c63-136">Response</span></span>
<span data-ttu-id="b2c63-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b2c63-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->