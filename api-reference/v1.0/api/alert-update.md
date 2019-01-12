---
title: 警告の更新
description: アラートの状態および割り当ての同期を保つソリューション全体に統合されたソリューション内で、編集可能な**アラート**のプロパティを更新します。 このメソッドは、id。 参照されているアラートのレコードがどのようなソリューションを更新します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 7b218daa56f7648bc888bbc0cd25619b22799325
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966035"
---
# <a name="update-alert"></a><span data-ttu-id="4450a-104">警告の更新</span><span class="sxs-lookup"><span data-stu-id="4450a-104">Update alert</span></span>

<span data-ttu-id="4450a-105">アラートの状態および割り当ての同期を保つソリューション全体に統合されたソリューション内で、編集可能な**アラート**のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4450a-105">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="4450a-106">このメソッドは、id。 参照されているアラートのレコードがどのようなソリューションを更新します。</span><span class="sxs-lookup"><span data-stu-id="4450a-106">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="4450a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4450a-107">Permissions</span></span>

<span data-ttu-id="4450a-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4450a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4450a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4450a-110">Permission type</span></span>      | <span data-ttu-id="4450a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4450a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4450a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4450a-112">Delegated (work or school account)</span></span> |   <span data-ttu-id="4450a-113">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4450a-113">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="4450a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4450a-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4450a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4450a-115">Not supported.</span></span>  |
|<span data-ttu-id="4450a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4450a-116">Application</span></span> | <span data-ttu-id="4450a-117">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4450a-117">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4450a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4450a-118">HTTP request</span></span>

> <span data-ttu-id="4450a-119">**注:** パラメーターおよび vendorInformation が含まれていると**警告**の ID を含める必要があります、`provider`と`vendor`このメソッドを使用します。</span><span class="sxs-lookup"><span data-stu-id="4450a-119">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="4450a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4450a-120">Request headers</span></span>

| <span data-ttu-id="4450a-121">名前</span><span class="sxs-lookup"><span data-stu-id="4450a-121">Name</span></span>       | <span data-ttu-id="4450a-122">説明</span><span class="sxs-lookup"><span data-stu-id="4450a-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4450a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4450a-123">Authorization</span></span>  | <span data-ttu-id="4450a-p104">Bearer {code}。必須。</span><span class="sxs-lookup"><span data-stu-id="4450a-p104">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="4450a-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="4450a-126">Prefer</span></span> | <span data-ttu-id="4450a-127">返す = 表現</span><span class="sxs-lookup"><span data-stu-id="4450a-127">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="4450a-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="4450a-128">Request body</span></span>

