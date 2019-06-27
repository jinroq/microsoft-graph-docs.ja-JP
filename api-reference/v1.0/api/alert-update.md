---
title: アラートを更新する
description: ソリューション間でアラートの状態と割り当てを同期させるために、任意の統合ソリューション内の編集可能な**警告**プロパティを更新します。 このメソッドは、参照される警告 ID のレコードを持つソリューションを更新します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: d448a7d23f7370650f7ab621fb0f467a3726bce1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264835"
---
# <a name="update-alert"></a><span data-ttu-id="46d35-104">アラートを更新する</span><span class="sxs-lookup"><span data-stu-id="46d35-104">Update alert</span></span>

<span data-ttu-id="46d35-105">ソリューション間でアラートの状態と割り当てを同期させるために、任意の統合ソリューション内の編集可能な**警告**プロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="46d35-105">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="46d35-106">このメソッドは、参照される警告 ID のレコードを持つソリューションを更新します。</span><span class="sxs-lookup"><span data-stu-id="46d35-106">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="46d35-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="46d35-107">Permissions</span></span>

<span data-ttu-id="46d35-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="46d35-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="46d35-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="46d35-110">Permission type</span></span>                        | <span data-ttu-id="46d35-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="46d35-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="46d35-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="46d35-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="46d35-113">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46d35-113">SecurityEvents.ReadWrite.All</span></span>        |
| <span data-ttu-id="46d35-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="46d35-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46d35-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46d35-115">Not supported.</span></span>                      |
| <span data-ttu-id="46d35-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="46d35-116">Application</span></span>                            | <span data-ttu-id="46d35-117">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46d35-117">SecurityEvents.ReadWrite.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="46d35-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="46d35-118">HTTP request</span></span>

> <span data-ttu-id="46d35-119">**注:** このメソッドを使用\*\*\*\* して、 `provider`および`vendor`を含む vendorInformation というパラメーターとして、警告 ID を含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="46d35-119">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="46d35-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="46d35-120">Request headers</span></span>

| <span data-ttu-id="46d35-121">名前</span><span class="sxs-lookup"><span data-stu-id="46d35-121">Name</span></span>          | <span data-ttu-id="46d35-122">説明</span><span class="sxs-lookup"><span data-stu-id="46d35-122">Description</span></span>              |
|:--------------|:-------------------------|
| <span data-ttu-id="46d35-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="46d35-123">Authorization</span></span> | <span data-ttu-id="46d35-124">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="46d35-124">Bearer {code}.</span></span> <span data-ttu-id="46d35-125">必須です。</span><span class="sxs-lookup"><span data-stu-id="46d35-125">Required.</span></span> |
| <span data-ttu-id="46d35-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="46d35-126">Prefer</span></span>        | <span data-ttu-id="46d35-127">戻り値 = 表現</span><span class="sxs-lookup"><span data-stu-id="46d35-127">return=representation</span></span>    |

## <a name="request-body"></a><span data-ttu-id="46d35-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="46d35-128">Request body</span></span>

