---
title: リソースを一覧表示する
description: この送信に関連付けられているリソースを一覧表示します。 **提出リソース**オブジェクトは、学生が作業している実際のリソースオブジェクトをラップしたものです。 このラッパーには、割り当て処理中に割り当てからコピーされた場合に、割り当てのリソースへのポインターも含まれています。 これらのリソースは、割り当ての作業コピーです。 **Submittedresources**は、正式に送信され、採点されるリソースです。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 51a70d3554ea0dac3c5e3487bb9f9dab88addba2
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "34749969"
---
# <a name="list-resources"></a><span data-ttu-id="9b99f-107">リソースを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="9b99f-107">List resources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b99f-108">この送信に関連付けられているリソースを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="9b99f-108">List the resources associated with this submission.</span></span> <span data-ttu-id="9b99f-109">**提出リソース**オブジェクトは、学生が作業している実際のリソースオブジェクトをラップしたものです。</span><span class="sxs-lookup"><span data-stu-id="9b99f-109">The **submissionResource** object is a wrapper around the actual resource object the student is working on.</span></span> <span data-ttu-id="9b99f-110">このラッパーには、割り当て処理中に割り当てからコピーされた場合に、割り当てのリソースへのポインターも含まれています。</span><span class="sxs-lookup"><span data-stu-id="9b99f-110">The wrapper also includes a pointer to the resources on the assignment if this was copied from the assignment during the assign process.</span></span> <span data-ttu-id="9b99f-111">これらのリソースは、割り当ての作業コピーです。</span><span class="sxs-lookup"><span data-stu-id="9b99f-111">These resources are the working copy of the assignment.</span></span> <span data-ttu-id="9b99f-112">**Submittedresources**は、正式に送信され、採点されるリソースです。</span><span class="sxs-lookup"><span data-stu-id="9b99f-112">The **submittedResources** are the resources that have officially been submitted to be graded.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b99f-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9b99f-113">Permissions</span></span>

<span data-ttu-id="9b99f-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9b99f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9b99f-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9b99f-116">Permission type</span></span>                        | <span data-ttu-id="9b99f-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9b99f-117">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="9b99f-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9b99f-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="9b99f-119">EduAssignments、EduAssignments、EduAssignments、および EduAssignments の読み取り/書き込みの基本</span><span class="sxs-lookup"><span data-stu-id="9b99f-119">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="9b99f-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9b99f-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b99f-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b99f-121">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="9b99f-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9b99f-122">Application</span></span>                            | <span data-ttu-id="9b99f-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b99f-123">Not supported.</span></span>                                                                                         |

## <a name="http-request"></a><span data-ttu-id="9b99f-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9b99f-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /educationClasses/assignments/{id}/submissions/{id}/resources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9b99f-125">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9b99f-125">Optional query parameters</span></span>

<span data-ttu-id="9b99f-126">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="9b99f-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9b99f-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b99f-127">Request headers</span></span>

| <span data-ttu-id="9b99f-128">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b99f-128">Header</span></span>        | <span data-ttu-id="9b99f-129">値</span><span class="sxs-lookup"><span data-stu-id="9b99f-129">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="9b99f-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b99f-130">Authorization</span></span> | <span data-ttu-id="9b99f-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9b99f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b99f-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="9b99f-133">Request body</span></span>

<span data-ttu-id="9b99f-134">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9b99f-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b99f-135">応答</span><span class="sxs-lookup"><span data-stu-id="9b99f-135">Response</span></span>

<span data-ttu-id="9b99f-136">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[educationSubmissionResource](../resources/educationsubmissionresource.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="9b99f-136">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b99f-137">例</span><span class="sxs-lookup"><span data-stu-id="9b99f-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9b99f-138">要求</span><span class="sxs-lookup"><span data-stu-id="9b99f-138">Request</span></span>

<span data-ttu-id="9b99f-139">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9b99f-139">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_resources"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignments/{id}/submissions/{id}/resources
```

##### <a name="response"></a><span data-ttu-id="9b99f-140">応答</span><span class="sxs-lookup"><span data-stu-id="9b99f-140">Response</span></span>

<span data-ttu-id="9b99f-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9b99f-141">The following is an example of the response.</span></span> 

><span data-ttu-id="9b99f-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9b99f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1045

{
  "value": [
    {
      "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
      "id": "f2387c3b-ec39-4bf2-a399-d7242677f024",
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
  "description": "List resources",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
