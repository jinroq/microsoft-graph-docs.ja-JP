---
title: secureScores のリスト
description: プロパティと、secureScores オブジェクトの関係を取得します。
localization_priority: Normal
ms.openlocfilehash: 034a333dec6b96919ffd01a49ed05cb16ca19a48
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573404"
---
# <a name="list-securescores"></a><span data-ttu-id="bc821-103">secureScores のリスト</span><span class="sxs-lookup"><span data-stu-id="bc821-103">List secureScores</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc821-104">プロパティと、 [secureScores](../resources/securescores.md)オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="bc821-104">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc821-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bc821-105">Permissions</span></span>

<span data-ttu-id="bc821-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bc821-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc821-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bc821-108">Permission type</span></span>      | <span data-ttu-id="bc821-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bc821-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc821-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bc821-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="bc821-111">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="bc821-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="bc821-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bc821-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="bc821-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc821-113">Not supported.</span></span>  |
|<span data-ttu-id="bc821-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bc821-114">Application</span></span> | <span data-ttu-id="bc821-115">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="bc821-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc821-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bc821-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="bc821-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bc821-117">Request headers</span></span>

| <span data-ttu-id="bc821-118">名前</span><span class="sxs-lookup"><span data-stu-id="bc821-118">Name</span></span>      |<span data-ttu-id="bc821-119">説明</span><span class="sxs-lookup"><span data-stu-id="bc821-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bc821-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc821-120">Authorization</span></span>  | <span data-ttu-id="bc821-p102">Bearer {code}。必須。</span><span class="sxs-lookup"><span data-stu-id="bc821-p102">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc821-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="bc821-123">Request body</span></span>

<span data-ttu-id="bc821-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bc821-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc821-125">応答</span><span class="sxs-lookup"><span data-stu-id="bc821-125">Response</span></span>

<span data-ttu-id="bc821-126">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に**secureScores**オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="bc821-126">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc821-127">例</span><span class="sxs-lookup"><span data-stu-id="bc821-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc821-128">要求</span><span class="sxs-lookup"><span data-stu-id="bc821-128">Request</span></span>

<span data-ttu-id="bc821-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bc821-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```

### <a name="response"></a><span data-ttu-id="bc821-130">応答</span><span class="sxs-lookup"><span data-stu-id="bc821-130">Response</span></span>

<span data-ttu-id="bc821-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bc821-131">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.secureScore"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "activeUserCount": 12,
            "createdDate": "createdDateTime.value",
            "currentScore": 12.4566633444,
            "enabledServices": ["Skype"],
            "licensedUserCount": 12,
            "maxScore": 45.2324443,
            "id": "id.value",            
            "azureTenantId": "azureTenantId.value",
            "averageComparativeScores": [
                {
                    "@odata.type":"microsoft.graph.averageComparativeScores",
                    "basis": "basis.value",
                    "averageScore": 34.2324443
                },
                {
                    "@odata.type":"microsoft.graph.averageComparativeScores",
                    "basis": "basis.value",
                    "averageScore": 34.2324443
                },
                {
                    "@odata.type":"microsoft.graph.averageComparativeScores",
                    "basis": "basis.value",
                    "averageScore": 34.2324443
                }
            ],
            "controlScores": [
                {
                    "@odata.type":"microsoft.graph.controlScores",
                    "controlCategory": "controlCategory.value",
                    "controlName": "controlName.value",
                    "description": "description.value",
                    "score": "score.value",
                    "total": "total.value",
                    "count": "count.value"
                }
            ]
        }
    ]
}

```


<!--
{
  "type": "#page.annotation",
  "description": "List secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/securescores-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
