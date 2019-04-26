---
title: educationassignment の更新
description: assignment オブジェクトを更新します。 この操作を行うことができるのは、クラス内の教師だけです。 PATCH 要求を使用して割り当ての状態を変更することはできないことに注意してください。 割り当ての状態を変更するには、発行アクションを使用します。
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: c8b6659d0af1ae57829add1f64c19cb954b8413f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325019"
---
# <a name="update-educationassignment"></a><span data-ttu-id="52234-106">educationassignment の更新</span><span class="sxs-lookup"><span data-stu-id="52234-106">Update educationassignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52234-107">assignment オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="52234-107">Update the assignment object.</span></span> <span data-ttu-id="52234-108">この操作を行うことができるのは、クラス内の教師だけです。</span><span class="sxs-lookup"><span data-stu-id="52234-108">Only teachers in the class can do this.</span></span> <span data-ttu-id="52234-109">PATCH 要求を使用して割り当ての状態を変更することはできないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="52234-109">Note that you can't use a PATCH request to change the status of an assignment.</span></span> <span data-ttu-id="52234-110">割り当ての状態を変更するには、[発行](../api/educationassignment-publish.md)アクションを使用します。</span><span class="sxs-lookup"><span data-stu-id="52234-110">Use the [publish](../api/educationassignment-publish.md) action to change the assignment status.</span></span>

## <a name="permissions"></a><span data-ttu-id="52234-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="52234-111">Permissions</span></span>
<span data-ttu-id="52234-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="52234-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52234-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="52234-114">Permission type</span></span>      | <span data-ttu-id="52234-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="52234-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52234-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="52234-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="52234-117">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="52234-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="52234-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="52234-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="52234-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52234-119">Not supported.</span></span>  |
|<span data-ttu-id="52234-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="52234-120">Application</span></span> | <span data-ttu-id="52234-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52234-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="52234-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="52234-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="52234-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="52234-123">Request headers</span></span>
| <span data-ttu-id="52234-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="52234-124">Header</span></span>       | <span data-ttu-id="52234-125">値</span><span class="sxs-lookup"><span data-stu-id="52234-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="52234-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="52234-126">Authorization</span></span>  | <span data-ttu-id="52234-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="52234-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="52234-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="52234-129">Content-Type</span></span>  | <span data-ttu-id="52234-130">application/json</span><span class="sxs-lookup"><span data-stu-id="52234-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="52234-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="52234-131">Request body</span></span>
<span data-ttu-id="52234-132">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="52234-132">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="52234-133">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="52234-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="52234-134">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="52234-134">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="52234-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52234-135">Property</span></span>     | <span data-ttu-id="52234-136">型</span><span class="sxs-lookup"><span data-stu-id="52234-136">Type</span></span>   |<span data-ttu-id="52234-137">説明</span><span class="sxs-lookup"><span data-stu-id="52234-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52234-138">allowLateSubmissions</span><span class="sxs-lookup"><span data-stu-id="52234-138">allowLateSubmissions</span></span>|<span data-ttu-id="52234-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="52234-139">Boolean</span></span>| <span data-ttu-id="52234-140">期日後に提出を送信できるかどうか。</span><span class="sxs-lookup"><span data-stu-id="52234-140">Whether submissions can be submitted after the due date.</span></span>|
|<span data-ttu-id="52234-141">allowStudentsToAddResourcesToSubmission</span><span class="sxs-lookup"><span data-stu-id="52234-141">allowStudentsToAddResourcesToSubmission</span></span>|<span data-ttu-id="52234-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="52234-142">Boolean</span></span>| <span data-ttu-id="52234-143">学生が提出物にリソースを追加できるかどうか。</span><span class="sxs-lookup"><span data-stu-id="52234-143">Whether a student can add resources to a submission.</span></span> <span data-ttu-id="52234-144">提出物のアイテムが割り当てリソースリストからのものだけであったかどうかを示しました。</span><span class="sxs-lookup"><span data-stu-id="52234-144">Indicated whether the only items on the submission came from the assignment resource list.</span></span> |
|<span data-ttu-id="52234-145">割り当ての datetime</span><span class="sxs-lookup"><span data-stu-id="52234-145">assignDateTime</span></span>|<span data-ttu-id="52234-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52234-146">DateTimeOffset</span></span>| <span data-ttu-id="52234-147">割り当てが学生に公開される日付。</span><span class="sxs-lookup"><span data-stu-id="52234-147">Date the assignment should be published to students.</span></span> |
|<span data-ttu-id="52234-148">への割り当て</span><span class="sxs-lookup"><span data-stu-id="52234-148">assignTo</span></span>|<span data-ttu-id="52234-149">educationAssignmentRecipient</span><span class="sxs-lookup"><span data-stu-id="52234-149">educationAssignmentRecipient</span></span>| <span data-ttu-id="52234-150">課題を受ける学生。</span><span class="sxs-lookup"><span data-stu-id="52234-150">Students who get the assignment.</span></span>|
|<span data-ttu-id="52234-151">displayName</span><span class="sxs-lookup"><span data-stu-id="52234-151">displayName</span></span>|<span data-ttu-id="52234-152">String</span><span class="sxs-lookup"><span data-stu-id="52234-152">String</span></span>| <span data-ttu-id="52234-153">割り当ての名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="52234-153">Name of assignment.</span></span> |
|<span data-ttu-id="52234-154">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="52234-154">dueDateTime</span></span>|<span data-ttu-id="52234-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52234-155">DateTimeOffset</span></span>| <span data-ttu-id="52234-156">日付の割り当て期限です。</span><span class="sxs-lookup"><span data-stu-id="52234-156">Date assignment is due.</span></span> |
|<span data-ttu-id="52234-157">変化</span><span class="sxs-lookup"><span data-stu-id="52234-157">grading</span></span>|<span data-ttu-id="52234-158">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="52234-158">educationAssignmentGradeType</span></span>| <span data-ttu-id="52234-159">割り当てが採点される方法。</span><span class="sxs-lookup"><span data-stu-id="52234-159">How the assignment will be graded.</span></span>|
|<span data-ttu-id="52234-160">手順</span><span class="sxs-lookup"><span data-stu-id="52234-160">instructions</span></span>|<span data-ttu-id="52234-161">itemBody</span><span class="sxs-lookup"><span data-stu-id="52234-161">itemBody</span></span>| <span data-ttu-id="52234-162">受講者に割り当てと共に提供される指示。</span><span class="sxs-lookup"><span data-stu-id="52234-162">Instructions to be given to the students along with the assignment.</span></span> |

## <a name="response"></a><span data-ttu-id="52234-163">応答</span><span class="sxs-lookup"><span data-stu-id="52234-163">Response</span></span>
<span data-ttu-id="52234-164">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[educationAssignment](../resources/educationassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="52234-164">If successful, this method returns a `200 OK` response code and an updated [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="52234-165">例</span><span class="sxs-lookup"><span data-stu-id="52234-165">Example</span></span>
##### <a name="request"></a><span data-ttu-id="52234-166">要求</span><span class="sxs-lookup"><span data-stu-id="52234-166">Request</span></span>
<span data-ttu-id="52234-167">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="52234-167">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="52234-168">応答</span><span class="sxs-lookup"><span data-stu-id="52234-168">Response</span></span>
<span data-ttu-id="52234-169">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="52234-169">The following is an example of the response.</span></span> 

><span data-ttu-id="52234-170">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="52234-170">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="52234-171">すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="52234-171">All of the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->
