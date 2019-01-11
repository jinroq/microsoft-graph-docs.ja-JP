---
title: secureScoreControlProfiles の更新
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: b89a5e147d4882dbe25456cd2acc42b56924d12b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817655"
---
# <a name="update-securescorecontrolprofiles"></a><span data-ttu-id="d11b1-104">secureScoreControlProfiles の更新</span><span class="sxs-lookup"><span data-stu-id="d11b1-104">Update secureScoreControlProfiles</span></span>

 > <span data-ttu-id="d11b1-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d11b1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d11b1-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d11b1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d11b1-107">**担当者**や**tenantNote**などのさまざまなプロパティを変更するのには統合されたソリューション内で編集可能な**secureScoreControlProfiles**プロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d11b1-107">Update an editable **secureScoreControlProfiles** property within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="d11b1-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d11b1-108">Permissions</span></span>

<span data-ttu-id="d11b1-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d11b1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d11b1-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d11b1-111">Permission type</span></span>      | <span data-ttu-id="d11b1-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d11b1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d11b1-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d11b1-113">Delegated (work or school account)</span></span> |   <span data-ttu-id="d11b1-114">SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="d11b1-114">SecurityEvents.ReadWrite.All.</span></span>  |
|<span data-ttu-id="d11b1-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d11b1-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d11b1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d11b1-116">Not supported.</span></span>  |
|<span data-ttu-id="d11b1-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d11b1-117">Application</span></span> | <span data-ttu-id="d11b1-118">SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="d11b1-118">SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d11b1-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d11b1-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d11b1-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d11b1-120">Request headers</span></span>

| <span data-ttu-id="d11b1-121">名前</span><span class="sxs-lookup"><span data-stu-id="d11b1-121">Name</span></span>       | <span data-ttu-id="d11b1-122">説明</span><span class="sxs-lookup"><span data-stu-id="d11b1-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d11b1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d11b1-123">Authorization</span></span>  | <span data-ttu-id="d11b1-p104">Bearer {code}。必須。</span><span class="sxs-lookup"><span data-stu-id="d11b1-p104">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="d11b1-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="d11b1-126">Prefer</span></span> | <span data-ttu-id="d11b1-127">返す = 表現します。</span><span class="sxs-lookup"><span data-stu-id="d11b1-127">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d11b1-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="d11b1-128">Request body</span></span>

<span data-ttu-id="d11b1-129">要求の本文には、更新される関連フィールドの値の JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="d11b1-129">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d11b1-130">SecureScoreControlProfile に更新可能なフィールドを次の表に一覧します。</span><span class="sxs-lookup"><span data-stu-id="d11b1-130">The following table lists the fields that can be updated for a secureScoreControlProfile.</span></span> <span data-ttu-id="d11b1-131">要求の本文に含まれていない既存のプロパティの値は変更されません。</span><span class="sxs-lookup"><span data-stu-id="d11b1-131">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="d11b1-132">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="d11b1-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d11b1-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d11b1-133">Property</span></span>   | <span data-ttu-id="d11b1-134">種類</span><span class="sxs-lookup"><span data-stu-id="d11b1-134">Type</span></span> |<span data-ttu-id="d11b1-135">説明</span><span class="sxs-lookup"><span data-stu-id="d11b1-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d11b1-136">担当者</span><span class="sxs-lookup"><span data-stu-id="d11b1-136">assignedTo</span></span>|<span data-ttu-id="d11b1-137">String</span><span class="sxs-lookup"><span data-stu-id="d11b1-137">String</span></span>|<span data-ttu-id="d11b1-138">アナリストのコントロールの名前は、選別、導入、または修復用に割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="d11b1-138">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="d11b1-139">tenantNote</span><span class="sxs-lookup"><span data-stu-id="d11b1-139">tenantNote</span></span>|<span data-ttu-id="d11b1-140">String</span><span class="sxs-lookup"><span data-stu-id="d11b1-140">String</span></span>|<span data-ttu-id="d11b1-141">(顧客管理) のコントロールのアナリストのコメントです。</span><span class="sxs-lookup"><span data-stu-id="d11b1-141">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="d11b1-142">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="d11b1-142">controlStateUpdates</span></span>| <span data-ttu-id="d11b1-143">String</span><span class="sxs-lookup"><span data-stu-id="d11b1-143">String</span></span>|<span data-ttu-id="d11b1-144">アナリストは、コントロールの設定を優先します。</span><span class="sxs-lookup"><span data-stu-id="d11b1-144">Analyst driven setting on the control.</span></span> <span data-ttu-id="d11b1-145">可能な値は、`ignore`、`thirdParty`、`reviewed` です。</span><span class="sxs-lookup"><span data-stu-id="d11b1-145">Possible values are: `ignore`, `thirdParty`, `reviewed`.</span></span>|


## <a name="response"></a><span data-ttu-id="d11b1-146">応答</span><span class="sxs-lookup"><span data-stu-id="d11b1-146">Response</span></span>

<span data-ttu-id="d11b1-147">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="d11b1-147">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="d11b1-148">省略可能な要求ヘッダーが使用され、メソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[secureScoreControlProfiles](../resources/securescorecontrolprofiles.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="d11b1-148">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d11b1-149">例</span><span class="sxs-lookup"><span data-stu-id="d11b1-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="d11b1-150">要求</span><span class="sxs-lookup"><span data-stu-id="d11b1-150">Request</span></span>

<span data-ttu-id="d11b1-151">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d11b1-151">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d11b1-152">応答</span><span class="sxs-lookup"><span data-stu-id="d11b1-152">Response</span></span>

<span data-ttu-id="d11b1-153">次は、正常な応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d11b1-153">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
} -->

```http
HTTP/1.1 204 No Content
```




<!-- {
  "type": "#page.annotation",
  "description": "Update secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
