---
title: セッションを更新する
description: 'この API を使用して、既存のブックのセッションを更新します。 '
author: lumine2008
ms.openlocfilehash: 4f039b0dd32cbcf5ba0e0a0346a593abc4078df3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336156"
---
# <a name="refresh-session"></a><span data-ttu-id="b4329-103">セッションを更新する</span><span class="sxs-lookup"><span data-stu-id="b4329-103">Refresh Session</span></span>

<span data-ttu-id="b4329-104">この API を使用して、既存のブックのセッションを更新します。</span><span class="sxs-lookup"><span data-stu-id="b4329-104">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b4329-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b4329-105">Permissions</span></span>
<span data-ttu-id="b4329-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b4329-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4329-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b4329-108">Permission type</span></span>      | <span data-ttu-id="b4329-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b4329-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4329-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b4329-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b4329-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4329-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b4329-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b4329-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4329-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4329-113">Not supported.</span></span>    |
|<span data-ttu-id="b4329-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b4329-114">Application</span></span> | <span data-ttu-id="b4329-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4329-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4329-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b4329-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="b4329-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b4329-117">Request headers</span></span>
| <span data-ttu-id="b4329-118">名前</span><span class="sxs-lookup"><span data-stu-id="b4329-118">Name</span></span>       | <span data-ttu-id="b4329-119">説明</span><span class="sxs-lookup"><span data-stu-id="b4329-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b4329-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4329-120">Authorization</span></span>  | <span data-ttu-id="b4329-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b4329-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b4329-123">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="b4329-123">workbook-session-id</span></span> | <span data-ttu-id="b4329-124">更新するブック セッションの ID</span><span class="sxs-lookup"><span data-stu-id="b4329-124">Workbook session Id to be refreshed</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4329-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b4329-125">Request body</span></span>
<span data-ttu-id="b4329-126">この API は、要求本文を必要としません。</span><span class="sxs-lookup"><span data-stu-id="b4329-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="b4329-127">応答</span><span class="sxs-lookup"><span data-stu-id="b4329-127">Response</span></span>

<span data-ttu-id="b4329-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="b4329-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b4329-129">例</span><span class="sxs-lookup"><span data-stu-id="b4329-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b4329-130">要求</span><span class="sxs-lookup"><span data-stu-id="b4329-130">Request</span></span>
<span data-ttu-id="b4329-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b4329-131">Here is an example of the request.</span></span>
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

<span data-ttu-id="b4329-132">workbook-session-id ヘッダーが必要となることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="b4329-132">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="b4329-133">応答</span><span class="sxs-lookup"><span data-stu-id="b4329-133">Response</span></span>
<span data-ttu-id="b4329-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b4329-134">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```