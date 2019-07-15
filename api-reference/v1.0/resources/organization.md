---
title: 組織リソースの種類
description: " 作成と削除はサポートされません。 directoryObject から継承します。"
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8b0255883f4e97a7b4aa101073cf0fac1654519e
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621397"
---
# <a name="organization-resource-type"></a><span data-ttu-id="75a0e-104">組織リソースの種類</span><span class="sxs-lookup"><span data-stu-id="75a0e-104">organization resource type</span></span>

<span data-ttu-id="75a0e-105">ユーザーやアプリケーションがサインインする Azure Active Directory テナントを表します。</span><span class="sxs-lookup"><span data-stu-id="75a0e-105">Represents the Azure Active Directory tenant that the user or application is signed in to.</span></span> <span data-ttu-id="75a0e-106">このリソースでは読み取りおよび更新操作のみがサポートされ、作成と削除はサポートされません。</span><span class="sxs-lookup"><span data-stu-id="75a0e-106">Only the read and update operations are supported on this resource; create and delete are not supported.</span></span> <span data-ttu-id="75a0e-107">[directoryObject](directoryobject.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="75a0e-107">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="75a0e-108">このリソースでは、[拡張機能](/graph/extensibility-overview)を使用してカスタム プロパティに独自のデータを追加することができます。</span><span class="sxs-lookup"><span data-stu-id="75a0e-108">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="75a0e-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="75a0e-109">Methods</span></span>

| <span data-ttu-id="75a0e-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="75a0e-110">Method</span></span>       | <span data-ttu-id="75a0e-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="75a0e-111">Return Type</span></span>  |<span data-ttu-id="75a0e-112">説明</span><span class="sxs-lookup"><span data-stu-id="75a0e-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="75a0e-113">組織を取得する</span><span class="sxs-lookup"><span data-stu-id="75a0e-113">Get organization</span></span>](../api/organization-get.md) | [<span data-ttu-id="75a0e-114">organization</span><span class="sxs-lookup"><span data-stu-id="75a0e-114">organization</span></span>](organization.md) |<span data-ttu-id="75a0e-115">組織オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="75a0e-115">Read properties and relationships of organization object.</span></span>|
|[<span data-ttu-id="75a0e-116">Update</span><span class="sxs-lookup"><span data-stu-id="75a0e-116">Update</span></span>](../api/organization-update.md) | [<span data-ttu-id="75a0e-117">organization</span><span class="sxs-lookup"><span data-stu-id="75a0e-117">organization</span></span>](organization.md)  |<span data-ttu-id="75a0e-118">organization オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="75a0e-118">Update organization object.</span></span> <span data-ttu-id="75a0e-119">更新できるプロパティは、**marketingNotificationMails**、**technicalNotificationMails**、**securityComplianceNotificationMails**、**securityComplianceNotificationPhones**、**privacyProfile** のみです。</span><span class="sxs-lookup"><span data-stu-id="75a0e-119">The only properties that can be updated are: **marketingNotificationMails**, **technicalNotificationMails**, **securityComplianceNotificationMails**, **securityComplianceNotificationPhones** and **privacyProfile**.</span></span> |
|<span data-ttu-id="75a0e-120">**オープン拡張機能**</span><span class="sxs-lookup"><span data-stu-id="75a0e-120">**Open extensions**</span></span>| 
|[<span data-ttu-id="75a0e-121">オープン拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="75a0e-121">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="75a0e-122">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="75a0e-122">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="75a0e-123">オープン拡張機能を作成し、新規または既存のリソースにカスタム プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="75a0e-123">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="75a0e-124">オープン拡張機能を取得する</span><span class="sxs-lookup"><span data-stu-id="75a0e-124">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="75a0e-125">[openTypeExtension](opentypeextension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="75a0e-125">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="75a0e-126">拡張機能の名前で識別されるオープン拡張機能を取得します。</span><span class="sxs-lookup"><span data-stu-id="75a0e-126">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="75a0e-127">**スキーマ拡張機能**</span><span class="sxs-lookup"><span data-stu-id="75a0e-127">**Schema extensions**</span></span>| 
|[<span data-ttu-id="75a0e-128">スキーマ拡張機能の値を追加する</span><span class="sxs-lookup"><span data-stu-id="75a0e-128">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="75a0e-129">スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。</span><span class="sxs-lookup"><span data-stu-id="75a0e-129">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|

## <a name="properties"></a><span data-ttu-id="75a0e-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75a0e-130">Properties</span></span>

| <span data-ttu-id="75a0e-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75a0e-131">Property</span></span> | <span data-ttu-id="75a0e-132">型</span><span class="sxs-lookup"><span data-stu-id="75a0e-132">Type</span></span> | <span data-ttu-id="75a0e-133">説明</span><span class="sxs-lookup"><span data-stu-id="75a0e-133">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="75a0e-134">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="75a0e-134">assignedPlans</span></span> | <span data-ttu-id="75a0e-135">[assignedPlan](assignedplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="75a0e-135">[assignedPlan](assignedplan.md) collection</span></span> | <span data-ttu-id="75a0e-p104">テナントに関連付けられているサービス プランのコレクション。null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="75a0e-p104">The collection of service plans associated with the tenant. Not nullable.</span></span> |
| <span data-ttu-id="75a0e-138">businessPhones</span><span class="sxs-lookup"><span data-stu-id="75a0e-138">businessPhones</span></span> | <span data-ttu-id="75a0e-139">String コレクション</span><span class="sxs-lookup"><span data-stu-id="75a0e-139">String collection</span></span> | <span data-ttu-id="75a0e-140">組織の電話番号。</span><span class="sxs-lookup"><span data-stu-id="75a0e-140">Telephone number for the organization.</span></span> <span data-ttu-id="75a0e-141">メモ: 文字列コレクションですが、このプロパティに設定できるのは 1 つの数字のみです。</span><span class="sxs-lookup"><span data-stu-id="75a0e-141">NOTE: Although this is a string collection, only one number can be set for this property.</span></span> |
| <span data-ttu-id="75a0e-142">city</span><span class="sxs-lookup"><span data-stu-id="75a0e-142">city</span></span> | <span data-ttu-id="75a0e-143">String</span><span class="sxs-lookup"><span data-stu-id="75a0e-143">String</span></span> | <span data-ttu-id="75a0e-144">組織の住所の市区町村名。</span><span class="sxs-lookup"><span data-stu-id="75a0e-144">City name of the address for the organization</span></span> |
| <span data-ttu-id="75a0e-145">country</span><span class="sxs-lookup"><span data-stu-id="75a0e-145">country</span></span> | <span data-ttu-id="75a0e-146">String</span><span class="sxs-lookup"><span data-stu-id="75a0e-146">String</span></span> | <span data-ttu-id="75a0e-147">組織の住所の国/地域名。</span><span class="sxs-lookup"><span data-stu-id="75a0e-147">Country/region name of the address for the organization</span></span> |
| <span data-ttu-id="75a0e-148">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="75a0e-148">countryLetterCode</span></span> | <span data-ttu-id="75a0e-149">String</span><span class="sxs-lookup"><span data-stu-id="75a0e-149">String</span></span> | <span data-ttu-id="75a0e-150">組織の国/地域の略称。</span><span class="sxs-lookup"><span data-stu-id="75a0e-150">Country/region abbreviation for the organization</span></span> |
| <span data-ttu-id="75a0e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="75a0e-151">createdDateTime</span></span> | <span data-ttu-id="75a0e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75a0e-152">DateTimeOffset</span></span> | <span data-ttu-id="75a0e-153">組織作成時のタイムスタンプです。</span><span class="sxs-lookup"><span data-stu-id="75a0e-153">Timestamp of when the organization was created.</span></span> <span data-ttu-id="75a0e-154">値は変更できず、組織が作成されると自動的に設定されます。</span><span class="sxs-lookup"><span data-stu-id="75a0e-154">The value cannot be modified and is automatically populated when the organization is created.</span></span> <span data-ttu-id="75a0e-155">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="75a0e-155">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="75a0e-156">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="75a0e-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="75a0e-157">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="75a0e-157">Read-only.</span></span> |
| <span data-ttu-id="75a0e-158">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="75a0e-158">deletedDateTime</span></span> | <span data-ttu-id="75a0e-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75a0e-159">DateTimeOffset</span></span> | <span data-ttu-id="75a0e-160">ISO 8601 形式を使用して Azure AD テナントが削除されたときの日時を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="75a0e-160">Represents date and time of when the Azure AD tenant was deleted using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="75a0e-161">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります: `'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="75a0e-161">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="75a0e-162">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="75a0e-162">Read-only.</span></span> |
| <span data-ttu-id="75a0e-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="75a0e-163">createdDateTime</span></span> | <span data-ttu-id="75a0e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75a0e-164">DateTimeOffset</span></span> | <span data-ttu-id="75a0e-165">組織作成時のタイムスタンプです。</span><span class="sxs-lookup"><span data-stu-id="75a0e-165">Timestamp of when the organization was created.</span></span> <span data-ttu-id="75a0e-166">値は変更できず、組織が作成されると自動的に設定されます。</span><span class="sxs-lookup"><span data-stu-id="75a0e-166">The value cannot be modified and is automatically populated when the organization is created.</span></span> <span data-ttu-id="75a0e-167">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="75a0e-167">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="75a0e-168">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="75a0e-168">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="75a0e-169">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="75a0e-169">Read-only.</span></span> |
| <span data-ttu-id="75a0e-170">displayName</span><span class="sxs-lookup"><span data-stu-id="75a0e-170">displayName</span></span> | <span data-ttu-id="75a0e-171">String</span><span class="sxs-lookup"><span data-stu-id="75a0e-171">String</span></span> | <span data-ttu-id="75a0e-172">テナントの表示名。</span><span class="sxs-lookup"><span data-stu-id="75a0e-172">The display name for the tenant.</span></span> |
| <span data-ttu-id="75a0e-173">id</span><span class="sxs-lookup"><span data-stu-id="75a0e-173">id</span></span> | <span data-ttu-id="75a0e-174">String</span><span class="sxs-lookup"><span data-stu-id="75a0e-174">String</span></span> | <span data-ttu-id="75a0e-175">テナント ID。組織 (またはテナント) を表す一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="75a0e-175">The tenant ID, a unique identifier representing the organization (or tenant).</span></span> <span data-ttu-id="75a0e-176">[directoryObject](directoryobject.md) から継承されました。</span><span class="sxs-lookup"><span data-stu-id="75a0e-176">Inherited from [directoryObject](directoryobject.md).</span></span> <span data-ttu-id="75a0e-177">キー。</span><span class="sxs-lookup"><span data-stu-id="75a0e-177">Key.</span></span> <span data-ttu-id="75a0e-178">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="75a0e-178">Not nullable.</span></span> <span data-ttu-id="75a0e-179">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="75a0e-179">Read-only.</span></span> |
| <span data-ttu-id="75a0e-180">isMultipleDataLocationsForServicesEnabled</span><span class="sxs-lookup"><span data-stu-id="75a0e-180">isMultipleDataLocationsForServicesEnabled</span></span> | <span data-ttu-id="75a0e-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="75a0e-181">Boolean</span></span> | <span data-ttu-id="75a0e-182">組織の Multi-Geo が有効の場合 **true**、組織の Multi-Geo が有効ではない場合 **false**、**null** (既定)。</span><span class="sxs-lookup"><span data-stu-id="75a0e-182">**true** if organization is Multi-Geo enabled; **false** if organization is not Multi-Geo enabled; **null** (default).</span></span> <span data-ttu-id="75a0e-183">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="75a0e-183">Read-only.</span></span> <span data-ttu-id="75a0e-184">詳細については、「[OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="75a0e-184">For more information, see [OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).</span></span> |
| <span data-ttu-id="75a0e-185">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="75a0e-185">marketingNotificationEmails</span></span> | <span data-ttu-id="75a0e-186">String collection</span><span class="sxs-lookup"><span data-stu-id="75a0e-186">String collection</span></span> | <span data-ttu-id="75a0e-187">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="75a0e-187">Not nullable.</span></span> |
| <span data-ttu-id="75a0e-188">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="75a0e-188">onPremisesLastSyncDateTime</span></span> | <span data-ttu-id="75a0e-189">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75a0e-189">DateTimeOffset</span></span> | <span data-ttu-id="75a0e-190">前回テナントがオンプレミスのディレクトリと同期した日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="75a0e-190">The time and date at which the tenant was last synced with the on-premise directory.</span></span> <span data-ttu-id="75a0e-191">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="75a0e-191">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="75a0e-192">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="75a0e-192">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="75a0e-193">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="75a0e-193">Read-only.</span></span> |
| <span data-ttu-id="75a0e-194">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="75a0e-194">onPremisesSyncEnabled</span></span> | <span data-ttu-id="75a0e-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="75a0e-195">Boolean</span></span> | <span data-ttu-id="75a0e-196">このオブジェクトがオンプレミスのディレクトリから同期される場合は **true**。このオブジェクトが最初にオンプレミスのディレクトリから同期されていて、今後は同期されない場合は **false**。このオブジェクトがオンプレミスのディレクトリから一度も同期されたことがない場合は **null** (既定値)。</span><span class="sxs-lookup"><span data-stu-id="75a0e-196">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default).</span></span> |
| <span data-ttu-id="75a0e-197">postalCode</span><span class="sxs-lookup"><span data-stu-id="75a0e-197">postalCode</span></span> | <span data-ttu-id="75a0e-198">String</span><span class="sxs-lookup"><span data-stu-id="75a0e-198">String</span></span> | <span data-ttu-id="75a0e-199">組織の住所の郵便番号。</span><span class="sxs-lookup"><span data-stu-id="75a0e-199">Postal code of the address for the organization</span></span> |
| <span data-ttu-id="75a0e-200">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="75a0e-200">preferredLanguage</span></span> | <span data-ttu-id="75a0e-201">String</span><span class="sxs-lookup"><span data-stu-id="75a0e-201">String</span></span> | <span data-ttu-id="75a0e-202">組織の優先言語。</span><span class="sxs-lookup"><span data-stu-id="75a0e-202">The preferred language for the organization.</span></span> <span data-ttu-id="75a0e-203">ISO 639-1 コードに従う必要があります (例: "en")。</span><span class="sxs-lookup"><span data-stu-id="75a0e-203">Should follow ISO 639-1 Code; for example "en".</span></span> |
| <span data-ttu-id="75a0e-204">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="75a0e-204">privacyProfile</span></span> | [<span data-ttu-id="75a0e-205">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="75a0e-205">privacyProfile</span></span>](privacyprofile.md) | <span data-ttu-id="75a0e-206">組織のプライバシー プロファイル。</span><span class="sxs-lookup"><span data-stu-id="75a0e-206">The privacy profile of an organization.</span></span> |
| <span data-ttu-id="75a0e-207">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="75a0e-207">provisionedPlans</span></span> | <span data-ttu-id="75a0e-208">[ProvisionedPlan](provisionedplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="75a0e-208">[ProvisionedPlan](provisionedplan.md) collection</span></span> | <span data-ttu-id="75a0e-209">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="75a0e-209">Not nullable.</span></span> |
| <span data-ttu-id="75a0e-210">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="75a0e-210">securityComplianceNotificationMails</span></span> | <span data-ttu-id="75a0e-211">String collection</span><span class="sxs-lookup"><span data-stu-id="75a0e-211">String collection</span></span> ||
| <span data-ttu-id="75a0e-212">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="75a0e-212">securityComplianceNotificationPhones</span></span> | <span data-ttu-id="75a0e-213">String collection</span><span class="sxs-lookup"><span data-stu-id="75a0e-213">String collection</span></span>||
| <span data-ttu-id="75a0e-214">state</span><span class="sxs-lookup"><span data-stu-id="75a0e-214">state</span></span> | <span data-ttu-id="75a0e-215">String</span><span class="sxs-lookup"><span data-stu-id="75a0e-215">String</span></span> | <span data-ttu-id="75a0e-216">組織の住所の都道府県名。</span><span class="sxs-lookup"><span data-stu-id="75a0e-216">State name of the address for the organization</span></span> |
| <span data-ttu-id="75a0e-217">街路</span><span class="sxs-lookup"><span data-stu-id="75a0e-217">street</span></span> | <span data-ttu-id="75a0e-218">String</span><span class="sxs-lookup"><span data-stu-id="75a0e-218">String</span></span> | <span data-ttu-id="75a0e-219">組織の住所の番地。</span><span class="sxs-lookup"><span data-stu-id="75a0e-219">Street name of the address for organization</span></span> |
| <span data-ttu-id="75a0e-220">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="75a0e-220">technicalNotificationMails</span></span> | <span data-ttu-id="75a0e-221">String collection</span><span class="sxs-lookup"><span data-stu-id="75a0e-221">String collection</span></span> | <span data-ttu-id="75a0e-222">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="75a0e-222">Not nullable.</span></span> |
| <span data-ttu-id="75a0e-223">verifiedDomains</span><span class="sxs-lookup"><span data-stu-id="75a0e-223">verifiedDomains</span></span> | <span data-ttu-id="75a0e-224">[VerifiedDomain](verifieddomain.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="75a0e-224">[VerifiedDomain](verifieddomain.md) collection</span></span> | <span data-ttu-id="75a0e-p113">このテナントに関連付けられているドメインのコレクション。null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="75a0e-p113">The collection of domains associated with this tenant. Not nullable.</span></span> |

## <a name="relationships"></a><span data-ttu-id="75a0e-227">関係</span><span class="sxs-lookup"><span data-stu-id="75a0e-227">Relationships</span></span>
| <span data-ttu-id="75a0e-228">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="75a0e-228">Relationship</span></span> | <span data-ttu-id="75a0e-229">型</span><span class="sxs-lookup"><span data-stu-id="75a0e-229">Type</span></span>   |<span data-ttu-id="75a0e-230">説明</span><span class="sxs-lookup"><span data-stu-id="75a0e-230">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75a0e-231">extensions</span><span class="sxs-lookup"><span data-stu-id="75a0e-231">extensions</span></span>|<span data-ttu-id="75a0e-232">[extension](extension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="75a0e-232">[extension](extension.md) collection</span></span>|<span data-ttu-id="75a0e-p114">組織に対して定義されているオープン拡張機能のコレクション。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="75a0e-p114">The collection of open extensions defined for the organization. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="75a0e-236">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="75a0e-236">JSON representation</span></span>

<span data-ttu-id="75a0e-237">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="75a0e-237">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "extensions"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.organization"
}-->

```json
{
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "businessPhones": ["string"],
  "city": "string",
  "country": "string",
  "countryLetterCode": "string",
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "displayName": "string",
  "id": "string (identifier)",
  "isMultipleDataLocationsForServicesEnabled": "boolean",
  "marketingNotificationEmails": ["string"],
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "postalCode": "string",
  "preferredLanguage": "string",
  "privacyProfile": {"@odata.type": "microsoft.graph.privacyProfile"},
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "securityComplianceNotificationMails": ["string"],
  "securityComplianceNotificationPhones": ["string"],
  "state": "string",
  "street": "string",
  "technicalNotificationMails": ["string"],
  "verifiedDomains": [{"@odata.type": "microsoft.graph.verifiedDomain"}]
}
```

## <a name="see-also"></a><span data-ttu-id="75a0e-238">関連項目</span><span class="sxs-lookup"><span data-stu-id="75a0e-238">See also</span></span>

- [<span data-ttu-id="75a0e-239">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="75a0e-239">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="75a0e-240">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="75a0e-240">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="75a0e-241">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="75a0e-241">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organization resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'businessPhones' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'onPremisesLastSyncDateTime' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'onPremisesSyncEnabled' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'securityComplianceNotificationMails' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'securityComplianceNotificationPhones' found in resource definition for 'microsoft.graph.organization', but not described in markdown table."
  ],
  "tocPath": ""
}-->
