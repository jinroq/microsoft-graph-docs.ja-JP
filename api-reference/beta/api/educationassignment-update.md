---
title: Educationassignment を更新します。
description: 割り当てオブジェクトを更新します。 クラスの先生だけは、これを実行できます。 割り当ての状態を変更するのには、修正プログラムの要求を使用できないことに注意してください。 発行アクションを使用すると、割り当ての状態を変更します。
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: eb5762f86e1572f9a9d5876199c945154a25293b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524962"
---
# <a name="update-educationassignment"></a><span data-ttu-id="94d96-106">Educationassignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="94d96-106">Update educationassignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94d96-107">割り当てオブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="94d96-107">Update the assignment object.</span></span> <span data-ttu-id="94d96-108">クラスの先生だけは、これを実行できます。</span><span class="sxs-lookup"><span data-stu-id="94d96-108">Only teachers in the class can do this.</span></span> <span data-ttu-id="94d96-109">割り当ての状態を変更するのには、修正プログラムの要求を使用できないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="94d96-109">Note that you can't use a PATCH request to change the status of an assignment.</span></span> <span data-ttu-id="94d96-110">[発行](../api/educationassignment-publish.md)アクションを使用すると、割り当ての状態を変更します。</span><span class="sxs-lookup"><span data-stu-id="94d96-110">Use the [publish](../api/educationassignment-publish.md) action to change the assignment status.</span></span>

## <a name="permissions"></a><span data-ttu-id="94d96-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="94d96-111">Permissions</span></span>
<span data-ttu-id="94d96-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="94d96-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94d96-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="94d96-114">Permission type</span></span>      | <span data-ttu-id="94d96-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="94d96-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94d96-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="94d96-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="94d96-117">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94d96-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="94d96-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="94d96-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="94d96-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94d96-119">Not supported.</span></span>  |
|<span data-ttu-id="94d96-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="94d96-120">Application</span></span> | <span data-ttu-id="94d96-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94d96-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="94d96-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="94d96-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="94d96-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="94d96-123">Request headers</span></span>
| <span data-ttu-id="94d96-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="94d96-124">Header</span></span>       | <span data-ttu-id="94d96-125">値</span><span class="sxs-lookup"><span data-stu-id="94d96-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="94d96-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="94d96-126">Authorization</span></span>  | <span data-ttu-id="94d96-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="94d96-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="94d96-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="94d96-129">Content-Type</span></span>  | <span data-ttu-id="94d96-130">application/json</span><span class="sxs-lookup"><span data-stu-id="94d96-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="94d96-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="94d96-131">Request body</span></span>
<span data-ttu-id="94d96-132">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="94d96-132">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="94d96-133">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="94d96-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="94d96-134">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="94d96-134">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="94d96-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="94d96-135">Property</span></span>     | <span data-ttu-id="94d96-136">型</span><span class="sxs-lookup"><span data-stu-id="94d96-136">Type</span></span>   |<span data-ttu-id="94d96-137">説明</span><span class="sxs-lookup"><span data-stu-id="94d96-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94d96-138">allowLateSubmissions</span><span class="sxs-lookup"><span data-stu-id="94d96-138">allowLateSubmissions</span></span>|<span data-ttu-id="94d96-139">ブール値</span><span class="sxs-lookup"><span data-stu-id="94d96-139">Boolean</span></span>| <span data-ttu-id="94d96-140">かどうかの提出書類は、期限より後に送信できます。</span><span class="sxs-lookup"><span data-stu-id="94d96-140">Whether submissions can be submitted after the due date.</span></span>|
|<span data-ttu-id="94d96-141">allowStudentsToAddResourcesToSubmission</span><span class="sxs-lookup"><span data-stu-id="94d96-141">allowStudentsToAddResourcesToSubmission</span></span>|<span data-ttu-id="94d96-142">ブール値</span><span class="sxs-lookup"><span data-stu-id="94d96-142">Boolean</span></span>| <span data-ttu-id="94d96-143">かどうか、受講生受講者は、提出書類にリソースを追加できます。</span><span class="sxs-lookup"><span data-stu-id="94d96-143">Whether a student can add resources to a submission.</span></span> <span data-ttu-id="94d96-144">リソースの割り当て] ボックスの一覧から、提出書類の項目のみが付属しているかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="94d96-144">Indicated whether the only items on the submission came from the assignment resource list.</span></span> |
|<span data-ttu-id="94d96-145">assignDateTime</span><span class="sxs-lookup"><span data-stu-id="94d96-145">assignDateTime</span></span>|<span data-ttu-id="94d96-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94d96-146">DateTimeOffset</span></span>| <span data-ttu-id="94d96-147">日付は受講者に割り当てを発行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="94d96-147">Date the assignment should be published to students.</span></span> |
|<span data-ttu-id="94d96-148">assignTo</span><span class="sxs-lookup"><span data-stu-id="94d96-148">assignTo</span></span>|<span data-ttu-id="94d96-149">educationAssignmentRecipient</span><span class="sxs-lookup"><span data-stu-id="94d96-149">educationAssignmentRecipient</span></span>| <span data-ttu-id="94d96-150">割り当てを取得した受講者です。</span><span class="sxs-lookup"><span data-stu-id="94d96-150">Students who get the assignment.</span></span>|
|<span data-ttu-id="94d96-151">displayName</span><span class="sxs-lookup"><span data-stu-id="94d96-151">displayName</span></span>|<span data-ttu-id="94d96-152">String</span><span class="sxs-lookup"><span data-stu-id="94d96-152">String</span></span>| <span data-ttu-id="94d96-153">割り当ての名前です。</span><span class="sxs-lookup"><span data-stu-id="94d96-153">Name of assignment.</span></span> |
|<span data-ttu-id="94d96-154">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="94d96-154">dueDateTime</span></span>|<span data-ttu-id="94d96-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94d96-155">DateTimeOffset</span></span>| <span data-ttu-id="94d96-156">割り当ての日付が期限です。</span><span class="sxs-lookup"><span data-stu-id="94d96-156">Date assignment is due.</span></span> |
|<span data-ttu-id="94d96-157">グレーディング</span><span class="sxs-lookup"><span data-stu-id="94d96-157">grading</span></span>|<span data-ttu-id="94d96-158">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="94d96-158">educationAssignmentGradeType</span></span>| <span data-ttu-id="94d96-159">どの割り当てが焼き付けるされます。</span><span class="sxs-lookup"><span data-stu-id="94d96-159">How the assignment will be graded.</span></span>|
|<span data-ttu-id="94d96-160">手順</span><span class="sxs-lookup"><span data-stu-id="94d96-160">instructions</span></span>|<span data-ttu-id="94d96-161">item.body</span><span class="sxs-lookup"><span data-stu-id="94d96-161">itemBody</span></span>| <span data-ttu-id="94d96-162">割り当てと受講者に指示します。</span><span class="sxs-lookup"><span data-stu-id="94d96-162">Instructions to be given to the students along with the assignment.</span></span> |

