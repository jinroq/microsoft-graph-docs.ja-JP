---
title: セッションを更新する
description: 'この API を使用して、既存のブックのセッションを更新します。 '
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 2f4d454214d2f21d1f6447ee224f3013cebb9078
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822338"
---
# <a name="refresh-session"></a><span data-ttu-id="7c723-103">セッションを更新する</span><span class="sxs-lookup"><span data-stu-id="7c723-103">Refresh Session</span></span>

<span data-ttu-id="7c723-104">この API を使用して、既存のブックのセッションを更新します。</span><span class="sxs-lookup"><span data-stu-id="7c723-104">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="7c723-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7c723-105">Permissions</span></span>
<span data-ttu-id="7c723-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7c723-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c723-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7c723-108">Permission type</span></span>      | <span data-ttu-id="7c723-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7c723-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c723-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7c723-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7c723-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c723-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7c723-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7c723-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c723-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c723-113">Not supported.</span></span>    |
|<span data-ttu-id="7c723-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7c723-114">Application</span></span> | <span data-ttu-id="7c723-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c723-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c723-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7c723-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="7c723-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c723-117">Request headers</span></span>
| <span data-ttu-id="7c723-118">名前</span><span class="sxs-lookup"><span data-stu-id="7c723-118">Name</span></span>       | <span data-ttu-id="7c723-119">説明</span><span class="sxs-lookup"><span data-stu-id="7c723-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7c723-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c723-120">Authorization</span></span>  | <span data-ttu-id="7c723-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7c723-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7c723-123">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="7c723-123">workbook-session-id</span></span> | <span data-ttu-id="7c723-124">更新するブック セッションの ID</span><span class="sxs-lookup"><span data-stu-id="7c723-124">Workbook session Id to be refreshed</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c723-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="7c723-125">Request body</span></span>
<span data-ttu-id="7c723-126">この API は、要求本文を必要としません。</span><span class="sxs-lookup"><span data-stu-id="7c723-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="7c723-127">応答</span><span class="sxs-lookup"><span data-stu-id="7c723-127">Response</span></span>

<span data-ttu-id="7c723-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="7c723-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7c723-129">例</span><span class="sxs-lookup"><span data-stu-id="7c723-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7c723-130">要求</span><span class="sxs-lookup"><span data-stu-id="7c723-130">Request</span></span>
<span data-ttu-id="7c723-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7c723-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "refresh_excel_session"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/refreshSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```

<span data-ttu-id="7c723-132">workbook-session-id ヘッダーが必要となることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="7c723-132">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="7c723-133">応答</span><span class="sxs-lookup"><span data-stu-id="7c723-133">Response</span></span>
<span data-ttu-id="7c723-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="7c723-134">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
