---
title: CountriesRegions の削除
description: Dynamics 365 Business Central の国/地域オブジェクトを削除します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 68b0ceaa1beef3528cf3afc228b961fe737f3bac
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956780"
---
# <a name="delete-countriesregions"></a><span data-ttu-id="3bf09-103">CountriesRegions の削除</span><span class="sxs-lookup"><span data-stu-id="3bf09-103">Delete countriesRegions</span></span>
<span data-ttu-id="3bf09-104">Dynamics 365 Business Central から国/地域オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="3bf09-104">Delete a countries/regions object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="3bf09-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3bf09-105">Permissions</span></span>
<span data-ttu-id="3bf09-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3bf09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bf09-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3bf09-108">Permission type</span></span> |<span data-ttu-id="3bf09-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3bf09-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="3bf09-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3bf09-110">Delegated (work or school account)</span></span>|<span data-ttu-id="3bf09-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bf09-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="3bf09-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="3bf09-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="3bf09-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3bf09-113">Not supported.</span></span>|
|<span data-ttu-id="3bf09-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3bf09-114">Application</span></span>|<span data-ttu-id="3bf09-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bf09-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bf09-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3bf09-116">HTTP request</span></span>
```
DELETE /financials/companies('{id}')/countriesRegions('{id}')
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3bf09-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3bf09-117">Optional query parameters</span></span>
<span data-ttu-id="3bf09-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3bf09-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3bf09-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3bf09-119">Request headers</span></span>
|<span data-ttu-id="3bf09-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3bf09-120">Header</span></span>|<span data-ttu-id="3bf09-121">値</span><span class="sxs-lookup"><span data-stu-id="3bf09-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="3bf09-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3bf09-122">Authorization</span></span>  |<span data-ttu-id="3bf09-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3bf09-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="3bf09-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="3bf09-125">If-Match</span></span>       |<span data-ttu-id="3bf09-126">必須です。</span><span class="sxs-lookup"><span data-stu-id="3bf09-126">Required.</span></span> <span data-ttu-id="3bf09-127">この要求ヘッダーが含まれていて、指定された eTag が**countriesRegions**の現在のタグと一致しない場合、 **countriesRegions**は更新されません。</span><span class="sxs-lookup"><span data-stu-id="3bf09-127">When this request header is included and the eTag provided does not match the current tag on the **countriesRegions**, the **countriesRegions** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3bf09-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="3bf09-128">Request body</span></span>
<span data-ttu-id="3bf09-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3bf09-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3bf09-130">応答</span><span class="sxs-lookup"><span data-stu-id="3bf09-130">Response</span></span>
<span data-ttu-id="3bf09-p104">成功した場合、このメソッドは ```204 No Content``` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="3bf09-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bf09-133">例</span><span class="sxs-lookup"><span data-stu-id="3bf09-133">Example</span></span>

<span data-ttu-id="3bf09-134">**要求**</span><span class="sxs-lookup"><span data-stu-id="3bf09-134">**Request**</span></span>

<span data-ttu-id="3bf09-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3bf09-135">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies('{id}')/countriesRegions('{id}')
```

<span data-ttu-id="3bf09-136">**応答**</span><span class="sxs-lookup"><span data-stu-id="3bf09-136">**Response**</span></span> 

<span data-ttu-id="3bf09-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="3bf09-137">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```
