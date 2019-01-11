---
title: 契約を更新します。
description: 契約オブジェクトのプロパティを更新します。
localization_priority: Normal
ms.openlocfilehash: b16a503b33193fa453ca52481854879ae4dcd121
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838732"
---
# <a name="update-agreement"></a><span data-ttu-id="6fa44-103">契約を更新します。</span><span class="sxs-lookup"><span data-stu-id="6fa44-103">Update agreement</span></span>

> <span data-ttu-id="6fa44-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6fa44-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6fa44-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6fa44-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6fa44-106">[契約](../resources/agreement.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6fa44-106">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6fa44-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6fa44-107">Permissions</span></span>
<span data-ttu-id="6fa44-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6fa44-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fa44-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6fa44-110">Permission type</span></span>                        | <span data-ttu-id="6fa44-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6fa44-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6fa44-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6fa44-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6fa44-113">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fa44-113">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="6fa44-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6fa44-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fa44-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6fa44-115">Not supported.</span></span> |
|<span data-ttu-id="6fa44-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6fa44-116">Application</span></span>                            | <span data-ttu-id="6fa44-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6fa44-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6fa44-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6fa44-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="6fa44-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6fa44-119">Request headers</span></span>
| <span data-ttu-id="6fa44-120">名前</span><span class="sxs-lookup"><span data-stu-id="6fa44-120">Name</span></span>         | <span data-ttu-id="6fa44-121">種類</span><span class="sxs-lookup"><span data-stu-id="6fa44-121">Type</span></span>        | <span data-ttu-id="6fa44-122">説明</span><span class="sxs-lookup"><span data-stu-id="6fa44-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="6fa44-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fa44-123">Authorization</span></span> | <span data-ttu-id="6fa44-124">string</span><span class="sxs-lookup"><span data-stu-id="6fa44-124">string</span></span> | <span data-ttu-id="6fa44-125">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="6fa44-125">Bearer \{token\}.</span></span> <span data-ttu-id="6fa44-126">必須。</span><span class="sxs-lookup"><span data-stu-id="6fa44-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6fa44-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="6fa44-127">Request body</span></span>
<span data-ttu-id="6fa44-128">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="6fa44-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6fa44-129">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="6fa44-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6fa44-130">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="6fa44-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6fa44-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6fa44-131">Property</span></span>     | <span data-ttu-id="6fa44-132">種類</span><span class="sxs-lookup"><span data-stu-id="6fa44-132">Type</span></span>        | <span data-ttu-id="6fa44-133">説明</span><span class="sxs-lookup"><span data-stu-id="6fa44-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6fa44-134">displayName</span><span class="sxs-lookup"><span data-stu-id="6fa44-134">displayName</span></span>|<span data-ttu-id="6fa44-135">String</span><span class="sxs-lookup"><span data-stu-id="6fa44-135">String</span></span>|<span data-ttu-id="6fa44-136">契約書の名前を表示します。</span><span class="sxs-lookup"><span data-stu-id="6fa44-136">Display name of the agreement.</span></span>|
|<span data-ttu-id="6fa44-137">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="6fa44-137">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="6fa44-138">ブール型</span><span class="sxs-lookup"><span data-stu-id="6fa44-138">Boolean</span></span>|<span data-ttu-id="6fa44-139">ユーザーはあるかどうかを展開し、受け入れる前に契約書を表示します。</span><span class="sxs-lookup"><span data-stu-id="6fa44-139">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="6fa44-140">応答</span><span class="sxs-lookup"><span data-stu-id="6fa44-140">Response</span></span>
<span data-ttu-id="6fa44-141">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本体で[契約](../resources/agreement.md)の更新されたオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="6fa44-141">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6fa44-142">例</span><span class="sxs-lookup"><span data-stu-id="6fa44-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6fa44-143">要求</span><span class="sxs-lookup"><span data-stu-id="6fa44-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_agreement"
}-->
```http
PATCH https://graph.microsoft.com/beta/agreements/<id>
Content-type: application/json
Content-length: 85

{
  "displayName": "displayName-value",
  "isViewingBeforeAcceptanceRequired": true
}
```
##### <a name="response"></a><span data-ttu-id="6fa44-144">応答</span><span class="sxs-lookup"><span data-stu-id="6fa44-144">Response</span></span>
><span data-ttu-id="6fa44-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6fa44-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 105

{
  "displayName": "displayName-value",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
