# <a name="update-alert"></a><span data-ttu-id="11990-101">警告の更新</span><span class="sxs-lookup"><span data-stu-id="11990-101">Update alert</span></span>

<span data-ttu-id="11990-102">アラートの状態および割り当ての同期を保つソリューション全体に統合されたソリューション内で、編集可能な**アラート**のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="11990-102">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="11990-103">このメソッドは、id。 参照されているアラートのレコードがどのようなソリューションを更新します。</span><span class="sxs-lookup"><span data-stu-id="11990-103">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="11990-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="11990-104">Permissions</span></span>

<span data-ttu-id="11990-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="11990-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="11990-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="11990-107">Permission type</span></span>      | <span data-ttu-id="11990-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="11990-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11990-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="11990-109">Delegated (work or school account)</span></span> |   <span data-ttu-id="11990-110">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11990-110">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="11990-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="11990-111">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="11990-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11990-112">Not supported.</span></span>  |
|<span data-ttu-id="11990-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="11990-113">Application</span></span> | <span data-ttu-id="11990-114">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11990-114">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="11990-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="11990-115">HTTP request</span></span>

> <span data-ttu-id="11990-116">**注:** パラメーターおよび vendorInformation が含まれていると**警告**の ID を含める必要があります、`provider`と`vendor`このメソッドを使用します。</span><span class="sxs-lookup"><span data-stu-id="11990-116">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="11990-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="11990-117">Request headers</span></span>

| <span data-ttu-id="11990-118">名前</span><span class="sxs-lookup"><span data-stu-id="11990-118">Name</span></span>       | <span data-ttu-id="11990-119">説明</span><span class="sxs-lookup"><span data-stu-id="11990-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="11990-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="11990-120">Authorization</span></span>  | <span data-ttu-id="11990-p103">Bearer {code}。必須。</span><span class="sxs-lookup"><span data-stu-id="11990-p103">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="11990-123">Prefer</span><span class="sxs-lookup"><span data-stu-id="11990-123">Prefer</span></span> | <span data-ttu-id="11990-124">返す = 表現</span><span class="sxs-lookup"><span data-stu-id="11990-124">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="11990-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="11990-125">Request body</span></span>

