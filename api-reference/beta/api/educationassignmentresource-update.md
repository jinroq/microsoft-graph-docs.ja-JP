---
title: educationAssignmentResource の更新
description: '割り当てに関連付けられているリソースのプロパティを更新します。 クラス内の教師のみが、割り当てリソースオブジェクトを変更できます。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 34b1c05937f57fe46d5d854d21a7c2e0b68240d2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457957"
---
# <a name="update-educationassignmentresource"></a><span data-ttu-id="6e141-104">educationAssignmentResource の更新</span><span class="sxs-lookup"><span data-stu-id="6e141-104">Update educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e141-105">割り当てに関連付けられているリソースのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6e141-105">Update the properties of resource associated with an assignment.</span></span> <span data-ttu-id="6e141-106">クラス内の教師のみが、割り当てリソースオブジェクトを変更できます。</span><span class="sxs-lookup"><span data-stu-id="6e141-106">Only teachers in a class can change assignment resource objects.</span></span>  

## <a name="permissions"></a><span data-ttu-id="6e141-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6e141-107">Permissions</span></span>
<span data-ttu-id="6e141-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6e141-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e141-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6e141-110">Permission type</span></span>      | <span data-ttu-id="6e141-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6e141-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e141-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6e141-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="6e141-113">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="6e141-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="6e141-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6e141-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6e141-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6e141-115">Not supported.</span></span>  |
|<span data-ttu-id="6e141-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6e141-116">Application</span></span> | <span data-ttu-id="6e141-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6e141-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6e141-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6e141-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6e141-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6e141-119">Request headers</span></span>
| <span data-ttu-id="6e141-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6e141-120">Header</span></span>       | <span data-ttu-id="6e141-121">値</span><span class="sxs-lookup"><span data-stu-id="6e141-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6e141-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e141-122">Authorization</span></span>  | <span data-ttu-id="6e141-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6e141-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6e141-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6e141-125">Content-Type</span></span>  | <span data-ttu-id="6e141-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e141-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6e141-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="6e141-127">Request body</span></span>
<span data-ttu-id="6e141-128">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="6e141-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6e141-129">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="6e141-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6e141-130">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="6e141-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6e141-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6e141-131">Property</span></span>     | <span data-ttu-id="6e141-132">型</span><span class="sxs-lookup"><span data-stu-id="6e141-132">Type</span></span>   |<span data-ttu-id="6e141-133">説明</span><span class="sxs-lookup"><span data-stu-id="6e141-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e141-134">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="6e141-134">distributeForStudentWork</span></span>|<span data-ttu-id="6e141-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e141-135">Boolean</span></span>| <span data-ttu-id="6e141-136">割り当てが発行されたときに、各学生のリソースオブジェクトにこのリソースをコピーする必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6e141-136">Indicates whether this resource should be copied to each student's resource object when the assignment is published.</span></span>|
|<span data-ttu-id="6e141-137">リソース</span><span class="sxs-lookup"><span data-stu-id="6e141-137">resource</span></span>|<span data-ttu-id="6e141-138">educationResource</span><span class="sxs-lookup"><span data-stu-id="6e141-138">educationResource</span></span>| <span data-ttu-id="6e141-139">Resource オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="6e141-139">Resource object.</span></span> |

## <a name="response"></a><span data-ttu-id="6e141-140">応答</span><span class="sxs-lookup"><span data-stu-id="6e141-140">Response</span></span>
<span data-ttu-id="6e141-141">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[educationAssignmentResource](../resources/educationassignmentresource.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6e141-141">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6e141-142">例</span><span class="sxs-lookup"><span data-stu-id="6e141-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6e141-143">要求</span><span class="sxs-lookup"><span data-stu-id="6e141-143">Request</span></span>
<span data-ttu-id="6e141-144">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6e141-144">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="6e141-145">応答</span><span class="sxs-lookup"><span data-stu-id="6e141-145">Response</span></span>
<span data-ttu-id="6e141-146">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6e141-146">The following is an example of the response.</span></span> 

><span data-ttu-id="6e141-147">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="6e141-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6e141-148">すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6e141-148">All of the properties will be returned from an actual call.</span></span>


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
<!--
{
  "type": "#page.annotation",
  "description": "Update educationassignmentresource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignmentresource-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
