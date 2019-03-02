---
title: 通貨の削除
description: Dynamics 365 Business Central の currency オブジェクトを削除します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 54ff3632680d0819c33a6594a2a3c3b9e882fd98
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365368"
---
# <a name="delete-currencies"></a><span data-ttu-id="d58e5-103">通貨の削除</span><span class="sxs-lookup"><span data-stu-id="d58e5-103">Delete currencies</span></span>
<span data-ttu-id="d58e5-104">Dynamics 365 Business Central から currency オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="d58e5-104">Delete a currency object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="d58e5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d58e5-105">Permissions</span></span>
<span data-ttu-id="d58e5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d58e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d58e5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d58e5-108">Permission type</span></span> |<span data-ttu-id="d58e5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d58e5-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="d58e5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d58e5-110">Delegated (work or school account)</span></span>|<span data-ttu-id="d58e5-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d58e5-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="d58e5-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="d58e5-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="d58e5-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d58e5-113">Not supported.</span></span>|
|<span data-ttu-id="d58e5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d58e5-114">Application</span></span>|<span data-ttu-id="d58e5-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d58e5-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d58e5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d58e5-116">HTTP request</span></span>
```
DELETE /financials/companies('{id}')/currencies('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d58e5-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d58e5-117">Optional query parameters</span></span>
<span data-ttu-id="d58e5-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d58e5-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d58e5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d58e5-119">Request headers</span></span>

|<span data-ttu-id="d58e5-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d58e5-120">Header</span></span>|<span data-ttu-id="d58e5-121">値</span><span class="sxs-lookup"><span data-stu-id="d58e5-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="d58e5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d58e5-122">Authorization</span></span>  |<span data-ttu-id="d58e5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d58e5-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="d58e5-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="d58e5-125">If-Match</span></span>       |<span data-ttu-id="d58e5-126">必須です。</span><span class="sxs-lookup"><span data-stu-id="d58e5-126">Required.</span></span> <span data-ttu-id="d58e5-127">この要求ヘッダーが含まれていて、指定された eTag が**通貨**の現在のタグと一致しない場合、**通貨**は次のようになりません。</span><span class="sxs-lookup"><span data-stu-id="d58e5-127">When this request header is included and the eTag provided does not match the current tag on the **currencies**, the **currencies** will not be</span></span>
 <span data-ttu-id="d58e5-128">まし.</span><span class="sxs-lookup"><span data-stu-id="d58e5-128">updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d58e5-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="d58e5-129">Request body</span></span>
<span data-ttu-id="d58e5-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d58e5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d58e5-131">応答</span><span class="sxs-lookup"><span data-stu-id="d58e5-131">Response</span></span>
<span data-ttu-id="d58e5-p104">成功した場合、このメソッドは ```204 No Content``` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="d58e5-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d58e5-134">例</span><span class="sxs-lookup"><span data-stu-id="d58e5-134">Example</span></span>

<span data-ttu-id="d58e5-135">**要求**</span><span class="sxs-lookup"><span data-stu-id="d58e5-135">**Request**</span></span>

<span data-ttu-id="d58e5-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d58e5-136">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies('{id}')/currencies('{id}')
```

<span data-ttu-id="d58e5-137">**応答**</span><span class="sxs-lookup"><span data-stu-id="d58e5-137">**Response**</span></span> 

<span data-ttu-id="d58e5-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d58e5-138">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```
