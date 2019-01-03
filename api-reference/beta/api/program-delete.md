---
title: プログラムを削除します。
description: Azure AD のレビュー機能にアクセス、プログラム オブジェクトを削除します。
ms.openlocfilehash: c09dcc36bfc4fbf279e7b6c49ea24bba9153c071
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072020"
---
# <a name="delete-program"></a><span data-ttu-id="e9a9a-103">プログラムを削除します。</span><span class="sxs-lookup"><span data-stu-id="e9a9a-103">Delete program</span></span>

> <span data-ttu-id="e9a9a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e9a9a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9a9a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e9a9a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e9a9a-106">Azure AD[アクセスの確認](../resources/accessreviews-root.md)機能では、[プログラム](../resources/program.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="e9a9a-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="e9a9a-107">まだプログラムを削除しないで`programControl`にリンクして、それらのアクセスのレビュー最初を削除またはプログラムからのリンクを解除し、別のプログラムにリンクします。</span><span class="sxs-lookup"><span data-stu-id="e9a9a-107">Do not delete a program which still has `programControl` linked to it, those access reviews should first be deleted or unlinked from the program and linked to a different program.</span></span>  <span data-ttu-id="e9a9a-108">また、組み込みの既定のプログラムを削除できないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="e9a9a-108">Also, please note that the built-in default program cannot be deleted.</span></span>


## <a name="permissions"></a><span data-ttu-id="e9a9a-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e9a9a-109">Permissions</span></span>
<span data-ttu-id="e9a9a-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e9a9a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9a9a-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e9a9a-112">Permission type</span></span>                        | <span data-ttu-id="e9a9a-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e9a9a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9a9a-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e9a9a-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="e9a9a-115">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="e9a9a-115"></span></span>  <span data-ttu-id="e9a9a-116">サインインしているユーザーは、プログラムを作成することを許可するディレクトリの役割でもあります。</span><span class="sxs-lookup"><span data-stu-id="e9a9a-116">The signed in user must also be in a directory role which permits them to create a program.</span></span> |
|<span data-ttu-id="e9a9a-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e9a9a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9a9a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e9a9a-118">Not supported.</span></span> |
|<span data-ttu-id="e9a9a-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e9a9a-119">Application</span></span>                            | <span data-ttu-id="e9a9a-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e9a9a-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9a9a-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e9a9a-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programs('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="e9a9a-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e9a9a-122">Request headers</span></span>
| <span data-ttu-id="e9a9a-123">名前</span><span class="sxs-lookup"><span data-stu-id="e9a9a-123">Name</span></span>         | <span data-ttu-id="e9a9a-124">型</span><span class="sxs-lookup"><span data-stu-id="e9a9a-124">Type</span></span>        | <span data-ttu-id="e9a9a-125">説明</span><span class="sxs-lookup"><span data-stu-id="e9a9a-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e9a9a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9a9a-126">Authorization</span></span> | <span data-ttu-id="e9a9a-127">string</span><span class="sxs-lookup"><span data-stu-id="e9a9a-127">string</span></span> | <span data-ttu-id="e9a9a-128">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="e9a9a-128">Bearer \{token\}.</span></span> <span data-ttu-id="e9a9a-129">必須。</span><span class="sxs-lookup"><span data-stu-id="e9a9a-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9a9a-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="e9a9a-130">Request body</span></span>
<span data-ttu-id="e9a9a-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e9a9a-131">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="e9a9a-132">応答</span><span class="sxs-lookup"><span data-stu-id="e9a9a-132">Response</span></span>
<span data-ttu-id="e9a9a-p106">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e9a9a-p106">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9a9a-135">例</span><span class="sxs-lookup"><span data-stu-id="e9a9a-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e9a9a-136">要求</span><span class="sxs-lookup"><span data-stu-id="e9a9a-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_program"
}-->
```http
DELETE https://graph.microsoft.com/beta/programs('7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
```
##### <a name="response"></a><span data-ttu-id="e9a9a-137">応答</span><span class="sxs-lookup"><span data-stu-id="e9a9a-137">Response</span></span>
><span data-ttu-id="e9a9a-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e9a9a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->