---
title: 名前付きアイテムの追加
description: ユーザーのロケールを数式に使用して、新しい名前を指定したスコープのコレクションに追加します。
localization_priority: Normal
ms.openlocfilehash: 57ae84505327f2afbe2936b2671b655e76a85bd4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836702"
---
# <a name="add-named-item"></a><span data-ttu-id="b2398-103">名前付きアイテムの追加</span><span class="sxs-lookup"><span data-stu-id="b2398-103">Add Named Item</span></span>

> <span data-ttu-id="b2398-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b2398-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2398-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b2398-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b2398-106">ユーザーのロケールを数式に使用して、新しい名前を指定したスコープのコレクションに追加します。</span><span class="sxs-lookup"><span data-stu-id="b2398-106">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2398-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b2398-107">Permissions</span></span>
<span data-ttu-id="b2398-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b2398-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2398-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b2398-110">Permission type</span></span>      | <span data-ttu-id="b2398-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b2398-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2398-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b2398-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b2398-113">Files.ReadWrite、Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2398-113">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="b2398-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b2398-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2398-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b2398-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b2398-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b2398-116">Application</span></span> | <span data-ttu-id="b2398-117">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2398-117">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2398-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b2398-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="b2398-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b2398-119">Request headers</span></span>
| <span data-ttu-id="b2398-120">名前</span><span class="sxs-lookup"><span data-stu-id="b2398-120">Name</span></span>       | <span data-ttu-id="b2398-121">説明</span><span class="sxs-lookup"><span data-stu-id="b2398-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b2398-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2398-122">Authorization</span></span>  | <span data-ttu-id="b2398-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b2398-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b2398-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b2398-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="b2398-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="b2398-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2398-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="b2398-128">Request body</span></span>
<span data-ttu-id="b2398-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="b2398-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b2398-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b2398-130">Parameter</span></span>    | <span data-ttu-id="b2398-131">Type</span><span class="sxs-lookup"><span data-stu-id="b2398-131">Type</span></span>   |<span data-ttu-id="b2398-132">説明</span><span class="sxs-lookup"><span data-stu-id="b2398-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2398-133">name</span><span class="sxs-lookup"><span data-stu-id="b2398-133">name</span></span>|<span data-ttu-id="b2398-134">文字列</span><span class="sxs-lookup"><span data-stu-id="b2398-134">string</span></span>|<span data-ttu-id="b2398-135">名前付きの項目の名前。</span><span class="sxs-lookup"><span data-stu-id="b2398-135">The name of the named item.</span></span>|
|<span data-ttu-id="b2398-136">reference</span><span class="sxs-lookup"><span data-stu-id="b2398-136">reference</span></span>|<span data-ttu-id="b2398-137">文字列</span><span class="sxs-lookup"><span data-stu-id="b2398-137">string</span></span>|<span data-ttu-id="b2398-138">名前が参照する数式または範囲。</span><span class="sxs-lookup"><span data-stu-id="b2398-138">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="b2398-139">comment</span><span class="sxs-lookup"><span data-stu-id="b2398-139">comment</span></span>|<span data-ttu-id="b2398-140">文字列</span><span class="sxs-lookup"><span data-stu-id="b2398-140">string</span></span>|<span data-ttu-id="b2398-141">名前付きアイテムに関連付けられているコメント。</span><span class="sxs-lookup"><span data-stu-id="b2398-141">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="b2398-142">応答</span><span class="sxs-lookup"><span data-stu-id="b2398-142">Response</span></span>

<span data-ttu-id="b2398-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [NamedItem](../resources/nameditem.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b2398-143">If successful, this method returns `200 OK` response code and [NamedItem](../resources/nameditem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2398-144">例</span><span class="sxs-lookup"><span data-stu-id="b2398-144">Example</span></span>
<span data-ttu-id="b2398-145">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="b2398-145">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b2398-146">要求</span><span class="sxs-lookup"><span data-stu-id="b2398-146">Request</span></span>
<span data-ttu-id="b2398-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b2398-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/add
Content-type: application/json
Content-length: 54

{
  "name": "test5",
  "reference": "=Sheet1!$F$15:$N$27",
  "comment": "Comment for the named item"
}


```

##### <a name="response"></a><span data-ttu-id="b2398-148">応答</span><span class="sxs-lookup"><span data-stu-id="b2398-148">Response</span></span>
<span data-ttu-id="b2398-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b2398-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookNamedItem",
    "@odata.type": "#microsoft.graph.workbookNamedItem",
    "@odata.id": "/users('ca41eb6e-5828-486b-ab52-c3bd1f7a4047')/drive/root/workbook/names(%27test5%27)",
    "comment": "Comment for the named item",
    "name": "test5",
    "scope": "Workbook",
    "type": "Range",
    "value": "Sheet1!$F$15:$N$27",
    "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItemCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
