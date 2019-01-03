---
title: inferenceClassificationOverride を削除する
description: その ID で指定されたオーバーライドを削除します。
ms.openlocfilehash: ef4ff995e0e7f4392d9ca13835976076b3fdbe59
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021310"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="8096b-103">inferenceClassificationOverride を削除する</span><span class="sxs-lookup"><span data-stu-id="8096b-103">Delete inferenceClassificationOverride</span></span>

<span data-ttu-id="8096b-104">その ID で指定された上書きを削除します。</span><span class="sxs-lookup"><span data-stu-id="8096b-104">Delete an override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="8096b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8096b-105">Permissions</span></span>
<span data-ttu-id="8096b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8096b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8096b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8096b-108">Permission type</span></span>      | <span data-ttu-id="8096b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8096b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8096b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8096b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8096b-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8096b-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8096b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8096b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8096b-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8096b-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8096b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8096b-114">Application</span></span> | <span data-ttu-id="8096b-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8096b-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8096b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8096b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8096b-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8096b-117">Request headers</span></span>
| <span data-ttu-id="8096b-118">名前</span><span class="sxs-lookup"><span data-stu-id="8096b-118">Name</span></span>       | <span data-ttu-id="8096b-119">型</span><span class="sxs-lookup"><span data-stu-id="8096b-119">Type</span></span> | <span data-ttu-id="8096b-120">説明</span><span class="sxs-lookup"><span data-stu-id="8096b-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8096b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8096b-121">Authorization</span></span>  | <span data-ttu-id="8096b-122">string</span><span class="sxs-lookup"><span data-stu-id="8096b-122">string</span></span>  | <span data-ttu-id="8096b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8096b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8096b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="8096b-125">Request body</span></span>
<span data-ttu-id="8096b-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8096b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8096b-127">応答</span><span class="sxs-lookup"><span data-stu-id="8096b-127">Response</span></span>

<span data-ttu-id="8096b-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="8096b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8096b-130">例</span><span class="sxs-lookup"><span data-stu-id="8096b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8096b-131">要求</span><span class="sxs-lookup"><span data-stu-id="8096b-131">Request</span></span>
<span data-ttu-id="8096b-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8096b-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["98f5bdef-576a-404d-a2ea-07a3cf34af4r"],
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
##### <a name="response"></a><span data-ttu-id="8096b-133">応答</span><span class="sxs-lookup"><span data-stu-id="8096b-133">Response</span></span>
<span data-ttu-id="8096b-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8096b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->