<span data-ttu-id="11990-126">要求の本文には、更新される関連フィールドの値の JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="11990-126">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="11990-127">含まれている**必要があります**本体、`vendorInformation`プロパティに有効な`provider`と`vendor`のフィールドです。</span><span class="sxs-lookup"><span data-stu-id="11990-127">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="11990-128">次の表では、アラートの更新可能なフィールドを示します。</span><span class="sxs-lookup"><span data-stu-id="11990-128">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="11990-129">要求の本文に含まれていない既存のプロパティの値は変更されません。</span><span class="sxs-lookup"><span data-stu-id="11990-129">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="11990-130">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="11990-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="11990-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="11990-131">Property</span></span>   | <span data-ttu-id="11990-132">型</span><span class="sxs-lookup"><span data-stu-id="11990-132">Type</span></span> |<span data-ttu-id="11990-133">説明</span><span class="sxs-lookup"><span data-stu-id="11990-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11990-134">担当者</span><span class="sxs-lookup"><span data-stu-id="11990-134">assignedTo</span></span>|<span data-ttu-id="11990-135">文字列</span><span class="sxs-lookup"><span data-stu-id="11990-135">String</span></span>|<span data-ttu-id="11990-136">アナリスト、警告の名前は、選別、調査、または修復用に割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="11990-136">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="11990-137">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="11990-137">closedDateTime</span></span>|<span data-ttu-id="11990-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11990-138">DateTimeOffset</span></span>|<span data-ttu-id="11990-139">時間のアラートが閉じられました。</span><span class="sxs-lookup"><span data-stu-id="11990-139">Time at which the alert was closed.</span></span> <span data-ttu-id="11990-140">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="11990-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="11990-141">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="11990-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="11990-142">comments</span><span class="sxs-lookup"><span data-stu-id="11990-142">comments</span></span>|<span data-ttu-id="11990-143">String コレクション</span><span class="sxs-lookup"><span data-stu-id="11990-143">String collection</span></span>|<span data-ttu-id="11990-144">(顧客の警告管理) の警告のアナリストのコメントです。</span><span class="sxs-lookup"><span data-stu-id="11990-144">Analyst comments on the alert (for customer alert management).</span></span>|
|<span data-ttu-id="11990-145">feedback</span><span class="sxs-lookup"><span data-stu-id="11990-145">feedback</span></span>|<span data-ttu-id="11990-146">alertFeedback</span><span class="sxs-lookup"><span data-stu-id="11990-146">alertFeedback</span></span>|<span data-ttu-id="11990-147">アナリストのフィードバック通知をします。</span><span class="sxs-lookup"><span data-stu-id="11990-147">Analyst feedback on the alert.</span></span> <span data-ttu-id="11990-148">可能な値は、`unknown`、`truePositive`、`falsePositive`、`benignPositive` です。</span><span class="sxs-lookup"><span data-stu-id="11990-148">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="11990-149">status</span><span class="sxs-lookup"><span data-stu-id="11990-149">status</span></span>|<span data-ttu-id="11990-150">alertStatus</span><span class="sxs-lookup"><span data-stu-id="11990-150">alertStatus</span></span>|<span data-ttu-id="11990-151">アラートのライフ サイクルのステータス (ステージ)。</span><span class="sxs-lookup"><span data-stu-id="11990-151">Alert lifecycle status (stage).</span></span> <span data-ttu-id="11990-152">可能な値は、`unknown`、`newAlert`、`inProgress`、`resolved` です。</span><span class="sxs-lookup"><span data-stu-id="11990-152">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="11990-153">タグの前に追加されるマークアップ</span><span class="sxs-lookup"><span data-stu-id="11990-153">tags</span></span>|<span data-ttu-id="11990-154">String コレクション</span><span class="sxs-lookup"><span data-stu-id="11990-154">String collection</span></span>|<span data-ttu-id="11990-155">アラートに適用することができますし、フィルターの条件 (たとえば、"HVA"、"されていた) として使用できるユーザー定義のラベル。</span><span class="sxs-lookup"><span data-stu-id="11990-155">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="11990-156">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="11990-156">vendorInformation</span></span> |[<span data-ttu-id="11990-157">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="11990-157">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="11990-158">セキュリティ製品やサービスの仕入先、プロバイダー、および subprovider の詳細を含む複合型 (仕入先など = Microsoft; プロバイダー = Windows Defender の ATP は subProvider AppLocker を =)。</span><span class="sxs-lookup"><span data-stu-id="11990-158">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="11990-159">**プロバイダーおよび仕入先のフィールドは、必要があります。**</span><span class="sxs-lookup"><span data-stu-id="11990-159">**Provider and vendor fields are required.**</span></span>|

## <a name="response"></a><span data-ttu-id="11990-160">応答</span><span class="sxs-lookup"><span data-stu-id="11990-160">Response</span></span>

<span data-ttu-id="11990-161">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="11990-161">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="11990-162">省略可能な要求ヘッダーが使用され、メソッドが返されます、`200 OK`応答コードおよび応答の本体で更新された[アラート](../resources/alert.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="11990-162">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="11990-163">例 1</span><span class="sxs-lookup"><span data-stu-id="11990-163">Example 1</span></span>

### <a name="request"></a><span data-ttu-id="11990-164">要求</span><span class="sxs-lookup"><span data-stu-id="11990-164">Request</span></span>

<span data-ttu-id="11990-165">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="11990-165">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="11990-166">応答</span><span class="sxs-lookup"><span data-stu-id="11990-166">Response</span></span>

<span data-ttu-id="11990-167">次は、正常な応答の例です。</span><span class="sxs-lookup"><span data-stu-id="11990-167">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="example-2"></a><span data-ttu-id="11990-168">例 2</span><span class="sxs-lookup"><span data-stu-id="11990-168">Example 2</span></span>

### <a name="request"></a><span data-ttu-id="11990-169">要求</span><span class="sxs-lookup"><span data-stu-id="11990-169">Request</span></span>

<span data-ttu-id="11990-170">次の例では、要求を含む、`Prefer`要求ヘッダー。</span><span class="sxs-lookup"><span data-stu-id="11990-170">The following example shows a request that includes the `Prefer` request header.</span></span>

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

### <a name="response"></a><span data-ttu-id="11990-171">応答</span><span class="sxs-lookup"><span data-stu-id="11990-171">Response</span></span>

<span data-ttu-id="11990-172">次の応答の例ではときに、省略可能な`Prefer: return=representation`要求ヘッダーを使用します。</span><span class="sxs-lookup"><span data-stu-id="11990-172">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="11990-p109">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="11990-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
