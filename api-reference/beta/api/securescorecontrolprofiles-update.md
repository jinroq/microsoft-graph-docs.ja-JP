---
title: secureScoreControlProfiles の更新
description: 任意の統合ソリューション内の編集可能な Securescorecontrolprofiles のプロパティを更新して、担当者または tenantNote などのさまざまなプロパティを変更します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 5c2060486fc5e007e8aa61751d14192d33e4d37c
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410422"
---
# <a name="update-securescorecontrolprofiles"></a><span data-ttu-id="da330-103">secureScoreControlProfiles の更新</span><span class="sxs-lookup"><span data-stu-id="da330-103">Update secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da330-104">任意の統合ソリューション内の編集可能な**securescorecontrolprofiles の**プロパティを更新して、**担当者**または**tenantnote**などのさまざまなプロパティを変更します。</span><span class="sxs-lookup"><span data-stu-id="da330-104">Update an editable **secureScoreControlProfiles** property within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="da330-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="da330-105">Permissions</span></span>

<span data-ttu-id="da330-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="da330-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da330-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="da330-108">Permission type</span></span>      | <span data-ttu-id="da330-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="da330-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da330-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="da330-110">Delegated (work or school account)</span></span> |   <span data-ttu-id="da330-111">SecurityEvents。</span><span class="sxs-lookup"><span data-stu-id="da330-111">SecurityEvents.ReadWrite.All.</span></span>  |
|<span data-ttu-id="da330-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="da330-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="da330-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da330-113">Not supported.</span></span>  |
|<span data-ttu-id="da330-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="da330-114">Application</span></span> | <span data-ttu-id="da330-115">SecurityEvents。</span><span class="sxs-lookup"><span data-stu-id="da330-115">SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="da330-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="da330-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="da330-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="da330-117">Request headers</span></span>

| <span data-ttu-id="da330-118">名前</span><span class="sxs-lookup"><span data-stu-id="da330-118">Name</span></span>       | <span data-ttu-id="da330-119">説明</span><span class="sxs-lookup"><span data-stu-id="da330-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="da330-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="da330-120">Authorization</span></span>  | <span data-ttu-id="da330-121">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="da330-121">Bearer {code}.</span></span> <span data-ttu-id="da330-122">必須です。</span><span class="sxs-lookup"><span data-stu-id="da330-122">Required.</span></span>|
|<span data-ttu-id="da330-123">Prefer</span><span class="sxs-lookup"><span data-stu-id="da330-123">Prefer</span></span> | <span data-ttu-id="da330-124">戻り値 = 表現。</span><span class="sxs-lookup"><span data-stu-id="da330-124">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da330-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="da330-125">Request body</span></span>

<span data-ttu-id="da330-126">要求本文で、更新する必要のある関連フィールドの値の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="da330-126">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="da330-127">次の表に、secureScoreControlProfile で更新できるフィールドを示します。</span><span class="sxs-lookup"><span data-stu-id="da330-127">The following table lists the fields that can be updated for a secureScoreControlProfile.</span></span> <span data-ttu-id="da330-128">要求本文に含まれていない既存のプロパティの値は変更されません。</span><span class="sxs-lookup"><span data-stu-id="da330-128">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="da330-129">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="da330-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="da330-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da330-130">Property</span></span>   | <span data-ttu-id="da330-131">型</span><span class="sxs-lookup"><span data-stu-id="da330-131">Type</span></span> |<span data-ttu-id="da330-132">説明</span><span class="sxs-lookup"><span data-stu-id="da330-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da330-133">assignedTo</span><span class="sxs-lookup"><span data-stu-id="da330-133">assignedTo</span></span>|<span data-ttu-id="da330-134">String</span><span class="sxs-lookup"><span data-stu-id="da330-134">String</span></span>|<span data-ttu-id="da330-135">トリアージ、実装、または修復のために、コントロールが割り当てられているアナリストの名前。</span><span class="sxs-lookup"><span data-stu-id="da330-135">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="da330-136">tenantNote</span><span class="sxs-lookup"><span data-stu-id="da330-136">tenantNote</span></span>|<span data-ttu-id="da330-137">String</span><span class="sxs-lookup"><span data-stu-id="da330-137">String</span></span>|<span data-ttu-id="da330-138">コントロールに関するアナリストコメント (カスタマーコントロール管理向け)。</span><span class="sxs-lookup"><span data-stu-id="da330-138">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="da330-139">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="da330-139">controlStateUpdates</span></span>| <span data-ttu-id="da330-140">String</span><span class="sxs-lookup"><span data-stu-id="da330-140">String</span></span>|<span data-ttu-id="da330-141">コントロールに対するアナリスト主導の設定。</span><span class="sxs-lookup"><span data-stu-id="da330-141">Analyst driven setting on the control.</span></span> <span data-ttu-id="da330-142">可能な値は、`ignore`、`thirdParty`、`reviewed` です。</span><span class="sxs-lookup"><span data-stu-id="da330-142">Possible values are: `ignore`, `thirdParty`, `reviewed`.</span></span>|


## <a name="response"></a><span data-ttu-id="da330-143">応答</span><span class="sxs-lookup"><span data-stu-id="da330-143">Response</span></span>

<span data-ttu-id="da330-144">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="da330-144">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="da330-145">オプションの要求ヘッダーが使用されている場合、 `200 OK`メソッドは応答コードと、応答本文で更新された[securescorecontrolprofiles の](../resources/securescorecontrolprofiles.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="da330-145">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da330-146">例</span><span class="sxs-lookup"><span data-stu-id="da330-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="da330-147">要求</span><span class="sxs-lookup"><span data-stu-id="da330-147">Request</span></span>

<span data-ttu-id="da330-148">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="da330-148">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="da330-149">プロトコル</span><span class="sxs-lookup"><span data-stu-id="da330-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/secureScoreControlProfiles/AdminMFA
Content-type: application/json

{
  "controlStateUpdates": "controlStateUpdates-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="da330-150">C#</span><span class="sxs-lookup"><span data-stu-id="da330-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-update-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="da330-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da330-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-update-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="da330-152">目的-C</span><span class="sxs-lookup"><span data-stu-id="da330-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-update-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="da330-153">応答</span><span class="sxs-lookup"><span data-stu-id="da330-153">Response</span></span>

<span data-ttu-id="da330-154">成功応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="da330-154">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
} -->

```http
HTTP/1.1 204 No Content
```




<!--
{
  "type": "#page.annotation",
  "description": "Update secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
