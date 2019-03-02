---
title: 仕訳帳を作成する
description: Dynamics 365 Business Central に journal オブジェクトを作成します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 27bef92d9392cd6369564e86417b438ed8bd5a5a
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365830"
---
# <a name="create-journals"></a><span data-ttu-id="be6c4-103">仕訳帳を作成する</span><span class="sxs-lookup"><span data-stu-id="be6c4-103">Create journals</span></span>
<span data-ttu-id="be6c4-104">Dynamics 365 Business Central にジャーナルを作成します。</span><span class="sxs-lookup"><span data-stu-id="be6c4-104">Creates a journal in Dynamics 365 Business Central.</span></span> 

## <a name="permissions"></a><span data-ttu-id="be6c4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="be6c4-105">Permissions</span></span>
<span data-ttu-id="be6c4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be6c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be6c4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="be6c4-108">Permission type</span></span> |<span data-ttu-id="be6c4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="be6c4-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="be6c4-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="be6c4-110">Delegated (work or school account)</span></span>|<span data-ttu-id="be6c4-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be6c4-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="be6c4-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="be6c4-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="be6c4-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be6c4-113">Not supported.</span></span>|
|<span data-ttu-id="be6c4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="be6c4-114">Application</span></span>|<span data-ttu-id="be6c4-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be6c4-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="be6c4-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="be6c4-116">HTTP request</span></span>

```
POST /financials/companies('{id}')/journals('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="be6c4-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="be6c4-117">Optional query parameters</span></span>
<span data-ttu-id="be6c4-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="be6c4-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be6c4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="be6c4-119">Request headers</span></span>
|<span data-ttu-id="be6c4-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="be6c4-120">Header</span></span>        |<span data-ttu-id="be6c4-121">値</span><span class="sxs-lookup"><span data-stu-id="be6c4-121">Value</span></span>                     |
|--------------|--------------------------|
|<span data-ttu-id="be6c4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="be6c4-122">Authorization</span></span> |<span data-ttu-id="be6c4-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="be6c4-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="be6c4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="be6c4-125">Content-Type</span></span>  |<span data-ttu-id="be6c4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="be6c4-126">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="be6c4-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="be6c4-127">Request body</span></span>
<span data-ttu-id="be6c4-128">要求本文で、**ジャーナル**オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="be6c4-128">In the request body, supply a JSON representation of a **journals** object.</span></span>

## <a name="response"></a><span data-ttu-id="be6c4-129">応答</span><span class="sxs-lookup"><span data-stu-id="be6c4-129">Response</span></span>
<span data-ttu-id="be6c4-130">成功した場合、この```201 Created```メソッドは応答コードと、応答本文で**ジャーナル**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="be6c4-130">If successful, this method returns ```201 Created``` response code and a **journals** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be6c4-131">例</span><span class="sxs-lookup"><span data-stu-id="be6c4-131">Example</span></span>

<span data-ttu-id="be6c4-132">**要求**</span><span class="sxs-lookup"><span data-stu-id="be6c4-132">**Request**</span></span>

<span data-ttu-id="be6c4-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="be6c4-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/journals
Content-type: application/json

```json
{
  "code": "DEFAULT"
}
```

<span data-ttu-id="be6c4-134">**応答**</span><span class="sxs-lookup"><span data-stu-id="be6c4-134">**Response**</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "DEFAULT",
  "displayName": "Default Journal Batch",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```

