---
title: secureScoreControlProfiles の更新
description: 担当者や tenantNote などのさまざまなプロパティを変更するのには統合されたソリューション内で編集可能な secureScoreControlProfiles プロパティを更新します。
localization_priority: Normal
ms.openlocfilehash: 2be11c6b369d9dc411afa5af2219c3bfa8605c8a
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573362"
---
# <a name="update-securescorecontrolprofiles"></a><span data-ttu-id="32b7b-103">secureScoreControlProfiles の更新</span><span class="sxs-lookup"><span data-stu-id="32b7b-103">Update secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32b7b-104">**担当者**や**tenantNote**などのさまざまなプロパティを変更するのには統合されたソリューション内で編集可能な**secureScoreControlProfiles**プロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="32b7b-104">Update an editable **secureScoreControlProfiles** property within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="32b7b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="32b7b-105">Permissions</span></span>

<span data-ttu-id="32b7b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="32b7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32b7b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="32b7b-108">Permission type</span></span>      | <span data-ttu-id="32b7b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="32b7b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32b7b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="32b7b-110">Delegated (work or school account)</span></span> |   <span data-ttu-id="32b7b-111">SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="32b7b-111">SecurityEvents.ReadWrite.All.</span></span>  |
|<span data-ttu-id="32b7b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="32b7b-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="32b7b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32b7b-113">Not supported.</span></span>  |
|<span data-ttu-id="32b7b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="32b7b-114">Application</span></span> | <span data-ttu-id="32b7b-115">SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="32b7b-115">SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="32b7b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="32b7b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="32b7b-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="32b7b-117">Request headers</span></span>

| <span data-ttu-id="32b7b-118">名前</span><span class="sxs-lookup"><span data-stu-id="32b7b-118">Name</span></span>       | <span data-ttu-id="32b7b-119">説明</span><span class="sxs-lookup"><span data-stu-id="32b7b-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="32b7b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="32b7b-120">Authorization</span></span>  | <span data-ttu-id="32b7b-p102">Bearer {code}。必須。</span><span class="sxs-lookup"><span data-stu-id="32b7b-p102">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="32b7b-123">Prefer</span><span class="sxs-lookup"><span data-stu-id="32b7b-123">Prefer</span></span> | <span data-ttu-id="32b7b-124">返す = 表現します。</span><span class="sxs-lookup"><span data-stu-id="32b7b-124">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="32b7b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="32b7b-125">Request body</span></span>

<span data-ttu-id="32b7b-126">要求の本文には、更新される関連フィールドの値の JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="32b7b-126">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="32b7b-127">SecureScoreControlProfile に更新可能なフィールドを次の表に一覧します。</span><span class="sxs-lookup"><span data-stu-id="32b7b-127">The following table lists the fields that can be updated for a secureScoreControlProfile.</span></span> <span data-ttu-id="32b7b-128">要求の本文に含まれていない既存のプロパティの値は変更されません。</span><span class="sxs-lookup"><span data-stu-id="32b7b-128">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="32b7b-129">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="32b7b-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="32b7b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32b7b-130">Property</span></span>   | <span data-ttu-id="32b7b-131">型</span><span class="sxs-lookup"><span data-stu-id="32b7b-131">Type</span></span> |<span data-ttu-id="32b7b-132">説明</span><span class="sxs-lookup"><span data-stu-id="32b7b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32b7b-133">担当者</span><span class="sxs-lookup"><span data-stu-id="32b7b-133">assignedTo</span></span>|<span data-ttu-id="32b7b-134">String</span><span class="sxs-lookup"><span data-stu-id="32b7b-134">String</span></span>|<span data-ttu-id="32b7b-135">アナリストのコントロールの名前は、選別、導入、または修復用に割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="32b7b-135">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="32b7b-136">tenantNote</span><span class="sxs-lookup"><span data-stu-id="32b7b-136">tenantNote</span></span>|<span data-ttu-id="32b7b-137">String</span><span class="sxs-lookup"><span data-stu-id="32b7b-137">String</span></span>|<span data-ttu-id="32b7b-138">(顧客管理) のコントロールのアナリストのコメントです。</span><span class="sxs-lookup"><span data-stu-id="32b7b-138">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="32b7b-139">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="32b7b-139">controlStateUpdates</span></span>| <span data-ttu-id="32b7b-140">String</span><span class="sxs-lookup"><span data-stu-id="32b7b-140">String</span></span>|<span data-ttu-id="32b7b-141">アナリストは、コントロールの設定を優先します。</span><span class="sxs-lookup"><span data-stu-id="32b7b-141">Analyst driven setting on the control.</span></span> <span data-ttu-id="32b7b-142">可能な値は、`ignore`、`thirdParty`、`reviewed` です。</span><span class="sxs-lookup"><span data-stu-id="32b7b-142">Possible values are: `ignore`, `thirdParty`, `reviewed`.</span></span>|


## <a name="response"></a><span data-ttu-id="32b7b-143">応答</span><span class="sxs-lookup"><span data-stu-id="32b7b-143">Response</span></span>

<span data-ttu-id="32b7b-144">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="32b7b-144">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="32b7b-145">省略可能な要求ヘッダーが使用され、メソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[secureScoreControlProfiles](../resources/securescorecontrolprofiles.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="32b7b-145">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32b7b-146">例</span><span class="sxs-lookup"><span data-stu-id="32b7b-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="32b7b-147">要求</span><span class="sxs-lookup"><span data-stu-id="32b7b-147">Request</span></span>

<span data-ttu-id="32b7b-148">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="32b7b-148">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/secureScoreControlProfiles/AdminMFA
Content-type: application/json

{
  "assignedTo": "assignedTo-value",
  "controlStateUpdates": "controlStateUpdates-value",
  "tenantNote": "tenantNote-value"
}
```

### <a name="response"></a><span data-ttu-id="32b7b-149">応答</span><span class="sxs-lookup"><span data-stu-id="32b7b-149">Response</span></span>

<span data-ttu-id="32b7b-150">次は、正常な応答の例です。</span><span class="sxs-lookup"><span data-stu-id="32b7b-150">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Update secureScoreControlProfile",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/securescorecontrolprofiles-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
