---
title: Educationassignment を更新します。
description: 割り当てオブジェクトを更新します。 クラスの先生だけは、これを実行できます。 割り当ての状態を変更するのには、修正プログラムの要求を使用できないことに注意してください。 発行アクションを使用すると、割り当ての状態を変更します。
ms.openlocfilehash: 8b23b7ac4b971856ed7a96b4991fca2e5220d069
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069228"
---
# <a name="update-educationassignment"></a><span data-ttu-id="eda81-106">Educationassignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="eda81-106">Update educationassignment</span></span>

> <span data-ttu-id="eda81-107">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="eda81-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eda81-108">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eda81-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eda81-109">割り当てオブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="eda81-109">Update the assignment object.</span></span> <span data-ttu-id="eda81-110">クラスの先生だけは、これを実行できます。</span><span class="sxs-lookup"><span data-stu-id="eda81-110">Only teachers in the class can do this.</span></span> <span data-ttu-id="eda81-111">割り当ての状態を変更するのには、修正プログラムの要求を使用できないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="eda81-111">Note that you can't use a PATCH request to change the status of an assignment.</span></span> <span data-ttu-id="eda81-112">[発行](../api/educationassignment-publish.md)アクションを使用すると、割り当ての状態を変更します。</span><span class="sxs-lookup"><span data-stu-id="eda81-112">Use the [publish](../api/educationassignment-publish.md) action to change the assignment status.</span></span>