<span data-ttu-id="46d35-129">要求本文で、更新する必要のある関連フィールドの値の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="46d35-129">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="46d35-130">本文には、有効`vendorInformation`な`provider` `vendor`フィールドとフィールドのプロパティが含まれて**いる必要があり**ます。</span><span class="sxs-lookup"><span data-stu-id="46d35-130">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="46d35-131">次の表に、通知に対して更新できるフィールドを示します。</span><span class="sxs-lookup"><span data-stu-id="46d35-131">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="46d35-132">要求本文に含まれていない既存のプロパティの値は変更されません。</span><span class="sxs-lookup"><span data-stu-id="46d35-132">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="46d35-133">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="46d35-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="46d35-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46d35-134">Property</span></span>          | <span data-ttu-id="46d35-135">型</span><span class="sxs-lookup"><span data-stu-id="46d35-135">Type</span></span>                                                                   | <span data-ttu-id="46d35-136">説明</span><span class="sxs-lookup"><span data-stu-id="46d35-136">Description</span></span> |
|:------------------|:-----------------------------------------------------------------------|:--|
| <span data-ttu-id="46d35-137">assignedTo</span><span class="sxs-lookup"><span data-stu-id="46d35-137">assignedTo</span></span>        | <span data-ttu-id="46d35-138">String</span><span class="sxs-lookup"><span data-stu-id="46d35-138">String</span></span>                                                                 | <span data-ttu-id="46d35-139">トリアージ、調査、または修復のためにアラートが割り当てられたアナリストの名前。</span><span class="sxs-lookup"><span data-stu-id="46d35-139">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span> |
| <span data-ttu-id="46d35-140">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="46d35-140">closedDateTime</span></span>    | <span data-ttu-id="46d35-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46d35-141">DateTimeOffset</span></span>                                                         | <span data-ttu-id="46d35-142">警告が閉じられた時刻。</span><span class="sxs-lookup"><span data-stu-id="46d35-142">Time at which the alert was closed.</span></span> <span data-ttu-id="46d35-143">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="46d35-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="46d35-144">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="46d35-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
| <span data-ttu-id="46d35-145">comments</span><span class="sxs-lookup"><span data-stu-id="46d35-145">comments</span></span>          | <span data-ttu-id="46d35-146">String コレクション</span><span class="sxs-lookup"><span data-stu-id="46d35-146">String collection</span></span>                                                      | <span data-ttu-id="46d35-147">アラートに関するアナリストのコメント (顧客の警告管理)。</span><span class="sxs-lookup"><span data-stu-id="46d35-147">Analyst comments on the alert (for customer alert management).</span></span> |
| <span data-ttu-id="46d35-148">feedback</span><span class="sxs-lookup"><span data-stu-id="46d35-148">feedback</span></span>          | <span data-ttu-id="46d35-149">alertFeedback</span><span class="sxs-lookup"><span data-stu-id="46d35-149">alertFeedback</span></span>                                                          | <span data-ttu-id="46d35-150">警告に関するアナリストのフィードバック。</span><span class="sxs-lookup"><span data-stu-id="46d35-150">Analyst feedback on the alert.</span></span> <span data-ttu-id="46d35-151">使用可能な値は、`unknown`、`truePositive`、`falsePositive`、`benignPositive` です。</span><span class="sxs-lookup"><span data-stu-id="46d35-151">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span> |
| <span data-ttu-id="46d35-152">status</span><span class="sxs-lookup"><span data-stu-id="46d35-152">status</span></span>            | <span data-ttu-id="46d35-153">alertStatus</span><span class="sxs-lookup"><span data-stu-id="46d35-153">alertStatus</span></span>                                                            | <span data-ttu-id="46d35-154">アラートライフサイクルの状態 (ステージ)。</span><span class="sxs-lookup"><span data-stu-id="46d35-154">Alert life cycle status (stage).</span></span> <span data-ttu-id="46d35-155">使用可能な値は、`unknown`、`newAlert`、`inProgress`、`resolved` です。</span><span class="sxs-lookup"><span data-stu-id="46d35-155">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span> |
| <span data-ttu-id="46d35-156">タグ</span><span class="sxs-lookup"><span data-stu-id="46d35-156">tags</span></span>              | <span data-ttu-id="46d35-157">String collection</span><span class="sxs-lookup"><span data-stu-id="46d35-157">String collection</span></span>                                                      | <span data-ttu-id="46d35-158">通知に適用することができ、フィルター条件として機能することができる、ユーザー定義のラベル (たとえば、"HVA"、"のこぎり" など)。</span><span class="sxs-lookup"><span data-stu-id="46d35-158">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span> |
| <span data-ttu-id="46d35-159">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="46d35-159">vendorInformation</span></span> | [<span data-ttu-id="46d35-160">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="46d35-160">securityVendorInformation</span></span>](../resources/securityvendorinformation.md) | <span data-ttu-id="46d35-161">セキュリティ製品/サービスの仕入先、プロバイダー、サブプロバイダーに関する詳細を含む複合型 (たとえば、仕入先 = Microsoft、プロバイダー = Windows Defender ATP、サブプロバイダー = AppLocker)。</span><span class="sxs-lookup"><span data-stu-id="46d35-161">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="46d35-162">**プロバイダーおよびベンダーフィールドは必須です。**</span><span class="sxs-lookup"><span data-stu-id="46d35-162">**Provider and vendor fields are required.**</span></span> |

## <a name="response"></a><span data-ttu-id="46d35-163">応答</span><span class="sxs-lookup"><span data-stu-id="46d35-163">Response</span></span>

<span data-ttu-id="46d35-164">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="46d35-164">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="46d35-165">オプションの要求ヘッダーが使用されている場合、 `200 OK`メソッドは応答コードと、応答本文で更新された[alert](../resources/alert.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="46d35-165">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="46d35-166">例</span><span class="sxs-lookup"><span data-stu-id="46d35-166">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="46d35-167">例 1: 希望するヘッダーのない要求</span><span class="sxs-lookup"><span data-stu-id="46d35-167">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="46d35-168">要求</span><span class="sxs-lookup"><span data-stu-id="46d35-168">Request</span></span>

<span data-ttu-id="46d35-169">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="46d35-169">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
Content-type: application/json

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": [
    "String"
  ],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": [
    "String"
  ],
  "vendorInformation": {
    "provider": "String",
    "vendor": "String"
  }
}
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="46d35-170">応答</span><span class="sxs-lookup"><span data-stu-id="46d35-170">Response</span></span>

<span data-ttu-id="46d35-171">成功応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="46d35-171">The following is an example of a successful response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="46d35-172">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="46d35-172">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="46d35-173">C#</span><span class="sxs-lookup"><span data-stu-id="46d35-173">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_alert-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="46d35-174">Javascript</span><span class="sxs-lookup"><span data-stu-id="46d35-174">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_alert-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="46d35-175">目的-C</span><span class="sxs-lookup"><span data-stu-id="46d35-175">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_alert-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="46d35-176">例 2: 要求ヘッダーを使用した要求</span><span class="sxs-lookup"><span data-stu-id="46d35-176">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="46d35-177">要求</span><span class="sxs-lookup"><span data-stu-id="46d35-177">Request</span></span>

<span data-ttu-id="46d35-178">次の例は、 `Prefer`要求ヘッダーを含む要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="46d35-178">The following example shows a request that includes the `Prefer` request header.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
Content-type: application/json
Prefer: return=representation

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": [
    "String"
  ],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": [
    "String"
  ],
  "vendorInformation": {
    "provider": "String",
    "vendor": "String"
  }
}
```

#### <a name="response"></a><span data-ttu-id="46d35-179">応答</span><span class="sxs-lookup"><span data-stu-id="46d35-179">Response</span></span>

<span data-ttu-id="46d35-180">オプション`Prefer: return=representation`の要求ヘッダーを使用する場合の応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="46d35-180">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

> <span data-ttu-id="46d35-p110">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="46d35-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "activityGroupName": "activityGroupName-value",
  "assignedTo": "assignedTo-value",
  "azureSubscriptionId": "azureSubscriptionId-value",
  "azureTenantId": "azureTenantId-value",
  "category": "category-value",
  "closedDateTime": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update alert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/alert-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/alert-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/alert-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/alert-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/alert-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
