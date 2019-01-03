---
title: ConnectorGroups を更新します。
description: Connectorgroup オブジェクトのプロパティを更新します。
ms.openlocfilehash: a9777394a3ecfc65a7c03c07643359ef3c763aca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066706"
---
# <a name="update-connectorgroups"></a><span data-ttu-id="2b8e5-103">ConnectorGroups を更新します。</span><span class="sxs-lookup"><span data-stu-id="2b8e5-103">Update connectorGroups</span></span>

> <span data-ttu-id="2b8e5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2b8e5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b8e5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b8e5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2b8e5-106">Connectorgroup オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2b8e5-106">Update the properties of connectorgroup object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2b8e5-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2b8e5-107">Permissions</span></span>
<span data-ttu-id="2b8e5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b8e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b8e5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2b8e5-110">Permission type</span></span>      | <span data-ttu-id="2b8e5-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2b8e5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b8e5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2b8e5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2b8e5-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2b8e5-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2b8e5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2b8e5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b8e5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b8e5-115">Not supported.</span></span>    |
|<span data-ttu-id="2b8e5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2b8e5-116">Application</span></span> | <span data-ttu-id="2b8e5-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b8e5-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b8e5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2b8e5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /connectorGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="2b8e5-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2b8e5-119">Optional request headers</span></span>
| <span data-ttu-id="2b8e5-120">名前</span><span class="sxs-lookup"><span data-stu-id="2b8e5-120">Name</span></span>       | <span data-ttu-id="2b8e5-121">説明</span><span class="sxs-lookup"><span data-stu-id="2b8e5-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2b8e5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b8e5-122">Authorization</span></span>  | <span data-ttu-id="2b8e5-123">ベアラーです。</span><span class="sxs-lookup"><span data-stu-id="2b8e5-123">Bearer.</span></span> <span data-ttu-id="2b8e5-124">必須</span><span class="sxs-lookup"><span data-stu-id="2b8e5-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b8e5-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="2b8e5-125">Request body</span></span>
<span data-ttu-id="2b8e5-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="2b8e5-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2b8e5-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b8e5-129">Property</span></span>     | <span data-ttu-id="2b8e5-130">型</span><span class="sxs-lookup"><span data-stu-id="2b8e5-130">Type</span></span>   |<span data-ttu-id="2b8e5-131">説明</span><span class="sxs-lookup"><span data-stu-id="2b8e5-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b8e5-132">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="2b8e5-132">connectorGroupType</span></span>|<span data-ttu-id="2b8e5-133">文字列</span><span class="sxs-lookup"><span data-stu-id="2b8e5-133">string</span></span>| <span data-ttu-id="2b8e5-134">使用可能な値: `applicationProxy`。</span><span class="sxs-lookup"><span data-stu-id="2b8e5-134">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="2b8e5-135">名前</span><span class="sxs-lookup"><span data-stu-id="2b8e5-135">name</span></span>|<span data-ttu-id="2b8e5-136">String</span><span class="sxs-lookup"><span data-stu-id="2b8e5-136">String</span></span>|<span data-ttu-id="2b8e5-137">ConnectorGroup の名前です。</span><span class="sxs-lookup"><span data-stu-id="2b8e5-137">The name of the connectorGroup.</span></span>|

## <a name="response"></a><span data-ttu-id="2b8e5-138">応答</span><span class="sxs-lookup"><span data-stu-id="2b8e5-138">Response</span></span>

<span data-ttu-id="2b8e5-139">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の更新された[connectorGroup](../resources/connectorgroup.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="2b8e5-139">If successful, this method returns a `200 OK` response code and updated [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2b8e5-140">例</span><span class="sxs-lookup"><span data-stu-id="2b8e5-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b8e5-141">要求</span><span class="sxs-lookup"><span data-stu-id="2b8e5-141">Request</span></span>
<span data-ttu-id="2b8e5-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2b8e5-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_connectorgroup"
}-->
```http
PATCH https://graph.microsoft.com/{ver}/connectorGroups/{id}
Content-type: application/json
Content-length: 99

{
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
}
```
##### <a name="response"></a><span data-ttu-id="2b8e5-143">応答</span><span class="sxs-lookup"><span data-stu-id="2b8e5-143">Response</span></span>
<span data-ttu-id="2b8e5-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2b8e5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 119

{
  "id": "id-value",
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update connectorgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->