---
title: paymentTerms の削除
description: Dynamics 365 Business Central の支払い用語オブジェクトを削除します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 2ab608cc7e8f0e6ea17ea9911746fea52fc66a7a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458692"
---
# <a name="delete-paymentterms"></a><span data-ttu-id="8d332-103">paymentTerms の削除</span><span class="sxs-lookup"><span data-stu-id="8d332-103">Delete paymentTerms</span></span>
<span data-ttu-id="8d332-104">Dynamics 365 Business Central から支払い用語オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="8d332-104">Delete a payment terms object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d332-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8d332-105">Permissions</span></span>
<span data-ttu-id="8d332-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8d332-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d332-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8d332-108">Permission type</span></span> |<span data-ttu-id="8d332-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8d332-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="8d332-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8d332-110">Delegated (work or school account)</span></span>|<span data-ttu-id="8d332-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d332-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="8d332-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="8d332-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="8d332-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d332-113">Not supported.</span></span>|
|<span data-ttu-id="8d332-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8d332-114">Application</span></span>|<span data-ttu-id="8d332-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d332-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d332-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8d332-116">HTTP request</span></span>
```
DELETE /financials/companies('{id}')/paymentTerms('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8d332-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8d332-117">Optional query parameters</span></span>
<span data-ttu-id="8d332-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8d332-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d332-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8d332-119">Request headers</span></span>

|<span data-ttu-id="8d332-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8d332-120">Header</span></span>         |<span data-ttu-id="8d332-121">値</span><span class="sxs-lookup"><span data-stu-id="8d332-121">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="8d332-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d332-122">Authorization</span></span>  |<span data-ttu-id="8d332-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8d332-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="8d332-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="8d332-125">If-Match</span></span>       |<span data-ttu-id="8d332-126">必須です。</span><span class="sxs-lookup"><span data-stu-id="8d332-126">Required.</span></span> <span data-ttu-id="8d332-127">この要求ヘッダーが含まれていて、指定された eTag が**paymentTerms**の現在のタグと一致しない場合、 **paymentTerms**は更新されません。</span><span class="sxs-lookup"><span data-stu-id="8d332-127">When this request header is included and the eTag provided does not match the current tag on the **paymentTerms**, the **paymentTerms** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d332-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="8d332-128">Request body</span></span>
<span data-ttu-id="8d332-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8d332-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d332-130">応答</span><span class="sxs-lookup"><span data-stu-id="8d332-130">Response</span></span>
<span data-ttu-id="8d332-p104">成功した場合、このメソッドは ```204 No Content``` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="8d332-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d332-133">例</span><span class="sxs-lookup"><span data-stu-id="8d332-133">Example</span></span>

<span data-ttu-id="8d332-134">**要求**</span><span class="sxs-lookup"><span data-stu-id="8d332-134">**Request**</span></span>

<span data-ttu-id="8d332-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8d332-135">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies('{id}')/paymentTerms('{id}')
```

<span data-ttu-id="8d332-136">**応答**</span><span class="sxs-lookup"><span data-stu-id="8d332-136">**Response**</span></span> 

<span data-ttu-id="8d332-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8d332-137">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```