<span data-ttu-id="4450a-129">要求の本文には、更新される関連フィールドの値の JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="4450a-129">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4450a-130">含まれている**必要があります**本体、`vendorInformation`プロパティに有効な`provider`と`vendor`のフィールドです。</span><span class="sxs-lookup"><span data-stu-id="4450a-130">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="4450a-131">次の表では、アラートの更新可能なフィールドを示します。</span><span class="sxs-lookup"><span data-stu-id="4450a-131">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="4450a-132">要求の本文に含まれていない既存のプロパティの値は変更されません。</span><span class="sxs-lookup"><span data-stu-id="4450a-132">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="4450a-133">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="4450a-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4450a-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4450a-134">Property</span></span>   | <span data-ttu-id="4450a-135">種類</span><span class="sxs-lookup"><span data-stu-id="4450a-135">Type</span></span> |<span data-ttu-id="4450a-136">説明</span><span class="sxs-lookup"><span data-stu-id="4450a-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4450a-137">担当者</span><span class="sxs-lookup"><span data-stu-id="4450a-137">assignedTo</span></span>|<span data-ttu-id="4450a-138">String</span><span class="sxs-lookup"><span data-stu-id="4450a-138">String</span></span>|<span data-ttu-id="4450a-139">アナリスト、警告の名前は、選別、調査、または修復用に割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="4450a-139">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="4450a-140">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="4450a-140">closedDateTime</span></span>|<span data-ttu-id="4450a-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4450a-141">DateTimeOffset</span></span>|<span data-ttu-id="4450a-142">時間のアラートが閉じられました。</span><span class="sxs-lookup"><span data-stu-id="4450a-142">Time at which the alert was closed.</span></span> <span data-ttu-id="4450a-143">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="4450a-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4450a-144">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4450a-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="4450a-145">comments</span><span class="sxs-lookup"><span data-stu-id="4450a-145">comments</span></span>|<span data-ttu-id="4450a-146">String コレクション</span><span class="sxs-lookup"><span data-stu-id="4450a-146">String collection</span></span>|<span data-ttu-id="4450a-147">(顧客の警告管理) の警告のアナリストのコメントです。</span><span class="sxs-lookup"><span data-stu-id="4450a-147">Analyst comments on the alert (for customer alert management).</span></span>|
|<span data-ttu-id="4450a-148">feedback</span><span class="sxs-lookup"><span data-stu-id="4450a-148">feedback</span></span>|<span data-ttu-id="4450a-149">alertFeedback</span><span class="sxs-lookup"><span data-stu-id="4450a-149">alertFeedback</span></span>|<span data-ttu-id="4450a-150">アナリストのフィードバック通知をします。</span><span class="sxs-lookup"><span data-stu-id="4450a-150">Analyst feedback on the alert.</span></span> <span data-ttu-id="4450a-151">可能な値は、`unknown`、`truePositive`、`falsePositive`、`benignPositive` です。</span><span class="sxs-lookup"><span data-stu-id="4450a-151">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="4450a-152">status</span><span class="sxs-lookup"><span data-stu-id="4450a-152">status</span></span>|<span data-ttu-id="4450a-153">alertStatus</span><span class="sxs-lookup"><span data-stu-id="4450a-153">alertStatus</span></span>|<span data-ttu-id="4450a-154">アラートのライフ サイクルのステータス (ステージ)。</span><span class="sxs-lookup"><span data-stu-id="4450a-154">Alert lifecycle status (stage).</span></span> <span data-ttu-id="4450a-155">可能な値は、`unknown`、`newAlert`、`inProgress`、`resolved` です。</span><span class="sxs-lookup"><span data-stu-id="4450a-155">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="4450a-156">タグの前に追加されるマークアップ</span><span class="sxs-lookup"><span data-stu-id="4450a-156">tags</span></span>|<span data-ttu-id="4450a-157">String コレクション</span><span class="sxs-lookup"><span data-stu-id="4450a-157">String collection</span></span>|<span data-ttu-id="4450a-158">アラートに適用することができますし、フィルターの条件 (たとえば、"HVA"、"されていた) として使用できるユーザー定義のラベル。</span><span class="sxs-lookup"><span data-stu-id="4450a-158">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="4450a-159">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="4450a-159">vendorInformation</span></span> |[<span data-ttu-id="4450a-160">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="4450a-160">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="4450a-161">セキュリティ製品やサービスの仕入先、プロバイダー、および subprovider の詳細を含む複合型 (仕入先など = Microsoft; プロバイダー = Windows Defender の ATP は subProvider AppLocker を =)。</span><span class="sxs-lookup"><span data-stu-id="4450a-161">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="4450a-162">**プロバイダーおよび仕入先のフィールドは、必要があります。**</span><span class="sxs-lookup"><span data-stu-id="4450a-162">**Provider and vendor fields are required.**</span></span>|

## <a name="response"></a><span data-ttu-id="4450a-163">応答</span><span class="sxs-lookup"><span data-stu-id="4450a-163">Response</span></span>

<span data-ttu-id="4450a-164">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="4450a-164">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="4450a-165">省略可能な要求ヘッダーが使用され、メソッドが返されます、`200 OK`応答コードおよび応答の本体で更新された[アラート](../resources/alert.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="4450a-165">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="4450a-166">例 1</span><span class="sxs-lookup"><span data-stu-id="4450a-166">Example 1</span></span>

### <a name="request"></a><span data-ttu-id="4450a-167">要求</span><span class="sxs-lookup"><span data-stu-id="4450a-167">Request</span></span>

<span data-ttu-id="4450a-168">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4450a-168">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4450a-169">応答</span><span class="sxs-lookup"><span data-stu-id="4450a-169">Response</span></span>

<span data-ttu-id="4450a-170">次は、正常な応答の例です。</span><span class="sxs-lookup"><span data-stu-id="4450a-170">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="example-2"></a><span data-ttu-id="4450a-171">例 2</span><span class="sxs-lookup"><span data-stu-id="4450a-171">Example 2</span></span>

### <a name="request"></a><span data-ttu-id="4450a-172">要求</span><span class="sxs-lookup"><span data-stu-id="4450a-172">Request</span></span>

<span data-ttu-id="4450a-173">次の例では、要求を含む、`Prefer`要求ヘッダー。</span><span class="sxs-lookup"><span data-stu-id="4450a-173">The following example shows a request that includes the `Prefer` request header.</span></span>

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

### <a name="response"></a><span data-ttu-id="4450a-174">応答</span><span class="sxs-lookup"><span data-stu-id="4450a-174">Response</span></span>

<span data-ttu-id="4450a-175">次の応答の例ではときに、省略可能な`Prefer: return=representation`要求ヘッダーを使用します。</span><span class="sxs-lookup"><span data-stu-id="4450a-175">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="4450a-p110">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4450a-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
