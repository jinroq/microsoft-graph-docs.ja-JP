---
title: アラートを更新する
description: ソリューション間でアラートの状態と割り当てを同期させるために、任意の統合ソリューション内の編集可能な警告プロパティを更新します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 47c5499a49ce6e9f4bae7962a0a30e26a7290ed2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855377"
---
# <a name="update-alert"></a><span data-ttu-id="9ec7a-103">アラートを更新する</span><span class="sxs-lookup"><span data-stu-id="9ec7a-103">Update alert</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ec7a-104">ソリューション間でアラートの状態と割り当てを同期させるために、任意の統合ソリューション内の編集可能な**警告**プロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-104">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="9ec7a-105">このメソッドは、参照される警告 ID のレコードを持つソリューションを更新します。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-105">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ec7a-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9ec7a-106">Permissions</span></span>

<span data-ttu-id="9ec7a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ec7a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9ec7a-109">Permission type</span></span>      | <span data-ttu-id="9ec7a-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9ec7a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ec7a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9ec7a-111">Delegated (work or school account)</span></span> |   <span data-ttu-id="9ec7a-112">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ec7a-112">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="9ec7a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9ec7a-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9ec7a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-114">Not supported.</span></span>  |
|<span data-ttu-id="9ec7a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9ec7a-115">Application</span></span> | <span data-ttu-id="9ec7a-116">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ec7a-116">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ec7a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9ec7a-117">HTTP request</span></span>

> <span data-ttu-id="9ec7a-118">**注:** このメソッドを使用\*\*\*\* して、 `provider`および`vendor`を含む vendorInformation というパラメーターとして、警告 ID を含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-118">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="9ec7a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9ec7a-119">Request headers</span></span>

| <span data-ttu-id="9ec7a-120">名前</span><span class="sxs-lookup"><span data-stu-id="9ec7a-120">Name</span></span>       | <span data-ttu-id="9ec7a-121">説明</span><span class="sxs-lookup"><span data-stu-id="9ec7a-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9ec7a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ec7a-122">Authorization</span></span>  | <span data-ttu-id="9ec7a-123">ベアラー {code}。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-123">Bearer {code}.</span></span> <span data-ttu-id="9ec7a-124">必須です。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-124">Required.</span></span>|
|<span data-ttu-id="9ec7a-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="9ec7a-125">Prefer</span></span> | <span data-ttu-id="9ec7a-126">戻り値 = 表現</span><span class="sxs-lookup"><span data-stu-id="9ec7a-126">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ec7a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9ec7a-127">Request body</span></span>

<span data-ttu-id="9ec7a-128">要求本文で、更新する必要のある関連フィールドの値の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-128">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="9ec7a-129">本文には、有効`vendorInformation`な`provider` `vendor`フィールドとフィールドのプロパティが含まれて**いる必要があり**ます。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-129">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="9ec7a-130">次の表に、通知に対して更新できるフィールドを示します。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-130">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="9ec7a-131">要求本文に含まれていない既存のプロパティの値は変更されません。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-131">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="9ec7a-132">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9ec7a-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9ec7a-133">Property</span></span>   | <span data-ttu-id="9ec7a-134">型</span><span class="sxs-lookup"><span data-stu-id="9ec7a-134">Type</span></span> |<span data-ttu-id="9ec7a-135">説明</span><span class="sxs-lookup"><span data-stu-id="9ec7a-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ec7a-136">assignedTo</span><span class="sxs-lookup"><span data-stu-id="9ec7a-136">assignedTo</span></span>|<span data-ttu-id="9ec7a-137">String</span><span class="sxs-lookup"><span data-stu-id="9ec7a-137">String</span></span>|<span data-ttu-id="9ec7a-138">トリアージ、調査、または修復のためにアラートが割り当てられたアナリストの名前。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-138">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="9ec7a-139">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ec7a-139">closedDateTime</span></span>|<span data-ttu-id="9ec7a-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ec7a-140">DateTimeOffset</span></span>|<span data-ttu-id="9ec7a-141">警告が閉じられた時刻。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-141">Time at which the alert was closed.</span></span> <span data-ttu-id="9ec7a-142">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9ec7a-143">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9ec7a-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="9ec7a-144">comments</span><span class="sxs-lookup"><span data-stu-id="9ec7a-144">comments</span></span>|<span data-ttu-id="9ec7a-145">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9ec7a-145">String collection</span></span>|<span data-ttu-id="9ec7a-146">アラートに関するアナリストのコメント (顧客の警告管理)。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-146">Analyst comments on the alert (for customer alert management).</span></span>|
|<span data-ttu-id="9ec7a-147">feedback</span><span class="sxs-lookup"><span data-stu-id="9ec7a-147">feedback</span></span>|<span data-ttu-id="9ec7a-148">alertFeedback 列挙</span><span class="sxs-lookup"><span data-stu-id="9ec7a-148">alertFeedback enum</span></span>|<span data-ttu-id="9ec7a-149">警告に関するアナリストのフィードバック。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-149">Analyst feedback on the alert.</span></span> <span data-ttu-id="9ec7a-150">使用可能な値は、`unknown`、`truePositive`、`falsePositive`、`benignPositive` です。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-150">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="9ec7a-151">status</span><span class="sxs-lookup"><span data-stu-id="9ec7a-151">status</span></span>|<span data-ttu-id="9ec7a-152">alertStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="9ec7a-152">alertStatus enum</span></span>|<span data-ttu-id="9ec7a-153">アラートライフサイクルの状態 (ステージ)。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-153">Alert life cycle status (stage).</span></span> <span data-ttu-id="9ec7a-154">使用可能な値は、`unknown`、`newAlert`、`inProgress`、`resolved` です。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-154">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="9ec7a-155">タグ</span><span class="sxs-lookup"><span data-stu-id="9ec7a-155">tags</span></span>|<span data-ttu-id="9ec7a-156">String collection</span><span class="sxs-lookup"><span data-stu-id="9ec7a-156">String collection</span></span>|<span data-ttu-id="9ec7a-157">通知に適用することができ、フィルター条件として機能することができる、ユーザー定義のラベル (たとえば、"HVA"、"のこぎり" など)。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-157">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="9ec7a-158">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="9ec7a-158">vendorInformation</span></span> |[<span data-ttu-id="9ec7a-159">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="9ec7a-159">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="9ec7a-160">セキュリティ製品/サービスの仕入先、プロバイダー、サブプロバイダーに関する詳細を含む複合型 (たとえば、仕入先 = Microsoft、プロバイダー = Windows Defender ATP、サブプロバイダー = AppLocker)。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-160">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="9ec7a-161">**プロバイダーおよびベンダーフィールドは必須です。**</span><span class="sxs-lookup"><span data-stu-id="9ec7a-161">**Provider and vendor fields are required.**</span></span>|

