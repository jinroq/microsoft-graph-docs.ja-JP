---
title: セッションを更新する
description: 'この API を使用して、既存のブックのセッションを更新します。 '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c10372e332072eb69bfb605484695d950185e62c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534697"
---
# <a name="refresh-session"></a><span data-ttu-id="c078c-103">セッションを更新する</span><span class="sxs-lookup"><span data-stu-id="c078c-103">Refresh Session</span></span>

<span data-ttu-id="c078c-104">この API を使用して、既存のブックのセッションを更新します。</span><span class="sxs-lookup"><span data-stu-id="c078c-104">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="c078c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c078c-105">Permissions</span></span>
<span data-ttu-id="c078c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c078c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c078c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c078c-108">Permission type</span></span>      | <span data-ttu-id="c078c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c078c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c078c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c078c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c078c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c078c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c078c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c078c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c078c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c078c-113">Not supported.</span></span>    |
|<span data-ttu-id="c078c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c078c-114">Application</span></span> | <span data-ttu-id="c078c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c078c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c078c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c078c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="c078c-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c078c-117">Request headers</span></span>
| <span data-ttu-id="c078c-118">名前</span><span class="sxs-lookup"><span data-stu-id="c078c-118">Name</span></span>       | <span data-ttu-id="c078c-119">説明</span><span class="sxs-lookup"><span data-stu-id="c078c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c078c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c078c-120">Authorization</span></span>  | <span data-ttu-id="c078c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c078c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c078c-123">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="c078c-123">workbook-session-id</span></span> | <span data-ttu-id="c078c-124">更新するブック セッションの ID</span><span class="sxs-lookup"><span data-stu-id="c078c-124">Workbook session Id to be refreshed</span></span> |

## <a name="request-body"></a><span data-ttu-id="c078c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c078c-125">Request body</span></span>
<span data-ttu-id="c078c-126">この API は、要求本文を必要としません。</span><span class="sxs-lookup"><span data-stu-id="c078c-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="c078c-127">応答</span><span class="sxs-lookup"><span data-stu-id="c078c-127">Response</span></span>

<span data-ttu-id="c078c-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="c078c-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c078c-129">例</span><span class="sxs-lookup"><span data-stu-id="c078c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c078c-130">要求</span><span class="sxs-lookup"><span data-stu-id="c078c-130">Request</span></span>
<span data-ttu-id="c078c-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c078c-131">Here is an example of the request.</span></span>
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

<span data-ttu-id="c078c-132">workbook-session-id ヘッダーが必要となることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="c078c-132">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="c078c-133">応答</span><span class="sxs-lookup"><span data-stu-id="c078c-133">Response</span></span>
<span data-ttu-id="c078c-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c078c-134">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
