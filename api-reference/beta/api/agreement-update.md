---
title: 契約を更新します。
description: 契約オブジェクトのプロパティを更新します。
ms.openlocfilehash: b9405a8c469876a349b5c1b0c00e6f6a5f225e72
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067411"
---
# <a name="update-agreement"></a><span data-ttu-id="0a58b-103">契約を更新します。</span><span class="sxs-lookup"><span data-stu-id="0a58b-103">Update agreement</span></span>

> <span data-ttu-id="0a58b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0a58b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a58b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a58b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0a58b-106">[契約](../resources/agreement.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0a58b-106">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0a58b-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0a58b-107">Permissions</span></span>
<span data-ttu-id="0a58b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0a58b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a58b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0a58b-110">Permission type</span></span>                        | <span data-ttu-id="0a58b-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0a58b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a58b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0a58b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0a58b-113">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a58b-113">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="0a58b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0a58b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a58b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a58b-115">Not supported.</span></span> |
|<span data-ttu-id="0a58b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0a58b-116">Application</span></span>                            | <span data-ttu-id="0a58b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a58b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a58b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0a58b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="0a58b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a58b-119">Request headers</span></span>
| <span data-ttu-id="0a58b-120">名前</span><span class="sxs-lookup"><span data-stu-id="0a58b-120">Name</span></span>         | <span data-ttu-id="0a58b-121">型</span><span class="sxs-lookup"><span data-stu-id="0a58b-121">Type</span></span>        | <span data-ttu-id="0a58b-122">説明</span><span class="sxs-lookup"><span data-stu-id="0a58b-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="0a58b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a58b-123">Authorization</span></span> | <span data-ttu-id="0a58b-124">string</span><span class="sxs-lookup"><span data-stu-id="0a58b-124">string</span></span> | <span data-ttu-id="0a58b-125">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="0a58b-125">Bearer \{token\}.</span></span> <span data-ttu-id="0a58b-126">必須。</span><span class="sxs-lookup"><span data-stu-id="0a58b-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a58b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0a58b-127">Request body</span></span>
<span data-ttu-id="0a58b-128">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="0a58b-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0a58b-129">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="0a58b-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0a58b-130">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="0a58b-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0a58b-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a58b-131">Property</span></span>     | <span data-ttu-id="0a58b-132">型</span><span class="sxs-lookup"><span data-stu-id="0a58b-132">Type</span></span>        | <span data-ttu-id="0a58b-133">説明</span><span class="sxs-lookup"><span data-stu-id="0a58b-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0a58b-134">displayName</span><span class="sxs-lookup"><span data-stu-id="0a58b-134">displayName</span></span>|<span data-ttu-id="0a58b-135">String</span><span class="sxs-lookup"><span data-stu-id="0a58b-135">String</span></span>|<span data-ttu-id="0a58b-136">契約書の名前を表示します。</span><span class="sxs-lookup"><span data-stu-id="0a58b-136">Display name of the agreement.</span></span>|
|<span data-ttu-id="0a58b-137">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="0a58b-137">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="0a58b-138">ブール値</span><span class="sxs-lookup"><span data-stu-id="0a58b-138">Boolean</span></span>|<span data-ttu-id="0a58b-139">ユーザーはあるかどうかを展開し、受け入れる前に契約書を表示します。</span><span class="sxs-lookup"><span data-stu-id="0a58b-139">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="0a58b-140">応答</span><span class="sxs-lookup"><span data-stu-id="0a58b-140">Response</span></span>
<span data-ttu-id="0a58b-141">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本体で[契約](../resources/agreement.md)の更新されたオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="0a58b-141">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0a58b-142">例</span><span class="sxs-lookup"><span data-stu-id="0a58b-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0a58b-143">要求</span><span class="sxs-lookup"><span data-stu-id="0a58b-143">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="0a58b-144">応答</span><span class="sxs-lookup"><span data-stu-id="0a58b-144">Response</span></span>
><span data-ttu-id="0a58b-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0a58b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
