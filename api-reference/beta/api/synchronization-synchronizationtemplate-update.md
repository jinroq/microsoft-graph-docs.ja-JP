---
title: SynchronizationTemplate を更新します。
description: 特定のアプリケーションに関連付けられている同期の (上書き) のテンプレートを更新します。
localization_priority: Normal
ms.openlocfilehash: ea4dfdc418d04467a6060a8c3d7d83423ba16e38
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816738"
---
# <a name="update-synchronizationtemplate"></a><span data-ttu-id="b5f40-103">SynchronizationTemplate を更新します。</span><span class="sxs-lookup"><span data-stu-id="b5f40-103">Update synchronizationTemplate</span></span>

> <span data-ttu-id="b5f40-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b5f40-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5f40-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b5f40-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b5f40-106">特定のアプリケーションに関連付けられている同期の (上書き) のテンプレートを更新します。</span><span class="sxs-lookup"><span data-stu-id="b5f40-106">Update (override) the synchronization template associated with a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5f40-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b5f40-107">Permissions</span></span>
<span data-ttu-id="b5f40-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b5f40-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5f40-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b5f40-110">Permission type</span></span>                        | <span data-ttu-id="b5f40-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b5f40-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5f40-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b5f40-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="b5f40-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5f40-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="b5f40-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b5f40-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="b5f40-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b5f40-115">Not supported.</span></span>|
|<span data-ttu-id="b5f40-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b5f40-116">Application</span></span>                            |<span data-ttu-id="b5f40-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b5f40-117">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="b5f40-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b5f40-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT application/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="b5f40-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b5f40-119">Request headers</span></span>

| <span data-ttu-id="b5f40-120">名前</span><span class="sxs-lookup"><span data-stu-id="b5f40-120">Name</span></span>           | <span data-ttu-id="b5f40-121">種類</span><span class="sxs-lookup"><span data-stu-id="b5f40-121">Type</span></span>    | <span data-ttu-id="b5f40-122">説明</span><span class="sxs-lookup"><span data-stu-id="b5f40-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="b5f40-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5f40-123">Authorization</span></span>  | <span data-ttu-id="b5f40-124">string</span><span class="sxs-lookup"><span data-stu-id="b5f40-124">string</span></span>  | <span data-ttu-id="b5f40-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b5f40-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5f40-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b5f40-127">Request body</span></span>

<span data-ttu-id="b5f40-128">要求の本文には、既存のテンプレートを置換する[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="b5f40-128">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to replace the existing template.</span></span> <span data-ttu-id="b5f40-129">すべてのプロパティが用意されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="b5f40-129">Make sure all properties are provided.</span></span> <span data-ttu-id="b5f40-130">不足しているプロパティが消去されます。</span><span class="sxs-lookup"><span data-stu-id="b5f40-130">Missing properties will be erased.</span></span>

### <a name="response"></a><span data-ttu-id="b5f40-131">応答</span><span class="sxs-lookup"><span data-stu-id="b5f40-131">Response</span></span>

<span data-ttu-id="b5f40-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="b5f40-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="examples"></a><span data-ttu-id="b5f40-134">例</span><span class="sxs-lookup"><span data-stu-id="b5f40-134">Examples</span></span>

##### <a name="request"></a><span data-ttu-id="b5f40-135">要求</span><span class="sxs-lookup"><span data-stu-id="b5f40-135">Request</span></span>
<span data-ttu-id="b5f40-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b5f40-136">The following is an example of a request.</span></span> 

><span data-ttu-id="b5f40-137">**注:** ここで示すように、要求オブジェクトは、読みやすさの短縮されます。</span><span class="sxs-lookup"><span data-stu-id="b5f40-137">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="b5f40-138">実際の呼び出しですべてのプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="b5f40-138">Include all the properties in an actual call.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_synchronizationtemplate"
}-->
```http
PUT https://graph.microsoft.com/beta/applications/{id}/synchronization/templates/{templateId}
Authorization: Bearer <token>
Content-type: application/json

{
    "id": "Slack",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM"
}
```

##### <a name="response"></a><span data-ttu-id="b5f40-139">応答</span><span class="sxs-lookup"><span data-stu-id="b5f40-139">Response</span></span>
<span data-ttu-id="b5f40-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b5f40-140">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update synchronizationtemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