## <a name="response"></a><span data-ttu-id="94d96-163">応答</span><span class="sxs-lookup"><span data-stu-id="94d96-163">Response</span></span>
<span data-ttu-id="94d96-164">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[educationAssignment](../resources/educationassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="94d96-164">If successful, this method returns a `200 OK` response code and an updated [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="94d96-165">例</span><span class="sxs-lookup"><span data-stu-id="94d96-165">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94d96-166">要求</span><span class="sxs-lookup"><span data-stu-id="94d96-166">Request</span></span>
<span data-ttu-id="94d96-167">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="94d96-167">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationassignment"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11021/assignments/19002
Content-type: application/json
Content-length: 279

{
  "displayName": "Week 1 reading assignment",
  "instructions": {
    "contentType": "Text",
    "content": "Read chapters 1 through 3"
  },
  "dueDateTime": "2014-02-01T00:00:00Z"
}
```
##### <a name="response"></a><span data-ttu-id="94d96-168">応答</span><span class="sxs-lookup"><span data-stu-id="94d96-168">Response</span></span>
<span data-ttu-id="94d96-169">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="94d96-169">The following is an example of the response.</span></span> 

><span data-ttu-id="94d96-170">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="94d96-170">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="94d96-171">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="94d96-171">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
  "classId": "11021",
  "displayName": "Week 1 reading assignment",
  "instructions": {
    "contentType": "Text",
    "content": "Read chapters 1 through 3"
  },
  "dueDateTime": "2014-02-01T00:00:00Z",
  "assignDateTime": "2014-01-01T00:00:00Z",
  "assignedDateTime": "2014-01-01T00:00:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update educationassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
