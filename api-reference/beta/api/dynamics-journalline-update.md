---
title: JournalLines の更新
description: Dynamics 365 Business Central の仕訳帳明細行を更新します。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: aa5f11574769e1a9b171353dd27afb5ef02e5ea1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956108"
---
# <a name="update-journallines"></a><span data-ttu-id="08886-103">JournalLines の更新</span><span class="sxs-lookup"><span data-stu-id="08886-103">Update journalLines</span></span>
<span data-ttu-id="08886-104">Dynamics 365 Business Central の journal 明細行オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="08886-104">Update the properties of a journal lines object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="08886-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="08886-105">Permissions</span></span>
<span data-ttu-id="08886-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="08886-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08886-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="08886-108">Permission type</span></span> |<span data-ttu-id="08886-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="08886-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="08886-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="08886-110">Delegated (work or school account)</span></span>|<span data-ttu-id="08886-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08886-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="08886-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="08886-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="08886-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08886-113">Not supported.</span></span>|
|<span data-ttu-id="08886-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="08886-114">Application</span></span>|<span data-ttu-id="08886-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08886-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08886-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="08886-116">HTTP request</span></span>

```
PATCH /financials/companies('{id}')/journals('{id}')/journalLines('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="08886-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="08886-117">Optional query parameters</span></span>
<span data-ttu-id="08886-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="08886-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="08886-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="08886-119">Request headers</span></span>
| <span data-ttu-id="08886-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="08886-120">Header</span></span>       | <span data-ttu-id="08886-121">値</span><span class="sxs-lookup"><span data-stu-id="08886-121">Value</span></span>                    |
|--------------|--------------------------|
|<span data-ttu-id="08886-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="08886-122">Authorization</span></span> |<span data-ttu-id="08886-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="08886-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="08886-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="08886-125">Content-Type</span></span>  |<span data-ttu-id="08886-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08886-126">application/json</span></span>          |
|<span data-ttu-id="08886-127">If-Match</span><span class="sxs-lookup"><span data-stu-id="08886-127">If-Match</span></span>      |<span data-ttu-id="08886-128">必須です。</span><span class="sxs-lookup"><span data-stu-id="08886-128">Required.</span></span> <span data-ttu-id="08886-129">この要求ヘッダーが含まれていて、指定された eTag が**journalLines**の現在のタグと一致しない場合、 **journalLines**は更新されません。</span><span class="sxs-lookup"><span data-stu-id="08886-129">When this request header is included and the eTag provided does not match the current tag on the **journalLines**, the **journalLines** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08886-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="08886-130">Request body</span></span>
<span data-ttu-id="08886-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="08886-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="08886-134">応答</span><span class="sxs-lookup"><span data-stu-id="08886-134">Response</span></span>
<span data-ttu-id="08886-135">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された**journalLines**オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="08886-135">If successful, this method returns a `200 OK` response code and an updated **journalLines** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08886-136">例</span><span class="sxs-lookup"><span data-stu-id="08886-136">Example</span></span>

<span data-ttu-id="08886-137">**要求**</span><span class="sxs-lookup"><span data-stu-id="08886-137">**Request**</span></span>

<span data-ttu-id="08886-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="08886-138">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies('{id}')/journals('{id}')/journalLines('{id}')
Content-type: application/json

{
  "amount": 2000
}
```

<span data-ttu-id="08886-139">**応答**</span><span class="sxs-lookup"><span data-stu-id="08886-139">**Response**</span></span>

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "journalDisplayName": "DEFAULT",
  "lineNumber": 10000,
  "accountId": "",
  "accountNumber": "",
  "postingDate": "2015-12-31",
  "documentNumber": "D00001",
  "externalDocumentNumber": "",
  "amount": 2000,
  "description": "",
  "comment": "",
  "lastModifiedDateTime": "2017-03-17T19:02:22.043Z"
}
```


