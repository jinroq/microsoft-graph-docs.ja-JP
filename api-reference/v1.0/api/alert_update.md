# <a name="update-alert"></a><span data-ttu-id="00b6f-101">警告の更新</span><span class="sxs-lookup"><span data-stu-id="00b6f-101">Update alert</span></span>

<span data-ttu-id="00b6f-102">統合ソリューション内の編集可能な**警告**プロパティを更新して、 ソリューション間で警告の状態と割り当ての同期を維持します。</span><span class="sxs-lookup"><span data-stu-id="00b6f-102">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="00b6f-103">このメソッドは、参照されている警告 ID のレコードのあるすべてのソリューションを更新します。</span><span class="sxs-lookup"><span data-stu-id="00b6f-103">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="00b6f-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="00b6f-104">Permissions</span></span>

<span data-ttu-id="00b6f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="00b6f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="00b6f-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="00b6f-107">Permission type</span></span>      | <span data-ttu-id="00b6f-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="00b6f-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00b6f-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="00b6f-109">Delegated (work or school account)</span></span> |   <span data-ttu-id="00b6f-110">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00b6f-110">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="00b6f-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="00b6f-111">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="00b6f-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00b6f-112">Not supported.</span></span>  |
|<span data-ttu-id="00b6f-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="00b6f-113">Application</span></span> | <span data-ttu-id="00b6f-114">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00b6f-114">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="00b6f-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="00b6f-115">HTTP request</span></span>

> <span data-ttu-id="00b6f-116">**注:** このメソッドでは、`provider` と `vendor` を含むパラメーターと vendorInformation として、**警告** ID を含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="00b6f-116">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="00b6f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="00b6f-117">Request headers</span></span>

| <span data-ttu-id="00b6f-118">名前</span><span class="sxs-lookup"><span data-stu-id="00b6f-118">Name</span></span>       | <span data-ttu-id="00b6f-119">説明</span><span class="sxs-lookup"><span data-stu-id="00b6f-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="00b6f-120">承認</span><span class="sxs-lookup"><span data-stu-id="00b6f-120">Authorization</span></span>  | <span data-ttu-id="00b6f-p103">Bearer {code}。必須。</span><span class="sxs-lookup"><span data-stu-id="00b6f-p103">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="00b6f-123">優先</span><span class="sxs-lookup"><span data-stu-id="00b6f-123">Prefer</span></span> | <span data-ttu-id="00b6f-124">返す = 表現</span><span class="sxs-lookup"><span data-stu-id="00b6f-124">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="00b6f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="00b6f-125">Request body</span></span>

