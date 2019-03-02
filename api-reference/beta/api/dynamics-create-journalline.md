---
title: journalLines を作成する
description: Dynamics 365 Business Central の仕訳帳明細行を作成します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: c6ed8b1ccbe1f33cad174e1c5e4f9b3832f2a5c9
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365424"
---
# <a name="create-journallines"></a><span data-ttu-id="0e76e-103">journalLines を作成する</span><span class="sxs-lookup"><span data-stu-id="0e76e-103">Create journalLines</span></span>
<span data-ttu-id="0e76e-104">Dynamics 365 Business Central に、ジャーナル明細行オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0e76e-104">Creates a journal line object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e76e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0e76e-105">Permissions</span></span>
<span data-ttu-id="0e76e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0e76e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e76e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0e76e-108">Permission type</span></span> |<span data-ttu-id="0e76e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0e76e-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="0e76e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0e76e-110">Delegated (work or school account)</span></span>|<span data-ttu-id="0e76e-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e76e-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="0e76e-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="0e76e-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="0e76e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0e76e-113">Not supported.</span></span>|
|<span data-ttu-id="0e76e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0e76e-114">Application</span></span>|<span data-ttu-id="0e76e-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e76e-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e76e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0e76e-116">HTTP request</span></span>

```
POST /financials/companies('{id}')/journals('{id}')/journalLines('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0e76e-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0e76e-117">Optional query parameters</span></span>
<span data-ttu-id="0e76e-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0e76e-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e76e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0e76e-119">Request headers</span></span>
|<span data-ttu-id="0e76e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0e76e-120">Header</span></span>        |<span data-ttu-id="0e76e-121">値</span><span class="sxs-lookup"><span data-stu-id="0e76e-121">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="0e76e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e76e-122">Authorization</span></span> |<span data-ttu-id="0e76e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0e76e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0e76e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0e76e-125">Content-Type</span></span>  |<span data-ttu-id="0e76e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e76e-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="0e76e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0e76e-127">Request body</span></span>
<span data-ttu-id="0e76e-128">要求本文で、 **journalLines**オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0e76e-128">In the request body, supply a JSON representation of **journalLines** object.</span></span>

## <a name="response"></a><span data-ttu-id="0e76e-129">応答</span><span class="sxs-lookup"><span data-stu-id="0e76e-129">Response</span></span>
<span data-ttu-id="0e76e-130">成功した場合、この```201 Created```メソッドは応答コードと、応答本文で**journalLines**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0e76e-130">If successful, this method returns ```201 Created``` response code and **journalLines** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e76e-131">例</span><span class="sxs-lookup"><span data-stu-id="0e76e-131">Example</span></span>

<span data-ttu-id="0e76e-132">**要求**</span><span class="sxs-lookup"><span data-stu-id="0e76e-132">**Request**</span></span>

<span data-ttu-id="0e76e-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0e76e-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/journals('{id}')/journalLines
Content-type: application/json

{
  "lineNumber": 10000,
  "accountId": "id-value",
  "accountNumber": "10400",
  "postingDate": "2015-12-31",
  "documentNumber": "1234",
  "externalDocumentNumber": "",
  "amount": 1500,
  "description": "Accounts Receivable",
  "comment": ""
}
```
<span data-ttu-id="0e76e-134">**応答**</span><span class="sxs-lookup"><span data-stu-id="0e76e-134">**Response**</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "journalDisplayName": "DEFAULT",
  "lineNumber": 10000,
  "accountId": "id-value",
  "accountNumber": "10400",
  "postingDate": "2015-12-31",
  "documentNumber": "1234",
  "externalDocumentNumber": "",
  "amount": 1500,
  "description": "Accounts Receivable",
  "comment": "",
  "lastModifiedDateTime": "2017-03-17T19:02:22.043Z"
}
```


