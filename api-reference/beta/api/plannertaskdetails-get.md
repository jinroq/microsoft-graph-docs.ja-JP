---
title: Get plannerTaskDetails
description: '**plannertaskdetails** オブジェクトのプロパティと関係を取得します。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 813f6ae2cdeac0e3b3797e7abdfc435d5bbb4a71
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975626"
---
# <a name="get-plannertaskdetails"></a><span data-ttu-id="7455c-103">Get plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="7455c-103">Get plannerTaskDetails</span></span>

> <span data-ttu-id="7455c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7455c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7455c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7455c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7455c-106">**plannertaskdetails** オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="7455c-106">Retrieve the properties and relationships of **plannertaskdetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7455c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7455c-107">Permissions</span></span>
<span data-ttu-id="7455c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7455c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7455c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7455c-110">Permission type</span></span>      | <span data-ttu-id="7455c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7455c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7455c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7455c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7455c-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7455c-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7455c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7455c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7455c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7455c-115">Not supported.</span></span>    |
|<span data-ttu-id="7455c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7455c-116">Application</span></span> | <span data-ttu-id="7455c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7455c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7455c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7455c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/<id>/details
```

## <a name="request-headers"></a><span data-ttu-id="7455c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7455c-119">Request headers</span></span>
| <span data-ttu-id="7455c-120">名前</span><span class="sxs-lookup"><span data-stu-id="7455c-120">Name</span></span>      |<span data-ttu-id="7455c-121">説明</span><span class="sxs-lookup"><span data-stu-id="7455c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7455c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7455c-122">Authorization</span></span>  | <span data-ttu-id="7455c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7455c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7455c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="7455c-125">Request body</span></span>
<span data-ttu-id="7455c-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7455c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7455c-127">応答</span><span class="sxs-lookup"><span data-stu-id="7455c-127">Response</span></span>

<span data-ttu-id="7455c-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [plannerTaskDetails](../resources/plannertaskdetails.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7455c-128">If successful, this method returns a `200 OK` response code and [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.</span></span>

<span data-ttu-id="7455c-p104">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7455c-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="7455c-132">例</span><span class="sxs-lookup"><span data-stu-id="7455c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7455c-133">要求</span><span class="sxs-lookup"><span data-stu-id="7455c-133">Request</span></span>
<span data-ttu-id="7455c-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7455c-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannertaskdetails"
}-->
```http
GET https://graph.microsoft.com/beta/planner/tasks/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/details
```
##### <a name="response"></a><span data-ttu-id="7455c-135">応答</span><span class="sxs-lookup"><span data-stu-id="7455c-135">Response</span></span>
<span data-ttu-id="7455c-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7455c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTaskDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1036

{
  "description": "Task details properties:\nchecklist:Sub items\nreferences:Related links",
  "previewType": "automatic",
  "references": {
    "https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer": {
      "@odata.type": "#microsoft.graph.plannerExternalReference",
      "alias": "Graph Explorer",
      "type": "Other",
      "previewPriority": "0009005706180391122",
      "lastModifiedBy": {
        "user": {
          "id": "fbab97d0-4932-4511-b675-204639209557"
        }
      },
      "lastModifiedDateTime": "2017-04-24T22:52:29.814Z"
    }
  },
  "checklist": {
    "d280ed1a-9f6b-4f9c-a962-fb4d00dc50ff": {
      "@odata.type": "#microsoft.graph.plannerChecklistItem",
      "isChecked": false,
      "title": "Try reading task details",
      "orderHint": "8587094707721254251P]",
      "lastModifiedBy": {
        "user": {
          "id": "e396de0e-4812-4fcb-9f9e-0358744df343"
        }
      },
      "lastModifiedDateTime": "2017-04-14T02:16:14.866Z"
    }
  },
  "id": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerTaskDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
