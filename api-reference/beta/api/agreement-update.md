---
title: 契約を更新する
description: アグリーメントオブジェクトのプロパティを更新します。
localization_priority: Normal
ms.openlocfilehash: fc6e4718a026f78a6e892dc13095492099b654cf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459319"
---
# <a name="update-agreement"></a><span data-ttu-id="37630-103">契約を更新する</span><span class="sxs-lookup"><span data-stu-id="37630-103">Update agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37630-104">[アグリーメント](../resources/agreement.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="37630-104">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="37630-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="37630-105">Permissions</span></span>
<span data-ttu-id="37630-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="37630-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37630-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="37630-108">Permission type</span></span>                        | <span data-ttu-id="37630-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="37630-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="37630-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="37630-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="37630-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37630-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="37630-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="37630-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37630-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37630-113">Not supported.</span></span> |
|<span data-ttu-id="37630-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="37630-114">Application</span></span>                            | <span data-ttu-id="37630-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37630-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="37630-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="37630-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="37630-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="37630-117">Request headers</span></span>
| <span data-ttu-id="37630-118">名前</span><span class="sxs-lookup"><span data-stu-id="37630-118">Name</span></span>         | <span data-ttu-id="37630-119">型</span><span class="sxs-lookup"><span data-stu-id="37630-119">Type</span></span>        | <span data-ttu-id="37630-120">説明</span><span class="sxs-lookup"><span data-stu-id="37630-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="37630-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="37630-121">Authorization</span></span> | <span data-ttu-id="37630-122">string</span><span class="sxs-lookup"><span data-stu-id="37630-122">string</span></span> | <span data-ttu-id="37630-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="37630-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="37630-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="37630-125">Request body</span></span>
<span data-ttu-id="37630-126">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="37630-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="37630-127">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="37630-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="37630-128">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="37630-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="37630-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="37630-129">Property</span></span>     | <span data-ttu-id="37630-130">型</span><span class="sxs-lookup"><span data-stu-id="37630-130">Type</span></span>        | <span data-ttu-id="37630-131">説明</span><span class="sxs-lookup"><span data-stu-id="37630-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="37630-132">displayName</span><span class="sxs-lookup"><span data-stu-id="37630-132">displayName</span></span>|<span data-ttu-id="37630-133">String</span><span class="sxs-lookup"><span data-stu-id="37630-133">String</span></span>|<span data-ttu-id="37630-134">アグリーメントの表示名。</span><span class="sxs-lookup"><span data-stu-id="37630-134">Display name of the agreement.</span></span>|
|<span data-ttu-id="37630-135">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="37630-135">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="37630-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="37630-136">Boolean</span></span>|<span data-ttu-id="37630-137">ユーザーが同意する前に、契約を展開して表示する必要があるかどうか。</span><span class="sxs-lookup"><span data-stu-id="37630-137">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="37630-138">応答</span><span class="sxs-lookup"><span data-stu-id="37630-138">Response</span></span>
<span data-ttu-id="37630-139">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[アグリーメント](../resources/agreement.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="37630-139">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="37630-140">例</span><span class="sxs-lookup"><span data-stu-id="37630-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="37630-141">要求</span><span class="sxs-lookup"><span data-stu-id="37630-141">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="37630-142">応答</span><span class="sxs-lookup"><span data-stu-id="37630-142">Response</span></span>
><span data-ttu-id="37630-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="37630-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Update agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/agreement-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
