---
title: アラートを更新する
description: ソリューション間でアラートの状態と割り当てを同期させるために、任意の統合ソリューション内の編集可能な**警告**プロパティを更新します。 このメソッドは、参照される警告 ID のレコードを持つソリューションを更新します。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 4fc4b99384cbb01a94460978f7d0b42cae3fa8aa
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365819"
---
# <a name="update-alert"></a><span data-ttu-id="695c2-104">アラートを更新する</span><span class="sxs-lookup"><span data-stu-id="695c2-104">Update alert</span></span>

<span data-ttu-id="695c2-105">ソリューション間でアラートの状態と割り当てを同期させるために、任意の統合ソリューション内の編集可能な**警告**プロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="695c2-105">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="695c2-106">このメソッドは、参照される警告 ID のレコードを持つソリューションを更新します。</span><span class="sxs-lookup"><span data-stu-id="695c2-106">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="695c2-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="695c2-107">Permissions</span></span>

<span data-ttu-id="695c2-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="695c2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="695c2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="695c2-110">Permission type</span></span>                        | <span data-ttu-id="695c2-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="695c2-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="695c2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="695c2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="695c2-113">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="695c2-113">SecurityEvents.ReadWrite.All</span></span>        |
| <span data-ttu-id="695c2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="695c2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="695c2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="695c2-115">Not supported.</span></span>                      |
| <span data-ttu-id="695c2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="695c2-116">Application</span></span>                            | <span data-ttu-id="695c2-117">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="695c2-117">SecurityEvents.ReadWrite.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="695c2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="695c2-118">HTTP request</span></span>

> <span data-ttu-id="695c2-119">**注:** このメソッドを使用\*\*\*\* して、 `provider`および`vendor`を含む vendorInformation というパラメーターとして、警告 ID を含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="695c2-119">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="695c2-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="695c2-120">Request headers</span></span>

| <span data-ttu-id="695c2-121">名前</span><span class="sxs-lookup"><span data-stu-id="695c2-121">Name</span></span>          | <span data-ttu-id="695c2-122">説明</span><span class="sxs-lookup"><span data-stu-id="695c2-122">Description</span></span>              |
|:--------------|:-------------------------|
| <span data-ttu-id="695c2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="695c2-123">Authorization</span></span> | <span data-ttu-id="695c2-124">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="695c2-124">Bearer {code}.</span></span> <span data-ttu-id="695c2-125">必須です。</span><span class="sxs-lookup"><span data-stu-id="695c2-125">Required.</span></span> |
| <span data-ttu-id="695c2-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="695c2-126">Prefer</span></span>        | <span data-ttu-id="695c2-127">戻り値 = 表現</span><span class="sxs-lookup"><span data-stu-id="695c2-127">return=representation</span></span>    |

## <a name="request-body"></a><span data-ttu-id="695c2-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="695c2-128">Request body</span></span>

