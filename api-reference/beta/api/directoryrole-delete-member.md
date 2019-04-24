---
title: ディレクトリ ロールのメンバーを削除する
description: directoryRole からメンバーを削除します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c45436660ed84476efd293095efb185757c01249
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455126"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="64988-103">ディレクトリ ロールのメンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="64988-103">Remove directory role member</span></span>

<span data-ttu-id="64988-104">directoryRole からメンバーを削除します。</span><span class="sxs-lookup"><span data-stu-id="64988-104">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="64988-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="64988-105">Permissions</span></span>

<span data-ttu-id="64988-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="64988-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="64988-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="64988-108">Permission type</span></span>      | <span data-ttu-id="64988-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="64988-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64988-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="64988-110">Delegated (work or school account)</span></span> | <span data-ttu-id="64988-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="64988-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="64988-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="64988-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64988-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="64988-113">Not supported.</span></span>    |
|<span data-ttu-id="64988-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="64988-114">Application</span></span> | <span data-ttu-id="64988-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="64988-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="64988-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="64988-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryRoles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="64988-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="64988-117">Request headers</span></span>

| <span data-ttu-id="64988-118">名前</span><span class="sxs-lookup"><span data-stu-id="64988-118">Name</span></span>       | <span data-ttu-id="64988-119">型</span><span class="sxs-lookup"><span data-stu-id="64988-119">Type</span></span> | <span data-ttu-id="64988-120">説明</span><span class="sxs-lookup"><span data-stu-id="64988-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="64988-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="64988-121">Authorization</span></span>  | <span data-ttu-id="64988-122">string</span><span class="sxs-lookup"><span data-stu-id="64988-122">string</span></span>  | <span data-ttu-id="64988-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="64988-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64988-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="64988-125">Request body</span></span>

<span data-ttu-id="64988-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="64988-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64988-127">応答</span><span class="sxs-lookup"><span data-stu-id="64988-127">Response</span></span>

<span data-ttu-id="64988-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="64988-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64988-130">例</span><span class="sxs-lookup"><span data-stu-id="64988-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="64988-131">要求</span><span class="sxs-lookup"><span data-stu-id="64988-131">Request</span></span>

<span data-ttu-id="64988-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="64988-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/{id}/members/{id}/$ref
```

##### <a name="response"></a><span data-ttu-id="64988-133">応答</span><span class="sxs-lookup"><span data-stu-id="64988-133">Response</span></span>

<span data-ttu-id="64988-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="64988-134">Here is an example of the response.</span></span> 
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
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
