---
title: inferenceClassificationOverride を削除する
description: ID で指定された優先受信トレイの上書きを削除します。
localization_priority: Normal
ms.openlocfilehash: 8c9213f48a0d7cc430b0177d6c3d3ff30819202e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328623"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="2a148-103">inferenceClassificationOverride を削除する</span><span class="sxs-lookup"><span data-stu-id="2a148-103">Delete inferenceClassificationOverride</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a148-104">ID で指定された[優先受信トレイ](../resources/manage-focused-inbox.md)の上書きを削除します。</span><span class="sxs-lookup"><span data-stu-id="2a148-104">Delete a [Focused Inbox](../resources/manage-focused-inbox.md) override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="2a148-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2a148-105">Permissions</span></span>
<span data-ttu-id="2a148-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a148-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a148-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2a148-108">Permission type</span></span>      | <span data-ttu-id="2a148-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2a148-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a148-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2a148-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2a148-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a148-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2a148-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2a148-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a148-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a148-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2a148-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2a148-114">Application</span></span> | <span data-ttu-id="2a148-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a148-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a148-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2a148-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2a148-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2a148-117">Request headers</span></span>
| <span data-ttu-id="2a148-118">名前</span><span class="sxs-lookup"><span data-stu-id="2a148-118">Name</span></span>       | <span data-ttu-id="2a148-119">型</span><span class="sxs-lookup"><span data-stu-id="2a148-119">Type</span></span> | <span data-ttu-id="2a148-120">説明</span><span class="sxs-lookup"><span data-stu-id="2a148-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2a148-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a148-121">Authorization</span></span>  | <span data-ttu-id="2a148-122">string</span><span class="sxs-lookup"><span data-stu-id="2a148-122">string</span></span>  | <span data-ttu-id="2a148-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2a148-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a148-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="2a148-125">Request body</span></span>
<span data-ttu-id="2a148-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2a148-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a148-127">応答</span><span class="sxs-lookup"><span data-stu-id="2a148-127">Response</span></span>

<span data-ttu-id="2a148-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="2a148-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a148-130">例</span><span class="sxs-lookup"><span data-stu-id="2a148-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2a148-131">要求</span><span class="sxs-lookup"><span data-stu-id="2a148-131">Request</span></span>
<span data-ttu-id="2a148-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2a148-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
##### <a name="response"></a><span data-ttu-id="2a148-133">応答</span><span class="sxs-lookup"><span data-stu-id="2a148-133">Response</span></span>
<span data-ttu-id="2a148-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2a148-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
