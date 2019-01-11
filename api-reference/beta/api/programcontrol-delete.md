---
title: デバッギングを削除します。
description: Azure AD のレビュー機能にアクセス、デバッギング オブジェクトを削除します。  プログラムからのアクセス レビューのリンクを解除します。
localization_priority: Normal
ms.openlocfilehash: 782cc8f336e84f82d937e3180d7de6af69e67e52
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843919"
---
# <a name="delete-programcontrol"></a><span data-ttu-id="f0054-104">デバッギングを削除します。</span><span class="sxs-lookup"><span data-stu-id="f0054-104">Delete programControl</span></span>

> <span data-ttu-id="f0054-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f0054-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0054-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0054-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f0054-107">Azure AD[アクセスの確認](../resources/accessreviews-root.md)機能では、[デバッギング](../resources/programcontrol.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="f0054-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="f0054-108">プログラムからのアクセス レビューのリンクを解除します。</span><span class="sxs-lookup"><span data-stu-id="f0054-108">This unlinks an access review from a program.</span></span>
## <a name="permissions"></a><span data-ttu-id="f0054-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f0054-109">Permissions</span></span>
<span data-ttu-id="f0054-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f0054-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0054-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f0054-112">Permission type</span></span>                        | <span data-ttu-id="f0054-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f0054-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0054-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f0054-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="f0054-115">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="f0054-115"></span></span>  <span data-ttu-id="f0054-116">サインインしているユーザーは、ディレクトリの役割、デバッギングを削除することを許可する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f0054-116">The signed in user must also be in a directory role which permits them to delete a programControl.</span></span> |
|<span data-ttu-id="f0054-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f0054-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0054-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0054-118">Not supported.</span></span> |
|<span data-ttu-id="f0054-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f0054-119">Application</span></span>                            | <span data-ttu-id="f0054-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0054-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0054-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f0054-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programControls('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="f0054-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f0054-122">Request headers</span></span>
| <span data-ttu-id="f0054-123">名前</span><span class="sxs-lookup"><span data-stu-id="f0054-123">Name</span></span>         | <span data-ttu-id="f0054-124">種類</span><span class="sxs-lookup"><span data-stu-id="f0054-124">Type</span></span>        | <span data-ttu-id="f0054-125">説明</span><span class="sxs-lookup"><span data-stu-id="f0054-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f0054-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0054-126">Authorization</span></span> | <span data-ttu-id="f0054-127">string</span><span class="sxs-lookup"><span data-stu-id="f0054-127">string</span></span> | <span data-ttu-id="f0054-128">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="f0054-128">Bearer \{token\}.</span></span> <span data-ttu-id="f0054-129">必須。</span><span class="sxs-lookup"><span data-stu-id="f0054-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0054-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="f0054-130">Request body</span></span>
<span data-ttu-id="f0054-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f0054-131">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="f0054-132">応答</span><span class="sxs-lookup"><span data-stu-id="f0054-132">Response</span></span>
<span data-ttu-id="f0054-p107">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="f0054-p107">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0054-135">例</span><span class="sxs-lookup"><span data-stu-id="f0054-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0054-136">要求</span><span class="sxs-lookup"><span data-stu-id="f0054-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_programControl"
}-->
```http
DELETE https://graph.microsoft.com/beta/programControls('7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
```
##### <a name="response"></a><span data-ttu-id="f0054-137">応答</span><span class="sxs-lookup"><span data-stu-id="f0054-137">Response</span></span>
><span data-ttu-id="f0054-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f0054-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
