# <a name="update-organization"></a><span data-ttu-id="82dbd-101">組織を更新する</span><span class="sxs-lookup"><span data-stu-id="82dbd-101">Update organization</span></span>

<span data-ttu-id="82dbd-102">現在認証されている組織のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="82dbd-102">Update the properties of the currently authenticated organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="82dbd-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="82dbd-103">Permissions</span></span>

<span data-ttu-id="82dbd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="82dbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="82dbd-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="82dbd-106">Permission type</span></span>      | <span data-ttu-id="82dbd-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="82dbd-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82dbd-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="82dbd-108">Delegated (work or school account)</span></span> | <span data-ttu-id="82dbd-109">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82dbd-109">Not supported.</span></span>    |
|<span data-ttu-id="82dbd-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="82dbd-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82dbd-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82dbd-111">Not supported.</span></span>    |
|<span data-ttu-id="82dbd-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="82dbd-112">Application</span></span> | <span data-ttu-id="82dbd-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82dbd-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="82dbd-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="82dbd-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization

```

## <a name="request-headers"></a><span data-ttu-id="82dbd-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="82dbd-115">Request headers</span></span>

| <span data-ttu-id="82dbd-116">名前</span><span class="sxs-lookup"><span data-stu-id="82dbd-116">Name</span></span>       | <span data-ttu-id="82dbd-117">型</span><span class="sxs-lookup"><span data-stu-id="82dbd-117">Type</span></span> | <span data-ttu-id="82dbd-118">説明</span><span class="sxs-lookup"><span data-stu-id="82dbd-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="82dbd-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="82dbd-119">Authorization</span></span>  | <span data-ttu-id="82dbd-120">string</span><span class="sxs-lookup"><span data-stu-id="82dbd-120">string</span></span>  | <span data-ttu-id="82dbd-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="82dbd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82dbd-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="82dbd-123">Request body</span></span>
<span data-ttu-id="82dbd-124">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="82dbd-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="82dbd-125">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="82dbd-125">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span> <span data-ttu-id="82dbd-126">最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="82dbd-126">For best performance, you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="82dbd-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82dbd-127">Property</span></span>     | <span data-ttu-id="82dbd-128">型</span><span class="sxs-lookup"><span data-stu-id="82dbd-128">Type</span></span>   |<span data-ttu-id="82dbd-129">説明</span><span class="sxs-lookup"><span data-stu-id="82dbd-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82dbd-130">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="82dbd-130">assignedPlans</span></span>|<span data-ttu-id="82dbd-131">AssignedPlan</span><span class="sxs-lookup"><span data-stu-id="82dbd-131">AssignedPlan</span></span>|<span data-ttu-id="82dbd-132">テナントに関連付けられているサービス プランのコレクション。</span><span class="sxs-lookup"><span data-stu-id="82dbd-132">The collection of service plans associated with the tenant. Not nullable.</span></span> <span data-ttu-id="82dbd-133">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="82dbd-133">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="82dbd-134">city</span><span class="sxs-lookup"><span data-stu-id="82dbd-134">city</span></span>|<span data-ttu-id="82dbd-135">String</span><span class="sxs-lookup"><span data-stu-id="82dbd-135">String</span></span>|            |
|<span data-ttu-id="82dbd-136">companyLastDirSyncTime</span><span class="sxs-lookup"><span data-stu-id="82dbd-136">companyLastDirSyncTime</span></span>|<span data-ttu-id="82dbd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82dbd-137">DateTimeOffset</span></span>|<span data-ttu-id="82dbd-138">前回テナントがオンプレミスのディレクトリと同期した日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="82dbd-138">The time and date at which the tenant was last synced with the on-premise directory.</span></span>|
|<span data-ttu-id="82dbd-139">country</span><span class="sxs-lookup"><span data-stu-id="82dbd-139">country</span></span>|<span data-ttu-id="82dbd-140">String</span><span class="sxs-lookup"><span data-stu-id="82dbd-140">String</span></span>|            |
|<span data-ttu-id="82dbd-141">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="82dbd-141">countryLetterCode</span></span>|<span data-ttu-id="82dbd-142">String</span><span class="sxs-lookup"><span data-stu-id="82dbd-142">String</span></span>|            |
|<span data-ttu-id="82dbd-143">deletionTimestamp</span><span class="sxs-lookup"><span data-stu-id="82dbd-143">deletionTimestamp</span></span>|<span data-ttu-id="82dbd-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82dbd-144">DateTimeOffset</span></span>||
|<span data-ttu-id="82dbd-145">dirSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="82dbd-145">dirSyncEnabled</span></span>|<span data-ttu-id="82dbd-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="82dbd-146">Boolean</span></span>|<span data-ttu-id="82dbd-147">このオブジェクトがオンプレミスのディレクトリから同期される場合は **true**。このオブジェクトが最初にオンプレミスのディレクトリから同期されていて、今後は同期されない場合は **false**。このオブジェクトがオンプレミスのディレクトリから一度も同期されたことがない場合は **null** (既定値)。</span><span class="sxs-lookup"><span data-stu-id="82dbd-147">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default).</span></span>|
|<span data-ttu-id="82dbd-148">displayName</span><span class="sxs-lookup"><span data-stu-id="82dbd-148">displayName</span></span>|<span data-ttu-id="82dbd-149">String</span><span class="sxs-lookup"><span data-stu-id="82dbd-149">String</span></span>|<span data-ttu-id="82dbd-150">テナントの表示名。</span><span class="sxs-lookup"><span data-stu-id="82dbd-150">The display name for the tenant.</span></span>|
|<span data-ttu-id="82dbd-151">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="82dbd-151">marketingNotificationEmails</span></span>|<span data-ttu-id="82dbd-152">String</span><span class="sxs-lookup"><span data-stu-id="82dbd-152">String</span></span>|                                        <span data-ttu-id="82dbd-153">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="82dbd-153">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="82dbd-154">objectType</span><span class="sxs-lookup"><span data-stu-id="82dbd-154">objectType</span></span>|<span data-ttu-id="82dbd-155">文字列</span><span class="sxs-lookup"><span data-stu-id="82dbd-155">String</span></span>|<span data-ttu-id="82dbd-156">オブジェクトの種類を識別する文字列です。</span><span class="sxs-lookup"><span data-stu-id="82dbd-156">A string that identifies the object type. For tenants the value is always “Company”.</span></span> <span data-ttu-id="82dbd-157">テナントの場合、値は常に “Company” です。</span><span class="sxs-lookup"><span data-stu-id="82dbd-157">A string that identifies the object type. For tenants the value is always “Company”.</span></span> <span data-ttu-id="82dbd-158">[directoryObject](../resources/directoryobject.md) から継承されます。</span><span class="sxs-lookup"><span data-stu-id="82dbd-158">Inherited from [directoryObject](../resources/directoryobject.md).</span></span>|
|<span data-ttu-id="82dbd-159">postalCode</span><span class="sxs-lookup"><span data-stu-id="82dbd-159">postalCode</span></span>|<span data-ttu-id="82dbd-160">String</span><span class="sxs-lookup"><span data-stu-id="82dbd-160">String</span></span>|            |
|<span data-ttu-id="82dbd-161">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="82dbd-161">preferredLanguage</span></span>|<span data-ttu-id="82dbd-162">String</span><span class="sxs-lookup"><span data-stu-id="82dbd-162">String</span></span>|            |
|<span data-ttu-id="82dbd-163">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="82dbd-163">provisionedPlans</span></span>|<span data-ttu-id="82dbd-164">ProvisionedPlan</span><span class="sxs-lookup"><span data-stu-id="82dbd-164">ProvisionedPlan</span></span>|                                        <span data-ttu-id="82dbd-165">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="82dbd-165">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="82dbd-166">provisioningErrors</span><span class="sxs-lookup"><span data-stu-id="82dbd-166">provisioningErrors</span></span>|<span data-ttu-id="82dbd-167">ProvisioningError</span><span class="sxs-lookup"><span data-stu-id="82dbd-167">ProvisioningError</span></span>|                                        <span data-ttu-id="82dbd-168">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="82dbd-168">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="82dbd-169">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="82dbd-169">securityComplianceNotificationMails</span></span>|<span data-ttu-id="82dbd-170">String</span><span class="sxs-lookup"><span data-stu-id="82dbd-170">String</span></span>||
|<span data-ttu-id="82dbd-171">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="82dbd-171">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="82dbd-172">String</span><span class="sxs-lookup"><span data-stu-id="82dbd-172">String</span></span>||
|<span data-ttu-id="82dbd-173">state</span><span class="sxs-lookup"><span data-stu-id="82dbd-173">state</span></span>|<span data-ttu-id="82dbd-174">String</span><span class="sxs-lookup"><span data-stu-id="82dbd-174">String</span></span>|            |
|<span data-ttu-id="82dbd-175">street</span><span class="sxs-lookup"><span data-stu-id="82dbd-175">street</span></span>|<span data-ttu-id="82dbd-176">String</span><span class="sxs-lookup"><span data-stu-id="82dbd-176">String</span></span>|            |
|<span data-ttu-id="82dbd-177">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="82dbd-177">technicalNotificationMails</span></span>|<span data-ttu-id="82dbd-178">String</span><span class="sxs-lookup"><span data-stu-id="82dbd-178">String</span></span>|                                        <span data-ttu-id="82dbd-179">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="82dbd-179">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="82dbd-180">telephoneNumber</span><span class="sxs-lookup"><span data-stu-id="82dbd-180">telephoneNumber</span></span>|<span data-ttu-id="82dbd-181">String</span><span class="sxs-lookup"><span data-stu-id="82dbd-181">String</span></span>|            |
|<span data-ttu-id="82dbd-182">verifiedDomains</span><span class="sxs-lookup"><span data-stu-id="82dbd-182">verifiedDomains</span></span>|<span data-ttu-id="82dbd-183">VerifiedDomain</span><span class="sxs-lookup"><span data-stu-id="82dbd-183">VerifiedDomain</span></span>|<span data-ttu-id="82dbd-184">このテナントに関連付けられているドメインのコレクション。</span><span class="sxs-lookup"><span data-stu-id="82dbd-184">The collection of domains associated with this tenant. Not nullable.</span></span> <span data-ttu-id="82dbd-185">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="82dbd-185">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="82dbd-186">応答</span><span class="sxs-lookup"><span data-stu-id="82dbd-186">Response</span></span>

<span data-ttu-id="82dbd-187">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [organization](../resources/organization.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="82dbd-187">If successful, this method returns a `200 OK` response code and updated [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82dbd-188">例</span><span class="sxs-lookup"><span data-stu-id="82dbd-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="82dbd-189">要求</span><span class="sxs-lookup"><span data-stu-id="82dbd-189">Request</span></span>

<span data-ttu-id="82dbd-190">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="82dbd-190">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization
Content-type: application/json
Content-length: 411

{
  "assignedPlans": [
    {
      "assignedDateTime": "datetime-value",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "servicePlanId-value"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "country": "country-value",
  "countryLetterCode": "countryLetterCode-value",
  "displayName": "displayName-value"
}
```

<br/>

### <a name="response"></a><span data-ttu-id="82dbd-191">応答</span><span class="sxs-lookup"><span data-stu-id="82dbd-191">Response</span></span>

<span data-ttu-id="82dbd-192">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="82dbd-192">Here is an example of the response.</span></span> <span data-ttu-id="82dbd-193">**注**:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="82dbd-193">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="82dbd-194">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="82dbd-194">All default properties will be returned from the actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 411

{
  "assignedPlans": [
    {
      "assignedDateTime": "datetime-value",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "servicePlanId-value"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "country": "country-value",
  "countryLetterCode": "countryLetterCode-value",
  "displayName": "displayName-value"
}
```

<br/>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
