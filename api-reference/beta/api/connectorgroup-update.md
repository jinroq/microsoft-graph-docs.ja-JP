---
title: ConnectorGroups を更新します。
description: Connectorgroup オブジェクトのプロパティを更新します。
localization_priority: Normal
ms.openlocfilehash: 9d6feec19552aeeebe51ba0fab07e805c6f4a2bb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530112"
---
# <a name="update-connectorgroups"></a><span data-ttu-id="98108-103">ConnectorGroups を更新します。</span><span class="sxs-lookup"><span data-stu-id="98108-103">Update connectorGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98108-104">Connectorgroup オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="98108-104">Update the properties of connectorgroup object.</span></span>
## <a name="permissions"></a><span data-ttu-id="98108-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="98108-105">Permissions</span></span>
<span data-ttu-id="98108-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="98108-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98108-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="98108-108">Permission type</span></span>      | <span data-ttu-id="98108-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="98108-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98108-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="98108-110">Delegated (work or school account)</span></span> | <span data-ttu-id="98108-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="98108-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="98108-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="98108-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98108-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="98108-113">Not supported.</span></span>    |
|<span data-ttu-id="98108-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="98108-114">Application</span></span> | <span data-ttu-id="98108-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98108-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="98108-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="98108-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /connectorGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="98108-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="98108-117">Optional request headers</span></span>
| <span data-ttu-id="98108-118">名前</span><span class="sxs-lookup"><span data-stu-id="98108-118">Name</span></span>       | <span data-ttu-id="98108-119">説明</span><span class="sxs-lookup"><span data-stu-id="98108-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="98108-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="98108-120">Authorization</span></span>  | <span data-ttu-id="98108-121">Bearer </span><span class="sxs-lookup"><span data-stu-id="98108-121">Bearer.</span></span> <span data-ttu-id="98108-122">必須</span><span class="sxs-lookup"><span data-stu-id="98108-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="98108-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="98108-123">Request body</span></span>
<span data-ttu-id="98108-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="98108-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="98108-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="98108-127">Property</span></span>     | <span data-ttu-id="98108-128">型</span><span class="sxs-lookup"><span data-stu-id="98108-128">Type</span></span>   |<span data-ttu-id="98108-129">説明</span><span class="sxs-lookup"><span data-stu-id="98108-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98108-130">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="98108-130">connectorGroupType</span></span>|<span data-ttu-id="98108-131">string</span><span class="sxs-lookup"><span data-stu-id="98108-131">string</span></span>| <span data-ttu-id="98108-132">使用可能な値: `applicationProxy`。</span><span class="sxs-lookup"><span data-stu-id="98108-132">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="98108-133">name</span><span class="sxs-lookup"><span data-stu-id="98108-133">name</span></span>|<span data-ttu-id="98108-134">String</span><span class="sxs-lookup"><span data-stu-id="98108-134">String</span></span>|<span data-ttu-id="98108-135">ConnectorGroup の名前です。</span><span class="sxs-lookup"><span data-stu-id="98108-135">The name of the connectorGroup.</span></span>|

## <a name="response"></a><span data-ttu-id="98108-136">応答</span><span class="sxs-lookup"><span data-stu-id="98108-136">Response</span></span>

<span data-ttu-id="98108-137">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の更新された[connectorGroup](../resources/connectorgroup.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="98108-137">If successful, this method returns a `200 OK` response code and updated [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="98108-138">例</span><span class="sxs-lookup"><span data-stu-id="98108-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="98108-139">要求</span><span class="sxs-lookup"><span data-stu-id="98108-139">Request</span></span>
<span data-ttu-id="98108-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="98108-140">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="98108-141">応答</span><span class="sxs-lookup"><span data-stu-id="98108-141">Response</span></span>
<span data-ttu-id="98108-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="98108-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/connectorgroup-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
