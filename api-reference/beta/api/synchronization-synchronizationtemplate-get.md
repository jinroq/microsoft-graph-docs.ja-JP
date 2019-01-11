---
title: SynchronizationTemplate を取得します。
description: Id によって同期テンプレートを取得します。
localization_priority: Normal
ms.openlocfilehash: 9754b1fbc8c86f05d22f0ada57b8b97e0b1efbed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863813"
---
# <a name="get-synchronizationtemplate"></a><span data-ttu-id="e82ec-103">SynchronizationTemplate を取得します。</span><span class="sxs-lookup"><span data-stu-id="e82ec-103">Get synchronizationTemplate</span></span>

> <span data-ttu-id="e82ec-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e82ec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e82ec-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e82ec-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e82ec-106">Id によって同期テンプレートを取得します。</span><span class="sxs-lookup"><span data-stu-id="e82ec-106">Retrieve a synchronization template by its identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="e82ec-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e82ec-107">Permissions</span></span>
<span data-ttu-id="e82ec-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e82ec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e82ec-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e82ec-110">Permission type</span></span>                        | <span data-ttu-id="e82ec-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e82ec-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e82ec-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e82ec-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="e82ec-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e82ec-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="e82ec-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e82ec-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="e82ec-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e82ec-115">Not supported.</span></span>|
|<span data-ttu-id="e82ec-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e82ec-116">Application</span></span>                            |<span data-ttu-id="e82ec-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e82ec-117">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="e82ec-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e82ec-118">HTTP Request</span></span>

```http
GET applications/{id}/synchronization/templates/{templateId}
GET servicePrincipals/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="e82ec-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e82ec-119">Request headers</span></span>

| <span data-ttu-id="e82ec-120">名前</span><span class="sxs-lookup"><span data-stu-id="e82ec-120">Name</span></span>           | <span data-ttu-id="e82ec-121">種類</span><span class="sxs-lookup"><span data-stu-id="e82ec-121">Type</span></span>    | <span data-ttu-id="e82ec-122">説明</span><span class="sxs-lookup"><span data-stu-id="e82ec-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="e82ec-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e82ec-123">Authorization</span></span>  | <span data-ttu-id="e82ec-124">string</span><span class="sxs-lookup"><span data-stu-id="e82ec-124">string</span></span>  | <span data-ttu-id="e82ec-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e82ec-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e82ec-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e82ec-127">Request body</span></span>

<span data-ttu-id="e82ec-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e82ec-128">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="e82ec-129">応答</span><span class="sxs-lookup"><span data-stu-id="e82ec-129">Response</span></span>

<span data-ttu-id="e82ec-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="e82ec-130">If successful, this method returns a `200 OK` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="e82ec-131">例</span><span class="sxs-lookup"><span data-stu-id="e82ec-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e82ec-132">要求</span><span class="sxs-lookup"><span data-stu-id="e82ec-132">Request</span></span>
<span data-ttu-id="e82ec-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e82ec-133">The following is an example of a request.</span></span>

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates/Slack
```

##### <a name="response"></a><span data-ttu-id="e82ec-134">応答</span><span class="sxs-lookup"><span data-stu-id="e82ec-134">Response</span></span>
<span data-ttu-id="e82ec-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e82ec-135">The following is an example of a response.</span></span>
><span data-ttu-id="e82ec-136">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="e82ec-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e82ec-137">すべてのプロパティは、実際の呼び出しで返されます。</span><span class="sxs-lookup"><span data-stu-id="e82ec-137">All the properties will be returned in an actual call.</span></span>

```http
HTTP/1.1 200 OK
{
    "id": "Slack",
    "factoryTag": "CustomSCIM",
    "schema": {
        "directories": [],
        "synchronizationRules": []
        }
}
```
