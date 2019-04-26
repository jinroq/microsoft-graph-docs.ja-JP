---
title: コネクタグループの更新
description: コネクタグループオブジェクトのプロパティを更新します。
localization_priority: Normal
ms.openlocfilehash: df45006b57886bd3296d92d34d75de65e5bbec89
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327628"
---
# <a name="update-connectorgroups"></a><span data-ttu-id="2054e-103">コネクタグループの更新</span><span class="sxs-lookup"><span data-stu-id="2054e-103">Update connectorGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2054e-104">コネクタグループオブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2054e-104">Update the properties of connectorgroup object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2054e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2054e-105">Permissions</span></span>
<span data-ttu-id="2054e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2054e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2054e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2054e-108">Permission type</span></span>      | <span data-ttu-id="2054e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2054e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2054e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2054e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2054e-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2054e-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2054e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2054e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2054e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2054e-113">Not supported.</span></span>    |
|<span data-ttu-id="2054e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2054e-114">Application</span></span> | <span data-ttu-id="2054e-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2054e-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2054e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2054e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /connectorGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="2054e-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2054e-117">Optional request headers</span></span>
| <span data-ttu-id="2054e-118">名前</span><span class="sxs-lookup"><span data-stu-id="2054e-118">Name</span></span>       | <span data-ttu-id="2054e-119">説明</span><span class="sxs-lookup"><span data-stu-id="2054e-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2054e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2054e-120">Authorization</span></span>  | <span data-ttu-id="2054e-121">ベアラー.</span><span class="sxs-lookup"><span data-stu-id="2054e-121">Bearer.</span></span> <span data-ttu-id="2054e-122">必須</span><span class="sxs-lookup"><span data-stu-id="2054e-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="2054e-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="2054e-123">Request body</span></span>
<span data-ttu-id="2054e-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="2054e-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2054e-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2054e-127">Property</span></span>     | <span data-ttu-id="2054e-128">型</span><span class="sxs-lookup"><span data-stu-id="2054e-128">Type</span></span>   |<span data-ttu-id="2054e-129">説明</span><span class="sxs-lookup"><span data-stu-id="2054e-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2054e-130">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="2054e-130">connectorGroupType</span></span>|<span data-ttu-id="2054e-131">string</span><span class="sxs-lookup"><span data-stu-id="2054e-131">string</span></span>| <span data-ttu-id="2054e-132">可能な値は`applicationProxy`次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="2054e-132">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="2054e-133">name</span><span class="sxs-lookup"><span data-stu-id="2054e-133">name</span></span>|<span data-ttu-id="2054e-134">String</span><span class="sxs-lookup"><span data-stu-id="2054e-134">String</span></span>|<span data-ttu-id="2054e-135">コネクタグループの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="2054e-135">The name of the connectorGroup.</span></span>|

## <a name="response"></a><span data-ttu-id="2054e-136">応答</span><span class="sxs-lookup"><span data-stu-id="2054e-136">Response</span></span>

<span data-ttu-id="2054e-137">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[コネクタグループ](../resources/connectorgroup.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2054e-137">If successful, this method returns a `200 OK` response code and updated [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2054e-138">例</span><span class="sxs-lookup"><span data-stu-id="2054e-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2054e-139">要求</span><span class="sxs-lookup"><span data-stu-id="2054e-139">Request</span></span>
<span data-ttu-id="2054e-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2054e-140">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="2054e-141">応答</span><span class="sxs-lookup"><span data-stu-id="2054e-141">Response</span></span>
<span data-ttu-id="2054e-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2054e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update connectorgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
