---
title: EducationAssignmentResource を更新します。
description: '割り当てに関連付けられているリソースのプロパティを更新します。 クラスで教師だけでは、割り当てリソースのオブジェクトを変更できます。  '
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: 91321cc124baa87a82f2f1f5fecc65365cafc18d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879311"
---
# <a name="update-educationassignmentresource"></a><span data-ttu-id="e2384-104">EducationAssignmentResource を更新します。</span><span class="sxs-lookup"><span data-stu-id="e2384-104">Update educationAssignmentResource</span></span>

> <span data-ttu-id="e2384-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e2384-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2384-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2384-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e2384-107">割り当てに関連付けられているリソースのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e2384-107">Update the properties of resource associated with an assignment.</span></span> <span data-ttu-id="e2384-108">クラスで教師だけでは、割り当てリソースのオブジェクトを変更できます。</span><span class="sxs-lookup"><span data-stu-id="e2384-108">Only teachers in a class can change assignment resource objects.</span></span>  

## <a name="permissions"></a><span data-ttu-id="e2384-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e2384-109">Permissions</span></span>
<span data-ttu-id="e2384-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2384-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2384-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e2384-112">Permission type</span></span>      | <span data-ttu-id="e2384-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e2384-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2384-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e2384-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="e2384-115">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2384-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="e2384-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e2384-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e2384-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2384-117">Not supported.</span></span>  |
|<span data-ttu-id="e2384-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e2384-118">Application</span></span> | <span data-ttu-id="e2384-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2384-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e2384-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e2384-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e2384-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e2384-121">Request headers</span></span>
| <span data-ttu-id="e2384-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e2384-122">Header</span></span>       | <span data-ttu-id="e2384-123">値</span><span class="sxs-lookup"><span data-stu-id="e2384-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e2384-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2384-124">Authorization</span></span>  | <span data-ttu-id="e2384-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e2384-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e2384-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e2384-127">Content-Type</span></span>  | <span data-ttu-id="e2384-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e2384-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e2384-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="e2384-129">Request body</span></span>
<span data-ttu-id="e2384-130">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="e2384-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e2384-131">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="e2384-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e2384-132">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="e2384-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e2384-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2384-133">Property</span></span>     | <span data-ttu-id="e2384-134">種類</span><span class="sxs-lookup"><span data-stu-id="e2384-134">Type</span></span>   |<span data-ttu-id="e2384-135">説明</span><span class="sxs-lookup"><span data-stu-id="e2384-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2384-136">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="e2384-136">distributeForStudentWork</span></span>|<span data-ttu-id="e2384-137">ブール型</span><span class="sxs-lookup"><span data-stu-id="e2384-137">Boolean</span></span>| <span data-ttu-id="e2384-138">割り当てを発行する際、このリソースを各受講者用のリソース オブジェクトにコピーかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e2384-138">Indicates whether this resource should be copied to each student's resource object when the assignment is published.</span></span>|
|<span data-ttu-id="e2384-139">resource</span><span class="sxs-lookup"><span data-stu-id="e2384-139">resource</span></span>|<span data-ttu-id="e2384-140">educationResource</span><span class="sxs-lookup"><span data-stu-id="e2384-140">educationResource</span></span>| <span data-ttu-id="e2384-141">リソース オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="e2384-141">Resource object.</span></span> |

## <a name="response"></a><span data-ttu-id="e2384-142">応答</span><span class="sxs-lookup"><span data-stu-id="e2384-142">Response</span></span>
<span data-ttu-id="e2384-143">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[educationAssignmentResource](../resources/educationassignmentresource.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="e2384-143">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e2384-144">例</span><span class="sxs-lookup"><span data-stu-id="e2384-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e2384-145">要求</span><span class="sxs-lookup"><span data-stu-id="e2384-145">Request</span></span>
<span data-ttu-id="e2384-146">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e2384-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "update_educationassignmentresource"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/850f51b7-1df9-4ec0-bd62-64a0214b9cbf
Content-type: application/json
Content-length: 822

{
  "distributeForStudentWork": "false"
}
```
##### <a name="response"></a><span data-ttu-id="e2384-147">応答</span><span class="sxs-lookup"><span data-stu-id="e2384-147">Response</span></span>
<span data-ttu-id="e2384-148">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e2384-148">The following is an example of the response.</span></span> 

><span data-ttu-id="e2384-149">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="e2384-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e2384-150">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e2384-150">All of the properties will be returned from an actual call.</span></span>


<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 832

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
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationassignmentresource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
