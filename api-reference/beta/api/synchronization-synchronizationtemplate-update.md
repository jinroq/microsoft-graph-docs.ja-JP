---
title: SynchronizationTemplate を更新します。
description: 特定のアプリケーションに関連付けられている同期の (上書き) のテンプレートを更新します。
localization_priority: Normal
ms.openlocfilehash: 152186afd9f7b7cce2a04170de7148d454525d80
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517464"
---
# <a name="update-synchronizationtemplate"></a><span data-ttu-id="39669-103">SynchronizationTemplate を更新します。</span><span class="sxs-lookup"><span data-stu-id="39669-103">Update synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39669-104">特定のアプリケーションに関連付けられている同期の (上書き) のテンプレートを更新します。</span><span class="sxs-lookup"><span data-stu-id="39669-104">Update (override) the synchronization template associated with a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="39669-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="39669-105">Permissions</span></span>
<span data-ttu-id="39669-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="39669-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39669-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="39669-108">Permission type</span></span>                        | <span data-ttu-id="39669-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="39669-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="39669-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="39669-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="39669-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39669-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="39669-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="39669-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="39669-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="39669-113">Not supported.</span></span>|
|<span data-ttu-id="39669-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="39669-114">Application</span></span>                            |<span data-ttu-id="39669-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="39669-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="39669-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="39669-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT application/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="39669-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="39669-117">Request headers</span></span>

| <span data-ttu-id="39669-118">名前</span><span class="sxs-lookup"><span data-stu-id="39669-118">Name</span></span>           | <span data-ttu-id="39669-119">型</span><span class="sxs-lookup"><span data-stu-id="39669-119">Type</span></span>    | <span data-ttu-id="39669-120">説明</span><span class="sxs-lookup"><span data-stu-id="39669-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="39669-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="39669-121">Authorization</span></span>  | <span data-ttu-id="39669-122">string</span><span class="sxs-lookup"><span data-stu-id="39669-122">string</span></span>  | <span data-ttu-id="39669-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="39669-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="39669-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="39669-125">Request body</span></span>

<span data-ttu-id="39669-126">要求の本文には、既存のテンプレートを置換する[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="39669-126">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to replace the existing template.</span></span> <span data-ttu-id="39669-127">すべてのプロパティが用意されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="39669-127">Make sure all properties are provided.</span></span> <span data-ttu-id="39669-128">不足しているプロパティが消去されます。</span><span class="sxs-lookup"><span data-stu-id="39669-128">Missing properties will be erased.</span></span>

### <a name="response"></a><span data-ttu-id="39669-129">応答</span><span class="sxs-lookup"><span data-stu-id="39669-129">Response</span></span>

<span data-ttu-id="39669-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="39669-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="examples"></a><span data-ttu-id="39669-132">例</span><span class="sxs-lookup"><span data-stu-id="39669-132">Examples</span></span>

##### <a name="request"></a><span data-ttu-id="39669-133">要求</span><span class="sxs-lookup"><span data-stu-id="39669-133">Request</span></span>
<span data-ttu-id="39669-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="39669-134">The following is an example of a request.</span></span> 

><span data-ttu-id="39669-135">**注:** ここで示すように、要求オブジェクトは、読みやすさの短縮されます。</span><span class="sxs-lookup"><span data-stu-id="39669-135">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="39669-136">実際の呼び出しですべてのプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="39669-136">Include all the properties in an actual call.</span></span>
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

##### <a name="response"></a><span data-ttu-id="39669-137">応答</span><span class="sxs-lookup"><span data-stu-id="39669-137">Response</span></span>
<span data-ttu-id="39669-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="39669-138">The following is an example of a response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update synchronizationtemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