<span data-ttu-id="00b6f-126">要求本文で、更新する関連フィールドの値の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="00b6f-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="00b6f-127">本文には、有効な`provider` と `vendor`フィールドのある `vendorInformation` プロパティが含まれて**いなければなりません**。</span><span class="sxs-lookup"><span data-stu-id="00b6f-127">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="00b6f-128">次の表では、警告の更新可能なフィールドを示します。</span><span class="sxs-lookup"><span data-stu-id="00b6f-128">The following table lists the authentication settings that can be changed for an authentication provider.</span></span> <span data-ttu-id="00b6f-129">要求の本文に含まれない既存のプロパティの値は変更されません。</span><span class="sxs-lookup"><span data-stu-id="00b6f-129">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="00b6f-130">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="00b6f-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="00b6f-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="00b6f-131">Property</span></span>   | <span data-ttu-id="00b6f-132">型</span><span class="sxs-lookup"><span data-stu-id="00b6f-132">Type</span></span> |<span data-ttu-id="00b6f-133">説明</span><span class="sxs-lookup"><span data-stu-id="00b6f-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00b6f-134">assignedTo</span><span class="sxs-lookup"><span data-stu-id="00b6f-134">AssignedTo</span></span>|<span data-ttu-id="00b6f-135">文字列</span><span class="sxs-lookup"><span data-stu-id="00b6f-135">String</span></span>|<span data-ttu-id="00b6f-136">警告は、アナリストの名前を選別、調査、または修復に割り当てます。</span><span class="sxs-lookup"><span data-stu-id="00b6f-136">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="00b6f-137">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="00b6f-137">closedDateTime</span></span>|<span data-ttu-id="00b6f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00b6f-138">DateTimeOffset</span></span>|<span data-ttu-id="00b6f-139">警告が終了した時間。</span><span class="sxs-lookup"><span data-stu-id="00b6f-139">Time at which the alert was closed.</span></span> <span data-ttu-id="00b6f-140">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="00b6f-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="00b6f-141">|||UNTRANSLATED_CONTENT_START|||For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.|||UNTRANSLATED_CONTENT_END|||</span><span class="sxs-lookup"><span data-stu-id="00b6f-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="00b6f-142">コメント</span><span class="sxs-lookup"><span data-stu-id="00b6f-142">comments</span></span>|<span data-ttu-id="00b6f-143">String コレクション</span><span class="sxs-lookup"><span data-stu-id="00b6f-143">String collection</span></span>|<span data-ttu-id="00b6f-144">警告 (顧客の警告管理用) に関するアナリストのコメントです。</span><span class="sxs-lookup"><span data-stu-id="00b6f-144">Analyst comments on the alert (for customer alert management).</span></span>|
|<span data-ttu-id="00b6f-145">フィードバック</span><span class="sxs-lookup"><span data-stu-id="00b6f-145">feedback</span></span>|<span data-ttu-id="00b6f-146">alertFeedback</span><span class="sxs-lookup"><span data-stu-id="00b6f-146">alertFeedback</span></span>|<span data-ttu-id="00b6f-147">警告に関するアナリストのフィードバックです。</span><span class="sxs-lookup"><span data-stu-id="00b6f-147">Analyst feedback on the alert.</span></span> <span data-ttu-id="00b6f-148">可能な値は、`unknown`、`truePositive`、`falsePositive`、`benignPositive` です。</span><span class="sxs-lookup"><span data-stu-id="00b6f-148">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="00b6f-149">状態</span><span class="sxs-lookup"><span data-stu-id="00b6f-149">status</span></span>|<span data-ttu-id="00b6f-150">alertStatus</span><span class="sxs-lookup"><span data-stu-id="00b6f-150">alertStatus</span></span>|<span data-ttu-id="00b6f-151">アラートのライフ サイクル ステータス (ステージ)。</span><span class="sxs-lookup"><span data-stu-id="00b6f-151">Alert lifecycle status (stage).</span></span> <span data-ttu-id="00b6f-152">可能な値は、`unknown`、`newAlert`、`inProgress`、`resolved` です。</span><span class="sxs-lookup"><span data-stu-id="00b6f-152">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="00b6f-153">タグ</span><span class="sxs-lookup"><span data-stu-id="00b6f-153">tags</span></span>|<span data-ttu-id="00b6f-154">String コレクション</span><span class="sxs-lookup"><span data-stu-id="00b6f-154">String collection</span></span>|<span data-ttu-id="00b6f-155">警告に適用でき、フィルター条件 ("HVA"、"SAW" など) として機能できるユーザーが定義可能なラベル。</span><span class="sxs-lookup"><span data-stu-id="00b6f-155">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="00b6f-156">vendorInformation \*</span><span class="sxs-lookup"><span data-stu-id="00b6f-156">vendorInformation \*</span></span>|[<span data-ttu-id="00b6f-157">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="00b6f-157">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="00b6f-158">セキュリティ製品、またはサービスの仕入先、サービス プロバイダー、およびサービス サブプロバイダーの詳細を含む複合型 (仕入先 = Microsoft、プロバイダー = Windows Defender ATP、サブプロバイダー = AppLocker など)。</span><span class="sxs-lookup"><span data-stu-id="00b6f-158">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="00b6f-159">**プロバイダーおよび仕入先のフィールドは必須です。**</span><span class="sxs-lookup"><span data-stu-id="00b6f-159">**Provider and vendor fields are required.**</span></span>|
<span data-ttu-id="00b6f-160">(\* は、必須フィールドを表します)。</span><span class="sxs-lookup"><span data-stu-id="00b6f-160">(\* Indicates a mandatory field.)</span></span>

## <a name="response"></a><span data-ttu-id="00b6f-161">応答</span><span class="sxs-lookup"><span data-stu-id="00b6f-161">Response</span></span>

<span data-ttu-id="00b6f-162">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="00b6f-162">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="00b6f-163">オプションの要求ヘッダーが使われている場合、このメソッドは`200 OK`応答コードと、応答本文で[警告](../resources/alert.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="00b6f-163">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="00b6f-164">例 1</span><span class="sxs-lookup"><span data-stu-id="00b6f-164">Example 1</span></span>

### <a name="request"></a><span data-ttu-id="00b6f-165">要求</span><span class="sxs-lookup"><span data-stu-id="00b6f-165">Request</span></span>

<span data-ttu-id="00b6f-166">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="00b6f-166">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="00b6f-167">応答</span><span class="sxs-lookup"><span data-stu-id="00b6f-167">Response</span></span>

<span data-ttu-id="00b6f-168">正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="00b6f-168">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="example-2"></a><span data-ttu-id="00b6f-169">例 2</span><span class="sxs-lookup"><span data-stu-id="00b6f-169">Example 2</span></span>

### <a name="request"></a><span data-ttu-id="00b6f-170">要求</span><span class="sxs-lookup"><span data-stu-id="00b6f-170">Request</span></span>

<span data-ttu-id="00b6f-171">次の例では、`Prefer` 要求ヘッダーを含む要求を示します。</span><span class="sxs-lookup"><span data-stu-id="00b6f-171">The following example shows a request that includes the `Prefer` request header.</span></span>

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

### <a name="response"></a><span data-ttu-id="00b6f-172">応答</span><span class="sxs-lookup"><span data-stu-id="00b6f-172">Response</span></span>

<span data-ttu-id="00b6f-173">|||UNTRANSLATED_CONTENT_START|||The following is an example of the response when the optional `Prefer: return=representation` request header is used.|||UNTRANSLATED_CONTENT_END|||</span><span class="sxs-lookup"><span data-stu-id="00b6f-173">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="00b6f-p109">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="00b6f-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
