---
title: 組織リソースの種類
description: 'Azure Active Directory テナントを表します。 '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 79fc7676752d4f1ba8363c527c46ac50e9f9afff
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966329"
---
# <a name="organization-resource-type"></a><span data-ttu-id="930af-103">組織リソースの種類</span><span class="sxs-lookup"><span data-stu-id="930af-103">organization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="930af-104">ユーザーやアプリケーションがサインインする Azure Active Directory テナントを表します。</span><span class="sxs-lookup"><span data-stu-id="930af-104">Represents the Azure Active Directory tenant that the user or application is signed in to.</span></span> <span data-ttu-id="930af-105">このリソースでは読み取りおよび更新操作のみがサポートされ、作成と削除はサポートされません。</span><span class="sxs-lookup"><span data-stu-id="930af-105">Only the read and update operations are supported on this resource; create and delete are not supported.</span></span> <span data-ttu-id="930af-106">[directoryObject](directoryobject.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="930af-106">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="930af-107">このリソースでは、[拡張機能](/graph/extensibility-overview)を使用してカスタム プロパティに独自のデータを追加することができます。</span><span class="sxs-lookup"><span data-stu-id="930af-107">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="930af-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="930af-108">Methods</span></span>

| <span data-ttu-id="930af-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="930af-109">Method</span></span>       | <span data-ttu-id="930af-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="930af-110">Return Type</span></span>  |<span data-ttu-id="930af-111">説明</span><span class="sxs-lookup"><span data-stu-id="930af-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="930af-112">組織を取得する</span><span class="sxs-lookup"><span data-stu-id="930af-112">Get organization</span></span>](../api/organization-get.md) | [<span data-ttu-id="930af-113">organization</span><span class="sxs-lookup"><span data-stu-id="930af-113">organization</span></span>](organization.md) |<span data-ttu-id="930af-114">組織オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="930af-114">Read properties and relationships of organization object.</span></span>|
|[<span data-ttu-id="930af-115">Update</span><span class="sxs-lookup"><span data-stu-id="930af-115">Update</span></span>](../api/organization-update.md) | [<span data-ttu-id="930af-116">organization</span><span class="sxs-lookup"><span data-stu-id="930af-116">organization</span></span>](organization.md)  |<span data-ttu-id="930af-117">organization オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="930af-117">Update organization object.</span></span> <span data-ttu-id="930af-118">更新できるプロパティは、**marketingNotificationMails**、**technicalNotificationMails**、**securityComplianceNotificationMails**、**securityComplianceNotificationPhones**、**privacyProfile** のみです。</span><span class="sxs-lookup"><span data-stu-id="930af-118">The only properties that can be updated are: **marketingNotificationMails**, **technicalNotificationMails**, **securityComplianceNotificationMails**, **securityComplianceNotificationPhones** and **privacyProfile**.</span></span> |
|<span data-ttu-id="930af-119">**オープン拡張機能**</span><span class="sxs-lookup"><span data-stu-id="930af-119">**Open extensions**</span></span>| | |
|[<span data-ttu-id="930af-120">オープン拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="930af-120">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="930af-121">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="930af-121">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="930af-122">オープン拡張機能を作成し、新規または既存のリソースにカスタム プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="930af-122">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="930af-123">オープン拡張機能を取得する</span><span class="sxs-lookup"><span data-stu-id="930af-123">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="930af-124">[openTypeExtension](opentypeextension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="930af-124">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="930af-125">拡張機能の名前で識別されるオープン拡張機能を取得します。</span><span class="sxs-lookup"><span data-stu-id="930af-125">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="930af-126">**スキーマ拡張機能**</span><span class="sxs-lookup"><span data-stu-id="930af-126">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="930af-127">スキーマ拡張機能の値を追加する</span><span class="sxs-lookup"><span data-stu-id="930af-127">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="930af-128">スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。</span><span class="sxs-lookup"><span data-stu-id="930af-128">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|

## <a name="properties"></a><span data-ttu-id="930af-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="930af-129">Properties</span></span>
| <span data-ttu-id="930af-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="930af-130">Property</span></span> | <span data-ttu-id="930af-131">型</span><span class="sxs-lookup"><span data-stu-id="930af-131">Type</span></span>   | <span data-ttu-id="930af-132">説明</span><span class="sxs-lookup"><span data-stu-id="930af-132">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="930af-133">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="930af-133">assignedPlans</span></span> | <span data-ttu-id="930af-134">[assignedPlan](assignedplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="930af-134">[assignedPlan](assignedplan.md) collection</span></span> | <span data-ttu-id="930af-p103">テナントに関連付けられているサービス プランのコレクション。null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="930af-p103">The collection of service plans associated with the tenant. Not nullable.</span></span> |
| <span data-ttu-id="930af-137">businessPhones</span><span class="sxs-lookup"><span data-stu-id="930af-137">businessPhones</span></span> | <span data-ttu-id="930af-138">String コレクション</span><span class="sxs-lookup"><span data-stu-id="930af-138">String collection</span></span> | <span data-ttu-id="930af-139">組織の電話番号。</span><span class="sxs-lookup"><span data-stu-id="930af-139">Telephone number for the organization.</span></span> <span data-ttu-id="930af-140">**メモ:** 文字列コレクションですが、このプロパティに設定できるのは 1 つの数字のみです。</span><span class="sxs-lookup"><span data-stu-id="930af-140">**Note:** Although this is a string collection, only one number can be set for this property.</span></span> |
| <span data-ttu-id="930af-141">city</span><span class="sxs-lookup"><span data-stu-id="930af-141">city</span></span> | <span data-ttu-id="930af-142">String</span><span class="sxs-lookup"><span data-stu-id="930af-142">String</span></span> | <span data-ttu-id="930af-143">組織の住所の市区町村名。</span><span class="sxs-lookup"><span data-stu-id="930af-143">City name of the address for the organization.</span></span> |
| <span data-ttu-id="930af-144">country</span><span class="sxs-lookup"><span data-stu-id="930af-144">country</span></span> | <span data-ttu-id="930af-145">String</span><span class="sxs-lookup"><span data-stu-id="930af-145">String</span></span> | <span data-ttu-id="930af-146">組織の住所の国/地域名。</span><span class="sxs-lookup"><span data-stu-id="930af-146">Country/region name of the address for the organization.</span></span> |
| <span data-ttu-id="930af-147">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="930af-147">countryLetterCode</span></span> | <span data-ttu-id="930af-148">String</span><span class="sxs-lookup"><span data-stu-id="930af-148">String</span></span> | <span data-ttu-id="930af-149">組織の国/地域の省略形。</span><span class="sxs-lookup"><span data-stu-id="930af-149">Country/region abbreviation for the organization.</span></span> |
| <span data-ttu-id="930af-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="930af-150">createdDateTime</span></span> | <span data-ttu-id="930af-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="930af-151">DateTimeOffset</span></span> | <span data-ttu-id="930af-152">組織作成時のタイムスタンプです。</span><span class="sxs-lookup"><span data-stu-id="930af-152">Timestamp of when the organization was created.</span></span> <span data-ttu-id="930af-153">値は変更できず、組織が作成されると自動的に設定されます。</span><span class="sxs-lookup"><span data-stu-id="930af-153">The value cannot be modified and is automatically populated when the organization is created.</span></span> <span data-ttu-id="930af-154">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="930af-154">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="930af-155">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="930af-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="930af-156">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="930af-156">Read-only.</span></span> |
| <span data-ttu-id="930af-157">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="930af-157">deletedDateTime</span></span> | <span data-ttu-id="930af-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="930af-158">DateTimeOffset</span></span> | <span data-ttu-id="930af-159">ISO 8601 形式を使用して Azure AD テナントが削除されたときの日時を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="930af-159">Represents date and time of when the Azure AD tenant was deleted using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="930af-160">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります: `'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="930af-160">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="930af-161">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="930af-161">Read-only.</span></span> |
| <span data-ttu-id="930af-162">displayName</span><span class="sxs-lookup"><span data-stu-id="930af-162">displayName</span></span> | <span data-ttu-id="930af-163">String</span><span class="sxs-lookup"><span data-stu-id="930af-163">String</span></span> | <span data-ttu-id="930af-164">テナントの表示名。</span><span class="sxs-lookup"><span data-stu-id="930af-164">The display name for the tenant.</span></span> |
| <span data-ttu-id="930af-165">id</span><span class="sxs-lookup"><span data-stu-id="930af-165">id</span></span> | <span data-ttu-id="930af-166">文字列</span><span class="sxs-lookup"><span data-stu-id="930af-166">String</span></span> | <span data-ttu-id="930af-167">テナント ID。組織 (またはテナント) を表す一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="930af-167">The tenant ID, a unique identifier representing the organization (or tenant).</span></span> <span data-ttu-id="930af-168">[directoryObject](directoryobject.md) から継承されました。</span><span class="sxs-lookup"><span data-stu-id="930af-168">Inherited from [directoryObject](directoryobject.md).</span></span> <span data-ttu-id="930af-169">キー。</span><span class="sxs-lookup"><span data-stu-id="930af-169">Key.</span></span> <span data-ttu-id="930af-170">null 許容型ではありません。</span><span class="sxs-lookup"><span data-stu-id="930af-170">Not nullable.</span></span> <span data-ttu-id="930af-171">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="930af-171">Read-only.</span></span> |
| <span data-ttu-id="930af-172">isMultipleDataLocationsForServicesEnabled</span><span class="sxs-lookup"><span data-stu-id="930af-172">isMultipleDataLocationsForServicesEnabled</span></span> | <span data-ttu-id="930af-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="930af-173">Boolean</span></span> | <span data-ttu-id="930af-174">組織の Multi-Geo が有効の場合 **true**、組織の Multi-Geo が有効ではない場合 **false**、**null** (既定)。</span><span class="sxs-lookup"><span data-stu-id="930af-174">**true** if organization is Multi-Geo enabled; **false** if organization is not Multi-Geo enabled; **null** (default).</span></span> <span data-ttu-id="930af-175">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="930af-175">Read-only.</span></span> <span data-ttu-id="930af-176">詳細については、「[OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="930af-176">For more information, see [OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).</span></span> |
| <span data-ttu-id="930af-177">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="930af-177">marketingNotificationEmails</span></span> | <span data-ttu-id="930af-178">String collection</span><span class="sxs-lookup"><span data-stu-id="930af-178">String collection</span></span> | <span data-ttu-id="930af-179">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="930af-179">Not nullable.</span></span> |
| <span data-ttu-id="930af-180">objectType</span><span class="sxs-lookup"><span data-stu-id="930af-180">objectType</span></span> | <span data-ttu-id="930af-181">String</span><span class="sxs-lookup"><span data-stu-id="930af-181">String</span></span> | <span data-ttu-id="930af-p109">オブジェクトの種類を識別する文字列です。テナントの場合、値は常に「会社」です。</span><span class="sxs-lookup"><span data-stu-id="930af-p109">A string that identifies the object type. For tenants the value is always “Company”.</span></span> |
| <span data-ttu-id="930af-184">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="930af-184">onPremisesLastSyncDateTime</span></span> | <span data-ttu-id="930af-185">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="930af-185">DateTimeOffset</span></span> | <span data-ttu-id="930af-186">前回テナントがオンプレミスのディレクトリと同期した日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="930af-186">The time and date at which the tenant was last synced with the on-premise directory.</span></span> <span data-ttu-id="930af-187">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="930af-187">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="930af-188">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="930af-188">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
| <span data-ttu-id="930af-189">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="930af-189">onPremisesSyncEnabled</span></span> | <span data-ttu-id="930af-190">ブール値</span><span class="sxs-lookup"><span data-stu-id="930af-190">Boolean</span></span> | <span data-ttu-id="930af-191">このオブジェクトがオンプレミスのディレクトリから同期される場合は **true**。このオブジェクトが最初にオンプレミスのディレクトリから同期されていて、今後は同期されない場合は **false**。このオブジェクトがオンプレミスのディレクトリから一度も同期されたことがない場合は **null** (既定値)。</span><span class="sxs-lookup"><span data-stu-id="930af-191">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default).</span></span> |
| <span data-ttu-id="930af-192">postalCode</span><span class="sxs-lookup"><span data-stu-id="930af-192">postalCode</span></span> | <span data-ttu-id="930af-193">String</span><span class="sxs-lookup"><span data-stu-id="930af-193">String</span></span> | <span data-ttu-id="930af-194">組織の住所の郵便番号。</span><span class="sxs-lookup"><span data-stu-id="930af-194">Postal code of the address for the organization.</span></span> |
| <span data-ttu-id="930af-195">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="930af-195">preferredLanguage</span></span> | <span data-ttu-id="930af-196">String</span><span class="sxs-lookup"><span data-stu-id="930af-196">String</span></span> | <span data-ttu-id="930af-197">組織の優先言語。</span><span class="sxs-lookup"><span data-stu-id="930af-197">The preferred language for the organization.</span></span> <span data-ttu-id="930af-198">ISO 639-1 コードに従う必要があります (例: "en")。</span><span class="sxs-lookup"><span data-stu-id="930af-198">Should follow ISO 639-1 Code; for example "en".</span></span> |
| <span data-ttu-id="930af-199">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="930af-199">privacyProfile</span></span> | [<span data-ttu-id="930af-200">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="930af-200">privacyProfile</span></span>](privacyprofile.md) | <span data-ttu-id="930af-201">組織のプライバシー プロファイル。</span><span class="sxs-lookup"><span data-stu-id="930af-201">The privacy profile of an organization.</span></span> |
| <span data-ttu-id="930af-202">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="930af-202">provisionedPlans</span></span> | <span data-ttu-id="930af-203">[provisionedPlan](provisionedplan.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="930af-203">[provisionedPlan](provisionedplan.md) collection</span></span> | <span data-ttu-id="930af-204">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="930af-204">Not nullable.</span></span> |
| <span data-ttu-id="930af-205">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="930af-205">securityComplianceNotificationMails</span></span> | <span data-ttu-id="930af-206">String collection</span><span class="sxs-lookup"><span data-stu-id="930af-206">String collection</span></span> ||
| <span data-ttu-id="930af-207">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="930af-207">securityComplianceNotificationPhones</span></span> | <span data-ttu-id="930af-208">String collection</span><span class="sxs-lookup"><span data-stu-id="930af-208">String collection</span></span> ||
| <span data-ttu-id="930af-209">state</span><span class="sxs-lookup"><span data-stu-id="930af-209">state</span></span> | <span data-ttu-id="930af-210">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="930af-210">String</span></span> | <span data-ttu-id="930af-211">組織の住所の都道府県名。</span><span class="sxs-lookup"><span data-stu-id="930af-211">State name of the address for the organization.</span></span> |
| <span data-ttu-id="930af-212">street</span><span class="sxs-lookup"><span data-stu-id="930af-212">street</span></span> | <span data-ttu-id="930af-213">String</span><span class="sxs-lookup"><span data-stu-id="930af-213">String</span></span> | <span data-ttu-id="930af-214">組織の住所のストリート名。</span><span class="sxs-lookup"><span data-stu-id="930af-214">Street name of the address for organization.</span></span> |
| <span data-ttu-id="930af-215">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="930af-215">technicalNotificationMails</span></span> |<span data-ttu-id="930af-216">String collection</span><span class="sxs-lookup"><span data-stu-id="930af-216">String collection</span></span> | <span data-ttu-id="930af-217">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="930af-217">Not nullable.</span></span> |
| <span data-ttu-id="930af-218">verifiedDomains</span><span class="sxs-lookup"><span data-stu-id="930af-218">verifiedDomains</span></span> | <span data-ttu-id="930af-219">[verifiedDomain](verifieddomain.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="930af-219">[verifiedDomain](verifieddomain.md) collection</span></span>|<span data-ttu-id="930af-p112">このテナントに関連付けられているドメインのコレクション。null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="930af-p112">The collection of domains associated with this tenant. Not nullable.</span></span> |

## <a name="relationships"></a><span data-ttu-id="930af-222">関係</span><span class="sxs-lookup"><span data-stu-id="930af-222">Relationships</span></span>

| <span data-ttu-id="930af-223">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="930af-223">Relationship</span></span>     | <span data-ttu-id="930af-224">型</span><span class="sxs-lookup"><span data-stu-id="930af-224">Type</span></span>   |<span data-ttu-id="930af-225">説明</span><span class="sxs-lookup"><span data-stu-id="930af-225">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="930af-226">extensions</span><span class="sxs-lookup"><span data-stu-id="930af-226">extensions</span></span>|<span data-ttu-id="930af-227">[extension](extension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="930af-227">[extension](extension.md) collection</span></span>|<span data-ttu-id="930af-228">組織リソースに対して定義されているオープン拡張機能のコレクション。</span><span class="sxs-lookup"><span data-stu-id="930af-228">The collection of open extensions defined for the organization resource.</span></span> <span data-ttu-id="930af-229">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="930af-229">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="930af-230">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="930af-230">JSON representation</span></span>

<span data-ttu-id="930af-231">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="930af-231">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "extensions"
  ],
  "keyProperty": "id",
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
  "objectType": "string",
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
  "verifiedDomains": [{"@odata.type": "microsoft.graph.verifiedDomain"}],
  "companyLastDirSyncTime": "2019-02-07T20:33:52.942Z",
  "dirSyncEnabled": true
}
```

## <a name="see-also"></a><span data-ttu-id="930af-232">関連項目</span><span class="sxs-lookup"><span data-stu-id="930af-232">See also</span></span>

- [<span data-ttu-id="930af-233">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="930af-233">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="930af-234">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="930af-234">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="930af-235">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="930af-235">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "organization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
