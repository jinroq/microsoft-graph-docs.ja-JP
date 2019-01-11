---
title: リスト educationAssignmentResources
description: この割り当てに関連付けられているすべてのリソースを取得します。
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: 650d731883a7cde8bc05ec50889be472bb0967a2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823892"
---
# <a name="list-educationassignmentresources"></a><span data-ttu-id="a62fc-103">リスト educationAssignmentResources</span><span class="sxs-lookup"><span data-stu-id="a62fc-103">List educationAssignmentResources</span></span>

> <span data-ttu-id="a62fc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a62fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a62fc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a62fc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a62fc-106">この割り当てに関連付けられているすべてのリソースを取得します。</span><span class="sxs-lookup"><span data-stu-id="a62fc-106">Get all the resources associated with this assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="a62fc-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a62fc-107">Permissions</span></span>
<span data-ttu-id="a62fc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a62fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a62fc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a62fc-110">Permission type</span></span>      | <span data-ttu-id="a62fc-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a62fc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a62fc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a62fc-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="a62fc-113">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a62fc-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="a62fc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a62fc-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a62fc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a62fc-115">Not supported.</span></span>  |
|<span data-ttu-id="a62fc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a62fc-116">Application</span></span> | <span data-ttu-id="a62fc-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a62fc-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a62fc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a62fc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a62fc-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a62fc-119">Optional query parameters</span></span>
<span data-ttu-id="a62fc-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a62fc-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a62fc-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a62fc-121">Request headers</span></span>
| <span data-ttu-id="a62fc-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a62fc-122">Header</span></span>       | <span data-ttu-id="a62fc-123">値</span><span class="sxs-lookup"><span data-stu-id="a62fc-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a62fc-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a62fc-124">Authorization</span></span>  | <span data-ttu-id="a62fc-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a62fc-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a62fc-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a62fc-127">Request body</span></span>
<span data-ttu-id="a62fc-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a62fc-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a62fc-129">応答</span><span class="sxs-lookup"><span data-stu-id="a62fc-129">Response</span></span>
<span data-ttu-id="a62fc-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[educationAssignmentResource](../resources/educationassignmentresource.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="a62fc-130">If successful, this method returns a `200 OK` response code and a collection of [educationAssignmentResource](../resources/educationassignmentresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a62fc-131">例</span><span class="sxs-lookup"><span data-stu-id="a62fc-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a62fc-132">要求</span><span class="sxs-lookup"><span data-stu-id="a62fc-132">Request</span></span>
<span data-ttu-id="a62fc-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a62fc-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_resources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/resources
```
##### <a name="response"></a><span data-ttu-id="a62fc-134">応答</span><span class="sxs-lookup"><span data-stu-id="a62fc-134">Response</span></span>
<span data-ttu-id="a62fc-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a62fc-135">The following is an example of the response.</span></span> 

><span data-ttu-id="a62fc-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a62fc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1011

{
  "value": [
    {
      "distributeForStudentWork": false,
      "resource": {
          "@odata.type": "#microsoft.graph.educationLinkResource",
          "displayName": "Microsoft Homepage",
          "createdDateTime": "2017-10-21T07:52:45.5675913Z",
          "createdBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "lastModifiedDateTime": "2017-10-21T07:52:45.5675913Z",
          "lastModifiedBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "link": "https://www.microsoft.com"
      },
      "id": "850f51b7-1df9-4ec0-bd62-64a0214b9cbf"
    },
    {
      "distributeForStudentWork": true,
      "resource": {
          "@odata.type": "#microsoft.graph.educationWordResource",
          "displayName": "Report.docx",
          "createdDateTime": "2017-10-21T07:52:53.9863696Z",
          "createdBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "lastModifiedDateTime": "2017-10-21T07:52:53.9863696Z",
          "lastModifiedBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeTZ_iul5AdW9f/items/017NJZI27BCN2QI2H7HJGLIVPXR6SD2DH6"
      },
      "id": "f2387c3b-ec39-4bf2-a399-d7242677f024"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List resources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