## <a name="response"></a><span data-ttu-id="9ec7a-162">応答</span><span class="sxs-lookup"><span data-stu-id="9ec7a-162">Response</span></span>

<span data-ttu-id="9ec7a-163">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-163">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="9ec7a-164">オプションの要求ヘッダーが使用されている場合、 `200 OK`メソッドは応答コードと、応答本文で更新された[alert](../resources/alert.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-164">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9ec7a-165">例</span><span class="sxs-lookup"><span data-stu-id="9ec7a-165">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="9ec7a-166">例 1: 希望するヘッダーのない要求</span><span class="sxs-lookup"><span data-stu-id="9ec7a-166">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="9ec7a-167">要求</span><span class="sxs-lookup"><span data-stu-id="9ec7a-167">Request</span></span>

<span data-ttu-id="9ec7a-168">ヘッダーの`Prefer`ない要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-168">The following is an example of the request without the `Prefer` header.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9ec7a-169">プロトコル</span><span class="sxs-lookup"><span data-stu-id="9ec7a-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/alerts/{alert_id}
Content-type: application/json

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9ec7a-170">C#</span><span class="sxs-lookup"><span data-stu-id="9ec7a-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-alert-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9ec7a-171">Javascript</span><span class="sxs-lookup"><span data-stu-id="9ec7a-171">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-alert-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9ec7a-172">目的-C</span><span class="sxs-lookup"><span data-stu-id="9ec7a-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-alert-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9ec7a-173">Java</span><span class="sxs-lookup"><span data-stu-id="9ec7a-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-alert-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="9ec7a-174">応答</span><span class="sxs-lookup"><span data-stu-id="9ec7a-174">Response</span></span>

<span data-ttu-id="9ec7a-175">成功応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-175">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="9ec7a-176">例 2: 要求ヘッダーを使用した要求</span><span class="sxs-lookup"><span data-stu-id="9ec7a-176">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="9ec7a-177">要求</span><span class="sxs-lookup"><span data-stu-id="9ec7a-177">Request</span></span>

<span data-ttu-id="9ec7a-178">次の例は、 `Prefer`要求ヘッダーを含む要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-178">The following example shows a request that includes the `Prefer` request header.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/alerts/{alert_id}
Content-type: application/json
Prefer: return=representation

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```

#### <a name="response"></a><span data-ttu-id="9ec7a-179">応答</span><span class="sxs-lookup"><span data-stu-id="9ec7a-179">Response</span></span>

<span data-ttu-id="9ec7a-180">オプション`Prefer: return=representation`の要求ヘッダーを使用する場合の応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-180">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="9ec7a-p109">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9ec7a-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update alert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
