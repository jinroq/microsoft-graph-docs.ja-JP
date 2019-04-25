---
title: secureScoreControlProfiles の更新
description: 任意の統合ソリューション内の編集可能な securescorecontrolprofiles のプロパティを更新して、担当者または tenantnote などのさまざまなプロパティを変更します。
localization_priority: Normal
ms.openlocfilehash: 711fd29e906822def0a5f4b5fbca13a1d73732d6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545631"
---
# <a name="update-securescorecontrolprofiles"></a><span data-ttu-id="824d0-103">secureScoreControlProfiles の更新</span><span class="sxs-lookup"><span data-stu-id="824d0-103">Update secureScoreControlProfiles</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="824d0-104">任意の統合ソリューション内の編集可能な**securescorecontrolprofiles の**プロパティを更新して、**担当者**または**tenantnote**などのさまざまなプロパティを変更します。</span><span class="sxs-lookup"><span data-stu-id="824d0-104">Update an editable **secureScoreControlProfiles** property within any integrated solution to change various properties, such as **assignedTo** or **tenantNote**.</span></span>

## <a name="permissions"></a><span data-ttu-id="824d0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="824d0-105">Permissions</span></span>

<span data-ttu-id="824d0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="824d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="824d0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="824d0-108">Permission type</span></span>      | <span data-ttu-id="824d0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="824d0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="824d0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="824d0-110">Delegated (work or school account)</span></span> |   <span data-ttu-id="824d0-111">securityevents。</span><span class="sxs-lookup"><span data-stu-id="824d0-111">SecurityEvents.ReadWrite.All.</span></span>  |
|<span data-ttu-id="824d0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="824d0-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="824d0-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="824d0-113">Not supported.</span></span>  |
|<span data-ttu-id="824d0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="824d0-114">Application</span></span> | <span data-ttu-id="824d0-115">securityevents。</span><span class="sxs-lookup"><span data-stu-id="824d0-115">SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="824d0-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="824d0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="824d0-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="824d0-117">Request headers</span></span>

| <span data-ttu-id="824d0-118">名前</span><span class="sxs-lookup"><span data-stu-id="824d0-118">Name</span></span>       | <span data-ttu-id="824d0-119">説明</span><span class="sxs-lookup"><span data-stu-id="824d0-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="824d0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="824d0-120">Authorization</span></span>  | <span data-ttu-id="824d0-121">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="824d0-121">Bearer {code}.</span></span> <span data-ttu-id="824d0-122">必須。</span><span class="sxs-lookup"><span data-stu-id="824d0-122">Required.</span></span>|
|<span data-ttu-id="824d0-123">Prefer</span><span class="sxs-lookup"><span data-stu-id="824d0-123">Prefer</span></span> | <span data-ttu-id="824d0-124">戻り値 = 表現。</span><span class="sxs-lookup"><span data-stu-id="824d0-124">return=representation.</span></span> |

## <a name="request-body"></a><span data-ttu-id="824d0-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="824d0-125">Request body</span></span>

<span data-ttu-id="824d0-126">要求本文で、更新する必要のある関連フィールドの値の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="824d0-126">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="824d0-127">次の表に、secureScoreControlProfile で更新できるフィールドを示します。</span><span class="sxs-lookup"><span data-stu-id="824d0-127">The following table lists the fields that can be updated for a secureScoreControlProfile.</span></span> <span data-ttu-id="824d0-128">要求本文に含まれていない既存のプロパティの値は変更されません。</span><span class="sxs-lookup"><span data-stu-id="824d0-128">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="824d0-129">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="824d0-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="824d0-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="824d0-130">Property</span></span>   | <span data-ttu-id="824d0-131">型</span><span class="sxs-lookup"><span data-stu-id="824d0-131">Type</span></span> |<span data-ttu-id="824d0-132">説明</span><span class="sxs-lookup"><span data-stu-id="824d0-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="824d0-133">assignedTo</span><span class="sxs-lookup"><span data-stu-id="824d0-133">assignedTo</span></span>|<span data-ttu-id="824d0-134">String</span><span class="sxs-lookup"><span data-stu-id="824d0-134">String</span></span>|<span data-ttu-id="824d0-135">トリアージ、実装、または修復のために、コントロールが割り当てられているアナリストの名前。</span><span class="sxs-lookup"><span data-stu-id="824d0-135">Name of the analyst the control is assigned to for triage, implementation, or remediation.</span></span>|
|<span data-ttu-id="824d0-136">tenantnote</span><span class="sxs-lookup"><span data-stu-id="824d0-136">tenantNote</span></span>|<span data-ttu-id="824d0-137">String</span><span class="sxs-lookup"><span data-stu-id="824d0-137">String</span></span>|<span data-ttu-id="824d0-138">コントロールに関するアナリストコメント (カスタマーコントロール管理向け)。</span><span class="sxs-lookup"><span data-stu-id="824d0-138">Analyst comments on the control (for customer control management).</span></span>|
|<span data-ttu-id="824d0-139">controlstateupdates</span><span class="sxs-lookup"><span data-stu-id="824d0-139">controlStateUpdates</span></span>| <span data-ttu-id="824d0-140">String</span><span class="sxs-lookup"><span data-stu-id="824d0-140">String</span></span>|<span data-ttu-id="824d0-141">コントロールに対するアナリスト主導の設定。</span><span class="sxs-lookup"><span data-stu-id="824d0-141">Analyst driven setting on the control.</span></span> <span data-ttu-id="824d0-142">可能な値は、`ignore`、`thirdParty`、`reviewed` です。</span><span class="sxs-lookup"><span data-stu-id="824d0-142">Possible values are: `ignore`, `thirdParty`, `reviewed`.</span></span>|


## <a name="response"></a><span data-ttu-id="824d0-143">応答</span><span class="sxs-lookup"><span data-stu-id="824d0-143">Response</span></span>

<span data-ttu-id="824d0-144">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="824d0-144">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="824d0-145">オプションの要求ヘッダーが使用されている場合、 `200 OK`メソッドは応答コードと、応答本文で更新された[securescorecontrolprofiles の](../resources/securescorecontrolprofiles.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="824d0-145">If the optional request header is used, the method returns a `200 OK` response code and the updated [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="824d0-146">例</span><span class="sxs-lookup"><span data-stu-id="824d0-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="824d0-147">要求</span><span class="sxs-lookup"><span data-stu-id="824d0-147">Request</span></span>

<span data-ttu-id="824d0-148">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="824d0-148">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="824d0-149">応答</span><span class="sxs-lookup"><span data-stu-id="824d0-149">Response</span></span>

<span data-ttu-id="824d0-150">成功応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="824d0-150">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
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
    "Error: /api-reference/beta/api/securescorecontrolprofiles-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