<span data-ttu-id="695c2-129">要求本文で、更新する必要のある関連フィールドの値の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="695c2-129">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="695c2-130">本文には、有効`vendorInformation`な`provider` `vendor`フィールドとフィールドのプロパティが含まれて**いる必要があり**ます。</span><span class="sxs-lookup"><span data-stu-id="695c2-130">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="695c2-131">次の表に、通知に対して更新できるフィールドを示します。</span><span class="sxs-lookup"><span data-stu-id="695c2-131">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="695c2-132">要求本文に含まれていない既存のプロパティの値は変更されません。</span><span class="sxs-lookup"><span data-stu-id="695c2-132">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="695c2-133">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="695c2-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="695c2-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="695c2-134">Property</span></span>          | <span data-ttu-id="695c2-135">型</span><span class="sxs-lookup"><span data-stu-id="695c2-135">Type</span></span>                                                                   | <span data-ttu-id="695c2-136">説明</span><span class="sxs-lookup"><span data-stu-id="695c2-136">Description</span></span> |
|:------------------|:-----------------------------------------------------------------------|:--|
| <span data-ttu-id="695c2-137">assignedTo</span><span class="sxs-lookup"><span data-stu-id="695c2-137">assignedTo</span></span>        | <span data-ttu-id="695c2-138">String</span><span class="sxs-lookup"><span data-stu-id="695c2-138">String</span></span>                                                                 | <span data-ttu-id="695c2-139">トリアージ、調査、または修復のためにアラートが割り当てられたアナリストの名前。</span><span class="sxs-lookup"><span data-stu-id="695c2-139">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span> |
| <span data-ttu-id="695c2-140">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="695c2-140">closedDateTime</span></span>    | <span data-ttu-id="695c2-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="695c2-141">DateTimeOffset</span></span>                                                         | <span data-ttu-id="695c2-142">警告が閉じられた時刻。</span><span class="sxs-lookup"><span data-stu-id="695c2-142">Time at which the alert was closed.</span></span> <span data-ttu-id="695c2-143">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="695c2-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="695c2-144">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="695c2-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
| <span data-ttu-id="695c2-145">comments</span><span class="sxs-lookup"><span data-stu-id="695c2-145">comments</span></span>          | <span data-ttu-id="695c2-146">String コレクション</span><span class="sxs-lookup"><span data-stu-id="695c2-146">String collection</span></span>                                                      | <span data-ttu-id="695c2-147">アラートに関するアナリストのコメント (顧客の警告管理)。</span><span class="sxs-lookup"><span data-stu-id="695c2-147">Analyst comments on the alert (for customer alert management).</span></span> |
| <span data-ttu-id="695c2-148">feedback</span><span class="sxs-lookup"><span data-stu-id="695c2-148">feedback</span></span>          | <span data-ttu-id="695c2-149">alertFeedback</span><span class="sxs-lookup"><span data-stu-id="695c2-149">alertFeedback</span></span>                                                          | <span data-ttu-id="695c2-150">警告に関するアナリストのフィードバック。</span><span class="sxs-lookup"><span data-stu-id="695c2-150">Analyst feedback on the alert.</span></span> <span data-ttu-id="695c2-151">使用可能な値は、`unknown`、`truePositive`、`falsePositive`、`benignPositive` です。</span><span class="sxs-lookup"><span data-stu-id="695c2-151">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span> |
| <span data-ttu-id="695c2-152">status</span><span class="sxs-lookup"><span data-stu-id="695c2-152">status</span></span>            | <span data-ttu-id="695c2-153">alertStatus</span><span class="sxs-lookup"><span data-stu-id="695c2-153">alertStatus</span></span>                                                            | <span data-ttu-id="695c2-154">アラートライフサイクルの状態 (ステージ)。</span><span class="sxs-lookup"><span data-stu-id="695c2-154">Alert life cycle status (stage).</span></span> <span data-ttu-id="695c2-155">使用可能な値は、`unknown`、`newAlert`、`inProgress`、`resolved` です。</span><span class="sxs-lookup"><span data-stu-id="695c2-155">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span> |
| <span data-ttu-id="695c2-156">タグ</span><span class="sxs-lookup"><span data-stu-id="695c2-156">tags</span></span>              | <span data-ttu-id="695c2-157">String collection</span><span class="sxs-lookup"><span data-stu-id="695c2-157">String collection</span></span>                                                      | <span data-ttu-id="695c2-158">通知に適用することができ、フィルター条件として機能することができる、ユーザー定義のラベル (たとえば、"HVA"、"のこぎり" など)。</span><span class="sxs-lookup"><span data-stu-id="695c2-158">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span> |
| <span data-ttu-id="695c2-159">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="695c2-159">vendorInformation</span></span> | [<span data-ttu-id="695c2-160">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="695c2-160">securityVendorInformation</span></span>](../resources/securityvendorinformation.md) | <span data-ttu-id="695c2-161">セキュリティ製品/サービスの仕入先、プロバイダー、サブプロバイダーに関する詳細を含む複合型 (たとえば、仕入先 = Microsoft、プロバイダー = Windows Defender ATP、サブプロバイダー = AppLocker)。</span><span class="sxs-lookup"><span data-stu-id="695c2-161">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="695c2-162">**プロバイダーおよびベンダーフィールドは必須です。**</span><span class="sxs-lookup"><span data-stu-id="695c2-162">**Provider and vendor fields are required.**</span></span> |

## <a name="response"></a><span data-ttu-id="695c2-163">応答</span><span class="sxs-lookup"><span data-stu-id="695c2-163">Response</span></span>

<span data-ttu-id="695c2-164">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="695c2-164">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="695c2-165">オプションの要求ヘッダーが使用されている場合、 `200 OK`メソッドは応答コードと、応答本文で更新された[alert](../resources/alert.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="695c2-165">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="695c2-166">例</span><span class="sxs-lookup"><span data-stu-id="695c2-166">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="695c2-167">例 1: 希望するヘッダーのない要求</span><span class="sxs-lookup"><span data-stu-id="695c2-167">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="695c2-168">要求</span><span class="sxs-lookup"><span data-stu-id="695c2-168">Request</span></span>

<span data-ttu-id="695c2-169">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="695c2-169">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="695c2-170">プロトコル</span><span class="sxs-lookup"><span data-stu-id="695c2-170">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="695c2-171">C#</span><span class="sxs-lookup"><span data-stu-id="695c2-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-alert-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="695c2-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="695c2-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-alert-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="695c2-173">目的-C</span><span class="sxs-lookup"><span data-stu-id="695c2-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-alert-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="695c2-174">Java</span><span class="sxs-lookup"><span data-stu-id="695c2-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-alert-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="695c2-175">応答</span><span class="sxs-lookup"><span data-stu-id="695c2-175">Response</span></span>

<span data-ttu-id="695c2-176">成功応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="695c2-176">The following is an example of a successful response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="695c2-177">例 2: 要求ヘッダーを使用した要求</span><span class="sxs-lookup"><span data-stu-id="695c2-177">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="695c2-178">要求</span><span class="sxs-lookup"><span data-stu-id="695c2-178">Request</span></span>

<span data-ttu-id="695c2-179">次の例は、 `Prefer`要求ヘッダーを含む要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="695c2-179">The following example shows a request that includes the `Prefer` request header.</span></span>

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

#### <a name="response"></a><span data-ttu-id="695c2-180">応答</span><span class="sxs-lookup"><span data-stu-id="695c2-180">Response</span></span>

<span data-ttu-id="695c2-181">オプション`Prefer: return=representation`の要求ヘッダーを使用する場合の応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="695c2-181">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

> <span data-ttu-id="695c2-p110">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="695c2-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  ]
}-->
