---
title: inferenceClassificationOverride を削除する
description: その ID で指定された受信トレイの中心のオーバーライドを削除します。
localization_priority: Normal
ms.openlocfilehash: 7db351e11ccfa8e88fe97ff1ee22173a87242d57
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870141"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="26a30-103">inferenceClassificationOverride を削除する</span><span class="sxs-lookup"><span data-stu-id="26a30-103">Delete inferenceClassificationOverride</span></span>

> <span data-ttu-id="26a30-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="26a30-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26a30-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26a30-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="26a30-106">その ID で指定された[受信トレイの中心](../resources/manage-focused-inbox.md)のオーバーライドを削除します。</span><span class="sxs-lookup"><span data-stu-id="26a30-106">Delete a [Focused Inbox](../resources/manage-focused-inbox.md) override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="26a30-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="26a30-107">Permissions</span></span>
<span data-ttu-id="26a30-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="26a30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26a30-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="26a30-110">Permission type</span></span>      | <span data-ttu-id="26a30-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="26a30-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26a30-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="26a30-112">Delegated (work or school account)</span></span> | <span data-ttu-id="26a30-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26a30-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="26a30-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="26a30-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26a30-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26a30-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="26a30-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="26a30-116">Application</span></span> | <span data-ttu-id="26a30-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26a30-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="26a30-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="26a30-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="26a30-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26a30-119">Request headers</span></span>
| <span data-ttu-id="26a30-120">名前</span><span class="sxs-lookup"><span data-stu-id="26a30-120">Name</span></span>       | <span data-ttu-id="26a30-121">種類</span><span class="sxs-lookup"><span data-stu-id="26a30-121">Type</span></span> | <span data-ttu-id="26a30-122">説明</span><span class="sxs-lookup"><span data-stu-id="26a30-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="26a30-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="26a30-123">Authorization</span></span>  | <span data-ttu-id="26a30-124">string</span><span class="sxs-lookup"><span data-stu-id="26a30-124">string</span></span>  | <span data-ttu-id="26a30-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="26a30-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26a30-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="26a30-127">Request body</span></span>
<span data-ttu-id="26a30-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="26a30-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26a30-129">応答</span><span class="sxs-lookup"><span data-stu-id="26a30-129">Response</span></span>

<span data-ttu-id="26a30-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="26a30-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26a30-132">例</span><span class="sxs-lookup"><span data-stu-id="26a30-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26a30-133">要求</span><span class="sxs-lookup"><span data-stu-id="26a30-133">Request</span></span>
<span data-ttu-id="26a30-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="26a30-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
##### <a name="response"></a><span data-ttu-id="26a30-135">応答</span><span class="sxs-lookup"><span data-stu-id="26a30-135">Response</span></span>
<span data-ttu-id="26a30-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="26a30-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
