---
title: 同期の既存のテンプレートを一覧表示します。
description: 特定のアプリケーションまたはサービス ・ プリンシパルに関連付けられている同期テンプレートを一覧表示します。
localization_priority: Normal
ms.openlocfilehash: 309d1ddd6d702652b14e10895de10486a5d23783
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523632"
---
# <a name="list-existing-synchronization-templates"></a><span data-ttu-id="13788-103">同期の既存のテンプレートを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="13788-103">List existing synchronization templates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13788-104">特定のアプリケーションまたはサービス ・ プリンシパルに関連付けられている同期テンプレートを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="13788-104">List the synchronization templates associated with a given application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="13788-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="13788-105">Permissions</span></span>
<span data-ttu-id="13788-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="13788-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13788-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="13788-108">Permission type</span></span>                        | <span data-ttu-id="13788-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="13788-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="13788-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="13788-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="13788-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13788-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="13788-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="13788-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="13788-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13788-113">Not supported.</span></span>|
|<span data-ttu-id="13788-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="13788-114">Application</span></span>                            |<span data-ttu-id="13788-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13788-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="13788-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="13788-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET servicePrincipals/{id}/synchronization/templates
GET applications/{id}/synchronization/templates
```

## <a name="request-headers"></a><span data-ttu-id="13788-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13788-117">Request headers</span></span>

| <span data-ttu-id="13788-118">名前</span><span class="sxs-lookup"><span data-stu-id="13788-118">Name</span></span>           | <span data-ttu-id="13788-119">型</span><span class="sxs-lookup"><span data-stu-id="13788-119">Type</span></span>    | <span data-ttu-id="13788-120">説明</span><span class="sxs-lookup"><span data-stu-id="13788-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="13788-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="13788-121">Authorization</span></span>  | <span data-ttu-id="13788-122">string</span><span class="sxs-lookup"><span data-stu-id="13788-122">string</span></span>  | <span data-ttu-id="13788-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="13788-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13788-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="13788-125">Request body</span></span>

<span data-ttu-id="13788-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="13788-126">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="13788-127">応答</span><span class="sxs-lookup"><span data-stu-id="13788-127">Response</span></span>

<span data-ttu-id="13788-128">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="13788-128">If successful, this method returns a `200 OK` response code and acollection of [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) objects in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="13788-129">例</span><span class="sxs-lookup"><span data-stu-id="13788-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="13788-130">要求</span><span class="sxs-lookup"><span data-stu-id="13788-130">Request</span></span>
<span data-ttu-id="13788-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="13788-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationtemplate"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates
```

##### <a name="response"></a><span data-ttu-id="13788-132">応答</span><span class="sxs-lookup"><span data-stu-id="13788-132">Response</span></span>
<span data-ttu-id="13788-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="13788-133">The following is an example of a response.</span></span>
><span data-ttu-id="13788-134">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="13788-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="13788-135">すべてのプロパティは、実際の呼び出しで返されます。</span><span class="sxs-lookup"><span data-stu-id="13788-135">All the properties will be returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
    "value": [
        {
            "id": "Slack",
            "factoryTag": "CustomSCIM",
            "schema": {
                    "directories": [],
                    "synchronizationRules": []
                    }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
