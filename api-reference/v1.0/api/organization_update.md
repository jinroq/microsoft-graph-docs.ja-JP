# <a name="update-organization"></a><span data-ttu-id="1c0f7-101">組織を更新する</span><span class="sxs-lookup"><span data-stu-id="1c0f7-101">Update organization</span></span>

<span data-ttu-id="1c0f7-102">現在認証されている組織のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1c0f7-102">Update the properties of the currently authenticated organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="1c0f7-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1c0f7-103">Permissions</span></span>
<span data-ttu-id="1c0f7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1c0f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1c0f7-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1c0f7-106">Permission type</span></span>      | <span data-ttu-id="1c0f7-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1c0f7-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c0f7-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1c0f7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1c0f7-109">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c0f7-109">Not supported.</span></span>    |
|<span data-ttu-id="1c0f7-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1c0f7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c0f7-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c0f7-111">Not supported.</span></span>    |
|<span data-ttu-id="1c0f7-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1c0f7-112">Application</span></span> | <span data-ttu-id="1c0f7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c0f7-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c0f7-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1c0f7-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /organization

```
## <a name="request-headers"></a><span data-ttu-id="1c0f7-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1c0f7-115">Request headers</span></span>
| <span data-ttu-id="1c0f7-116">名前</span><span class="sxs-lookup"><span data-stu-id="1c0f7-116">Name</span></span>       | <span data-ttu-id="1c0f7-117">型</span><span class="sxs-lookup"><span data-stu-id="1c0f7-117">Type</span></span> | <span data-ttu-id="1c0f7-118">説明</span><span class="sxs-lookup"><span data-stu-id="1c0f7-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1c0f7-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c0f7-119">Authorization</span></span>  | <span data-ttu-id="1c0f7-120">string</span><span class="sxs-lookup"><span data-stu-id="1c0f7-120">string</span></span>  | <span data-ttu-id="1c0f7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1c0f7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c0f7-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="1c0f7-123">Request body</span></span>
<span data-ttu-id="1c0f7-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="1c0f7-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1c0f7-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1c0f7-127">Property</span></span>     | <span data-ttu-id="1c0f7-128">型</span><span class="sxs-lookup"><span data-stu-id="1c0f7-128">Type</span></span>   |<span data-ttu-id="1c0f7-129">説明</span><span class="sxs-lookup"><span data-stu-id="1c0f7-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1c0f7-130">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="1c0f7-130">assignedPlans</span></span>|<span data-ttu-id="1c0f7-131">AssignedPlan</span><span class="sxs-lookup"><span data-stu-id="1c0f7-131">AssignedPlan</span></span>|<span data-ttu-id="1c0f7-p104">テナントに関連付けられているサービス プランのコレクション。                          **注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="1c0f7-p104">The collection of service plans associated with the tenant.                            **Notes**: not nullable.</span></span>            |
|<span data-ttu-id="1c0f7-134">city</span><span class="sxs-lookup"><span data-stu-id="1c0f7-134">city</span></span>|<span data-ttu-id="1c0f7-135">String</span><span class="sxs-lookup"><span data-stu-id="1c0f7-135">String</span></span>|            |
|<span data-ttu-id="1c0f7-136">companyLastDirSyncTime</span><span class="sxs-lookup"><span data-stu-id="1c0f7-136">companyLastDirSyncTime</span></span>|<span data-ttu-id="1c0f7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c0f7-137">DateTimeOffset</span></span>|<span data-ttu-id="1c0f7-138">前回テナントがオンプレミスのディレクトリと同期した日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="1c0f7-138">The time and date at which the tenant was last synced with the on-premise directory.</span></span>|
|<span data-ttu-id="1c0f7-139">country</span><span class="sxs-lookup"><span data-stu-id="1c0f7-139">country</span></span>|<span data-ttu-id="1c0f7-140">String</span><span class="sxs-lookup"><span data-stu-id="1c0f7-140">String</span></span>|            |
|<span data-ttu-id="1c0f7-141">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="1c0f7-141">countryLetterCode</span></span>|<span data-ttu-id="1c0f7-142">String</span><span class="sxs-lookup"><span data-stu-id="1c0f7-142">String</span></span>|            |
|<span data-ttu-id="1c0f7-143">deletionTimestamp</span><span class="sxs-lookup"><span data-stu-id="1c0f7-143">deletionTimestamp</span></span>|<span data-ttu-id="1c0f7-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c0f7-144">DateTimeOffset</span></span>||
|<span data-ttu-id="1c0f7-145">dirSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="1c0f7-145">dirSyncEnabled</span></span>|<span data-ttu-id="1c0f7-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c0f7-146">Boolean</span></span>|<span data-ttu-id="1c0f7-147">このオブジェクトがオンプレミスのディレクトリから同期される場合は **true**。このオブジェクトが最初にオンプレミスのディレクトリから同期されていて、今後は同期されない場合は **false**。このオブジェクトがオンプレミスのディレクトリから一度も同期されたことがない場合は **null** (既定値)。</span><span class="sxs-lookup"><span data-stu-id="1c0f7-147">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default).</span></span>|
|<span data-ttu-id="1c0f7-148">displayName</span><span class="sxs-lookup"><span data-stu-id="1c0f7-148">displayName</span></span>|<span data-ttu-id="1c0f7-149">String</span><span class="sxs-lookup"><span data-stu-id="1c0f7-149">String</span></span>|<span data-ttu-id="1c0f7-150">テナントの表示名。</span><span class="sxs-lookup"><span data-stu-id="1c0f7-150">The display name for the tenant.</span></span>|
|<span data-ttu-id="1c0f7-151">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="1c0f7-151">marketingNotificationEmails</span></span>|<span data-ttu-id="1c0f7-152">String</span><span class="sxs-lookup"><span data-stu-id="1c0f7-152">String</span></span>|                                        <span data-ttu-id="1c0f7-153">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="1c0f7-153">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="1c0f7-154">objectType</span><span class="sxs-lookup"><span data-stu-id="1c0f7-154">objectType</span></span>|<span data-ttu-id="1c0f7-155">String</span><span class="sxs-lookup"><span data-stu-id="1c0f7-155">String</span></span>|<span data-ttu-id="1c0f7-p105">オブジェクトの種類を識別する文字列です。テナントの場合、値は常に「Company」です。[directoryObject](../resources/directoryobject.md) から継承されます。</span><span class="sxs-lookup"><span data-stu-id="1c0f7-p105">A string that identifies the object type. For tenants the value is always “Company”. Inherited from [directoryObject](../resources/directoryobject.md).</span></span>|
|<span data-ttu-id="1c0f7-159">postalCode</span><span class="sxs-lookup"><span data-stu-id="1c0f7-159">postalCode</span></span>|<span data-ttu-id="1c0f7-160">String</span><span class="sxs-lookup"><span data-stu-id="1c0f7-160">String</span></span>|            |
|<span data-ttu-id="1c0f7-161">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="1c0f7-161">preferredLanguage</span></span>|<span data-ttu-id="1c0f7-162">String</span><span class="sxs-lookup"><span data-stu-id="1c0f7-162">String</span></span>|            |
|<span data-ttu-id="1c0f7-163">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="1c0f7-163">provisionedPlans</span></span>|<span data-ttu-id="1c0f7-164">ProvisionedPlan</span><span class="sxs-lookup"><span data-stu-id="1c0f7-164">ProvisionedPlan</span></span>|                                        <span data-ttu-id="1c0f7-165">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="1c0f7-165">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="1c0f7-166">provisioningErrors</span><span class="sxs-lookup"><span data-stu-id="1c0f7-166">provisioningErrors</span></span>|<span data-ttu-id="1c0f7-167">ProvisioningError</span><span class="sxs-lookup"><span data-stu-id="1c0f7-167">ProvisioningError</span></span>|                                        <span data-ttu-id="1c0f7-168">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="1c0f7-168">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="1c0f7-169">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="1c0f7-169">securityComplianceNotificationMails</span></span>|<span data-ttu-id="1c0f7-170">String</span><span class="sxs-lookup"><span data-stu-id="1c0f7-170">String</span></span>||
|<span data-ttu-id="1c0f7-171">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="1c0f7-171">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="1c0f7-172">String</span><span class="sxs-lookup"><span data-stu-id="1c0f7-172">String</span></span>||
|<span data-ttu-id="1c0f7-173">state</span><span class="sxs-lookup"><span data-stu-id="1c0f7-173">state</span></span>|<span data-ttu-id="1c0f7-174">String</span><span class="sxs-lookup"><span data-stu-id="1c0f7-174">String</span></span>|            |
|<span data-ttu-id="1c0f7-175">street</span><span class="sxs-lookup"><span data-stu-id="1c0f7-175">street</span></span>|<span data-ttu-id="1c0f7-176">String</span><span class="sxs-lookup"><span data-stu-id="1c0f7-176">String</span></span>|            |
|<span data-ttu-id="1c0f7-177">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="1c0f7-177">technicalNotificationMails</span></span>|<span data-ttu-id="1c0f7-178">String</span><span class="sxs-lookup"><span data-stu-id="1c0f7-178">String</span></span>|                                        <span data-ttu-id="1c0f7-179">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="1c0f7-179">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="1c0f7-180">telephoneNumber</span><span class="sxs-lookup"><span data-stu-id="1c0f7-180">telephoneNumber</span></span>|<span data-ttu-id="1c0f7-181">String</span><span class="sxs-lookup"><span data-stu-id="1c0f7-181">String</span></span>|            |
|<span data-ttu-id="1c0f7-182">verifiedDomains</span><span class="sxs-lookup"><span data-stu-id="1c0f7-182">verifiedDomains</span></span>|<span data-ttu-id="1c0f7-183">VerifiedDomain</span><span class="sxs-lookup"><span data-stu-id="1c0f7-183">VerifiedDomain</span></span>|<span data-ttu-id="1c0f7-p106">このテナントに関連付けられているドメインのコレクション。                          **注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="1c0f7-p106">The collection of domains associated with this tenant.                            **Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="1c0f7-186">応答</span><span class="sxs-lookup"><span data-stu-id="1c0f7-186">Response</span></span>

<span data-ttu-id="1c0f7-187">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [organization](../resources/organization.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1c0f7-187">If successful, this method returns a `200 OK` response code and updated [organization](../resources/organization.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1c0f7-188">例</span><span class="sxs-lookup"><span data-stu-id="1c0f7-188">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c0f7-189">要求</span><span class="sxs-lookup"><span data-stu-id="1c0f7-189">Request</span></span>
<span data-ttu-id="1c0f7-190">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1c0f7-190">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="1c0f7-191">応答</span><span class="sxs-lookup"><span data-stu-id="1c0f7-191">Response</span></span>
<span data-ttu-id="1c0f7-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1c0f7-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