## <a name="permissions"></a><span data-ttu-id="eda81-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="eda81-113">Permissions</span></span>
<span data-ttu-id="eda81-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eda81-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eda81-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eda81-116">Permission type</span></span>      | <span data-ttu-id="eda81-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="eda81-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eda81-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eda81-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="eda81-119">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eda81-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="eda81-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eda81-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="eda81-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eda81-121">Not supported.</span></span>  |
|<span data-ttu-id="eda81-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eda81-122">Application</span></span> | <span data-ttu-id="eda81-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eda81-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="eda81-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eda81-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="eda81-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eda81-125">Request headers</span></span>
| <span data-ttu-id="eda81-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eda81-126">Header</span></span>       | <span data-ttu-id="eda81-127">値</span><span class="sxs-lookup"><span data-stu-id="eda81-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="eda81-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="eda81-128">Authorization</span></span>  | <span data-ttu-id="eda81-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="eda81-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="eda81-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eda81-131">Content-Type</span></span>  | <span data-ttu-id="eda81-132">application/json</span><span class="sxs-lookup"><span data-stu-id="eda81-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eda81-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="eda81-133">Request body</span></span>
<span data-ttu-id="eda81-134">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="eda81-134">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="eda81-135">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="eda81-135">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="eda81-136">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="eda81-136">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="eda81-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eda81-137">Property</span></span>     | <span data-ttu-id="eda81-138">型</span><span class="sxs-lookup"><span data-stu-id="eda81-138">Type</span></span>   |<span data-ttu-id="eda81-139">説明</span><span class="sxs-lookup"><span data-stu-id="eda81-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eda81-140">allowLateSubmissions</span><span class="sxs-lookup"><span data-stu-id="eda81-140">allowLateSubmissions</span></span>|<span data-ttu-id="eda81-141">ブール値</span><span class="sxs-lookup"><span data-stu-id="eda81-141">Boolean</span></span>| <span data-ttu-id="eda81-142">かどうかの提出書類は、期限より後に送信できます。</span><span class="sxs-lookup"><span data-stu-id="eda81-142">Whether submissions can be submitted after the due date.</span></span>|
|<span data-ttu-id="eda81-143">allowStudentsToAddResourcesToSubmission</span><span class="sxs-lookup"><span data-stu-id="eda81-143">allowStudentsToAddResourcesToSubmission</span></span>|<span data-ttu-id="eda81-144">ブール値</span><span class="sxs-lookup"><span data-stu-id="eda81-144">Boolean</span></span>| <span data-ttu-id="eda81-145">かどうか、受講生受講者は、提出書類にリソースを追加できます。</span><span class="sxs-lookup"><span data-stu-id="eda81-145">Whether a student can add resources to a submission.</span></span> <span data-ttu-id="eda81-146">リソースの割り当て] ボックスの一覧から、提出書類の項目のみが付属しているかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="eda81-146">Indicated whether the only items on the submission came from the assignment resource list.</span></span> |
|<span data-ttu-id="eda81-147">assignDateTime</span><span class="sxs-lookup"><span data-stu-id="eda81-147">assignDateTime</span></span>|<span data-ttu-id="eda81-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eda81-148">DateTimeOffset</span></span>| <span data-ttu-id="eda81-149">日付は受講者に割り当てを発行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="eda81-149">Date the assignment should be published to students.</span></span> |
|<span data-ttu-id="eda81-150">assignTo</span><span class="sxs-lookup"><span data-stu-id="eda81-150">assignTo</span></span>|<span data-ttu-id="eda81-151">educationAssignmentRecipient</span><span class="sxs-lookup"><span data-stu-id="eda81-151">educationAssignmentRecipient</span></span>| <span data-ttu-id="eda81-152">割り当てを取得した受講者です。</span><span class="sxs-lookup"><span data-stu-id="eda81-152">Students who get the assignment.</span></span>|
|<span data-ttu-id="eda81-153">displayName</span><span class="sxs-lookup"><span data-stu-id="eda81-153">displayName</span></span>|<span data-ttu-id="eda81-154">String</span><span class="sxs-lookup"><span data-stu-id="eda81-154">String</span></span>| <span data-ttu-id="eda81-155">割り当ての名前です。</span><span class="sxs-lookup"><span data-stu-id="eda81-155">Name of assignment.</span></span> |
|<span data-ttu-id="eda81-156">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="eda81-156">dueDateTime</span></span>|<span data-ttu-id="eda81-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eda81-157">DateTimeOffset</span></span>| <span data-ttu-id="eda81-158">割り当ての日付が期限です。</span><span class="sxs-lookup"><span data-stu-id="eda81-158">Date assignment is due.</span></span> |
|<span data-ttu-id="eda81-159">グレーディング</span><span class="sxs-lookup"><span data-stu-id="eda81-159">grading</span></span>|<span data-ttu-id="eda81-160">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="eda81-160">educationAssignmentGradeType</span></span>| <span data-ttu-id="eda81-161">どの割り当てが焼き付けるされます。</span><span class="sxs-lookup"><span data-stu-id="eda81-161">How the assignment will be graded.</span></span>|
|<span data-ttu-id="eda81-162">指示</span><span class="sxs-lookup"><span data-stu-id="eda81-162">instructions</span></span>|<span data-ttu-id="eda81-163">itemBody</span><span class="sxs-lookup"><span data-stu-id="eda81-163">itemBody</span></span>| <span data-ttu-id="eda81-164">割り当てと受講者に指示します。</span><span class="sxs-lookup"><span data-stu-id="eda81-164">Instructions to be given to the students along with the assignment.</span></span> |

## <a name="response"></a><span data-ttu-id="eda81-165">応答</span><span class="sxs-lookup"><span data-stu-id="eda81-165">Response</span></span>
<span data-ttu-id="eda81-166">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[educationAssignment](../resources/educationassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="eda81-166">If successful, this method returns a `200 OK` response code and an updated [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eda81-167">例</span><span class="sxs-lookup"><span data-stu-id="eda81-167">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eda81-168">要求</span><span class="sxs-lookup"><span data-stu-id="eda81-168">Request</span></span>
<span data-ttu-id="eda81-169">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="eda81-169">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="eda81-170">応答</span><span class="sxs-lookup"><span data-stu-id="eda81-170">Response</span></span>
<span data-ttu-id="eda81-171">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="eda81-171">The following is an example of the response.</span></span> 

><span data-ttu-id="eda81-172">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="eda81-172">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="eda81-173">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="eda81-173">All of the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Update educationassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->