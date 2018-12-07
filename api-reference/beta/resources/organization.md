---
title: 組織リソースの種類
description: 'Azure Active Directory のテナント型を表します。 '
ms.openlocfilehash: 053656eb042ca04f2d487d47ee62624875fa4e17
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191145"
---
# <a name="organization-resource-type"></a><span data-ttu-id="358ab-103">組織リソースの種類</span><span class="sxs-lookup"><span data-stu-id="358ab-103">organization resource type</span></span>

> <span data-ttu-id="358ab-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="358ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="358ab-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="358ab-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="358ab-106">Azure Active Directory のテナント型を表します。</span><span class="sxs-lookup"><span data-stu-id="358ab-106">Represents an Azure Active Directory tenant.</span></span> 

<span data-ttu-id="358ab-107">このリソースでは、[拡張機能](/graph/extensibility-overview)を使用してカスタム プロパティに独自のデータを追加することができます。</span><span class="sxs-lookup"><span data-stu-id="358ab-107">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

<span data-ttu-id="358ab-108">のみ、読み取りおよび更新操作がサポートされてのテナントです。作成および削除はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="358ab-108">Only the read and update operations are supported on tenants; create and delete are not supported.</span></span> <span data-ttu-id="358ab-109">[directoryObject](directoryobject.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="358ab-109">Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="358ab-110">Methods</span><span class="sxs-lookup"><span data-stu-id="358ab-110">Methods</span></span>

| <span data-ttu-id="358ab-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="358ab-111">Method</span></span>       | <span data-ttu-id="358ab-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="358ab-112">Return Type</span></span>  |<span data-ttu-id="358ab-113">説明</span><span class="sxs-lookup"><span data-stu-id="358ab-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="358ab-114">組織を取得する</span><span class="sxs-lookup"><span data-stu-id="358ab-114">Get organization</span></span>](../api/organization-get.md) | [<span data-ttu-id="358ab-115">organization</span><span class="sxs-lookup"><span data-stu-id="358ab-115">organization</span></span>](organization.md) |<span data-ttu-id="358ab-116">組織オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="358ab-116">Read properties and relationships of organization object.</span></span>|
|[<span data-ttu-id="358ab-117">Update</span><span class="sxs-lookup"><span data-stu-id="358ab-117">Update</span></span>](../api/organization-update.md) | [<span data-ttu-id="358ab-118">organization</span><span class="sxs-lookup"><span data-stu-id="358ab-118">organization</span></span>](organization.md)  |<span data-ttu-id="358ab-119">organization オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="358ab-119">Update organization object.</span></span> <span data-ttu-id="358ab-120">更新できるプロパティは、**marketingNotificationMails**、**technicalNotificationMails**、**securityComplianceNotificationMails**、**securityComplianceNotificationPhones**、**privacyProfile** のみです。</span><span class="sxs-lookup"><span data-stu-id="358ab-120">The only properties that can be updated are: **marketingNotificationMails**, **technicalNotificationMails**, **securityComplianceNotificationMails**, **securityComplianceNotificationPhones** and **privacyProfile**.</span></span> |
|<span data-ttu-id="358ab-121">**オープン拡張機能**</span><span class="sxs-lookup"><span data-stu-id="358ab-121">**Open extensions**</span></span>| | |
|[<span data-ttu-id="358ab-122">オープン拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="358ab-122">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="358ab-123">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="358ab-123">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="358ab-124">オープン拡張機能を作成し、新規または既存のリソースにカスタム プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="358ab-124">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="358ab-125">オープン拡張機能を取得する</span><span class="sxs-lookup"><span data-stu-id="358ab-125">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="358ab-126">[openTypeExtension](opentypeextension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="358ab-126">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="358ab-127">拡張機能の名前で識別されるオープン拡張機能を取得します。</span><span class="sxs-lookup"><span data-stu-id="358ab-127">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="358ab-128">**スキーマ拡張機能**</span><span class="sxs-lookup"><span data-stu-id="358ab-128">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="358ab-129">スキーマ拡張機能の値を追加する</span><span class="sxs-lookup"><span data-stu-id="358ab-129">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="358ab-130">スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。</span><span class="sxs-lookup"><span data-stu-id="358ab-130">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|

## <a name="properties"></a><span data-ttu-id="358ab-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="358ab-131">Properties</span></span>
| <span data-ttu-id="358ab-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="358ab-132">Property</span></span>     | <span data-ttu-id="358ab-133">種類</span><span class="sxs-lookup"><span data-stu-id="358ab-133">Type</span></span>   |<span data-ttu-id="358ab-134">説明</span><span class="sxs-lookup"><span data-stu-id="358ab-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="358ab-135">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="358ab-135">assignedPlans</span></span>|<span data-ttu-id="358ab-136">[assignedPlan](assignedplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="358ab-136">[assignedPlan](assignedplan.md) collection</span></span>|<span data-ttu-id="358ab-p104">テナントに関連付けられているサービス プランのコレクション。null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="358ab-p104">The collection of service plans associated with the tenant. Not nullable.</span></span>            |
|<span data-ttu-id="358ab-139">city</span><span class="sxs-lookup"><span data-stu-id="358ab-139">city</span></span>|<span data-ttu-id="358ab-140">String</span><span class="sxs-lookup"><span data-stu-id="358ab-140">String</span></span>| <span data-ttu-id="358ab-141">組織の住所の市区町村名</span><span class="sxs-lookup"><span data-stu-id="358ab-141">City name of the address for the organization</span></span> |
|<span data-ttu-id="358ab-142">companyLastDirSyncTime</span><span class="sxs-lookup"><span data-stu-id="358ab-142">companyLastDirSyncTime</span></span>|<span data-ttu-id="358ab-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="358ab-143">DateTimeOffset</span></span>|<span data-ttu-id="358ab-p105">テナントがオンプレミスのディレクトリと最後に同期した日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="358ab-p105">The time and date at which the tenant was last synced with the on-premise directory.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="358ab-146">country</span><span class="sxs-lookup"><span data-stu-id="358ab-146">country</span></span>|<span data-ttu-id="358ab-147">String</span><span class="sxs-lookup"><span data-stu-id="358ab-147">String</span></span>| <span data-ttu-id="358ab-148">組織の住所の国/地域名</span><span class="sxs-lookup"><span data-stu-id="358ab-148">Country/region name of the address for the organization</span></span> |
|<span data-ttu-id="358ab-149">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="358ab-149">countryLetterCode</span></span>|<span data-ttu-id="358ab-150">String</span><span class="sxs-lookup"><span data-stu-id="358ab-150">String</span></span>| <span data-ttu-id="358ab-151">組織の国/地域の略称</span><span class="sxs-lookup"><span data-stu-id="358ab-151">Country/region abbreviation for the organization</span></span> |
|<span data-ttu-id="358ab-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="358ab-152">createdDateTime</span></span>|<span data-ttu-id="358ab-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="358ab-153">DateTimeOffset</span></span>| <span data-ttu-id="358ab-154">組織が作成された日時のタイムスタンプです。</span><span class="sxs-lookup"><span data-stu-id="358ab-154">Timestamp of when the organization was created.</span></span> <span data-ttu-id="358ab-155">値は変更できず、組織が作成されたときに自動的に設定されます。</span><span class="sxs-lookup"><span data-stu-id="358ab-155">The value cannot be modified and is automatically populated when the organization is created.</span></span> <span data-ttu-id="358ab-156">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="358ab-156">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="358ab-157">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="358ab-157">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="358ab-158">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="358ab-158">Read-only.</span></span> |
|<span data-ttu-id="358ab-159">deletionTimestamp</span><span class="sxs-lookup"><span data-stu-id="358ab-159">deletionTimestamp</span></span>|<span data-ttu-id="358ab-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="358ab-160">DateTimeOffset</span></span>|<span data-ttu-id="358ab-p107">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="358ab-p107">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="358ab-163">dirSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="358ab-163">dirSyncEnabled</span></span>|<span data-ttu-id="358ab-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="358ab-164">Boolean</span></span>|<span data-ttu-id="358ab-165">このオブジェクトがオンプレミスのディレクトリから同期される場合は **true**。このオブジェクトが最初にオンプレミスのディレクトリから同期されていて、今後は同期されない場合は **false**。このオブジェクトがオンプレミスのディレクトリから一度も同期されたことがない場合は **null** (既定値)。</span><span class="sxs-lookup"><span data-stu-id="358ab-165">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default).</span></span>|
|<span data-ttu-id="358ab-166">displayName</span><span class="sxs-lookup"><span data-stu-id="358ab-166">displayName</span></span>|<span data-ttu-id="358ab-167">String</span><span class="sxs-lookup"><span data-stu-id="358ab-167">String</span></span>|<span data-ttu-id="358ab-168">テナントの表示名。</span><span class="sxs-lookup"><span data-stu-id="358ab-168">The display name for the tenant.</span></span>|
|<span data-ttu-id="358ab-169">id</span><span class="sxs-lookup"><span data-stu-id="358ab-169">id</span></span>|<span data-ttu-id="358ab-170">String</span><span class="sxs-lookup"><span data-stu-id="358ab-170">String</span></span>|<span data-ttu-id="358ab-p108">テナントの一意識別子。[directoryObject](directoryobject.md) から継承されます。キー。null 許容ではありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="358ab-p108">The unique identifier for the tenant. Inherited from [directoryObject](directoryobject.md). Key. Not nullable. Read-only.</span></span>|
|<span data-ttu-id="358ab-176">isMultipleDataLocationsForServicesEnabled</span><span class="sxs-lookup"><span data-stu-id="358ab-176">isMultipleDataLocationsForServicesEnabled</span></span>|<span data-ttu-id="358ab-177">ブール型</span><span class="sxs-lookup"><span data-stu-id="358ab-177">Boolean</span></span>|<span data-ttu-id="358ab-178">**true の**場合組織は、複数地域で有効になっています。複数地域が有効な場合は**false**の組織ではありません。**null**(既定値)。</span><span class="sxs-lookup"><span data-stu-id="358ab-178">**true** if organization is Multi-Geo enabled; **false** if organization is not Multi-Geo enabled; **null** (default).</span></span> <span data-ttu-id="358ab-179">取得のみ可能な値です。</span><span class="sxs-lookup"><span data-stu-id="358ab-179">Read-only.</span></span> <span data-ttu-id="358ab-180">詳細については、[オンラインの複数の地域 OneDrive](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="358ab-180">For more information, see [OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).</span></span>|
|<span data-ttu-id="358ab-181">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="358ab-181">marketingNotificationEmails</span></span>|<span data-ttu-id="358ab-182">String コレクション</span><span class="sxs-lookup"><span data-stu-id="358ab-182">String collection</span></span>| <span data-ttu-id="358ab-183">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="358ab-183">Not nullable.</span></span>            |
|<span data-ttu-id="358ab-184">objectType</span><span class="sxs-lookup"><span data-stu-id="358ab-184">objectType</span></span>|<span data-ttu-id="358ab-185">String</span><span class="sxs-lookup"><span data-stu-id="358ab-185">String</span></span>|<span data-ttu-id="358ab-p110">オブジェクトの種類を識別する文字列です。テナントの場合、値は常に「会社」です。</span><span class="sxs-lookup"><span data-stu-id="358ab-p110">A string that identifies the object type. For tenants the value is always “Company”.</span></span> |
|<span data-ttu-id="358ab-188">postalCode</span><span class="sxs-lookup"><span data-stu-id="358ab-188">postalCode</span></span>|<span data-ttu-id="358ab-189">String</span><span class="sxs-lookup"><span data-stu-id="358ab-189">String</span></span>| <span data-ttu-id="358ab-190">組織の住所の郵便番号</span><span class="sxs-lookup"><span data-stu-id="358ab-190">Postal code of the address for the organization</span></span> |
|<span data-ttu-id="358ab-191">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="358ab-191">preferredLanguage</span></span>|<span data-ttu-id="358ab-192">String</span><span class="sxs-lookup"><span data-stu-id="358ab-192">String</span></span>| <span data-ttu-id="358ab-193">組織の優先言語。</span><span class="sxs-lookup"><span data-stu-id="358ab-193">The preferred language for the organization.</span></span> <span data-ttu-id="358ab-194">ISO 639-1 コードに従う必要があります (例: "en")。</span><span class="sxs-lookup"><span data-stu-id="358ab-194">Should follow ISO 639-1 Code; for example "en".</span></span> |
|<span data-ttu-id="358ab-195">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="358ab-195">privacyProfile</span></span>|[<span data-ttu-id="358ab-196">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="358ab-196">privacyProfile</span></span>](privacyprofile.md)| <span data-ttu-id="358ab-197">組織のプライバシー プロファイル。</span><span class="sxs-lookup"><span data-stu-id="358ab-197">The privacy profile of an organization.</span></span>            |
|<span data-ttu-id="358ab-198">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="358ab-198">provisionedPlans</span></span>|<span data-ttu-id="358ab-199">[ProvisionedPlan](provisionedplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="358ab-199">[ProvisionedPlan](provisionedplan.md) collection</span></span>| <span data-ttu-id="358ab-200">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="358ab-200">Not nullable.</span></span>            |
|<span data-ttu-id="358ab-201">provisioningErrors</span><span class="sxs-lookup"><span data-stu-id="358ab-201">provisioningErrors</span></span>|<span data-ttu-id="358ab-202">ProvisioningError コレクション</span><span class="sxs-lookup"><span data-stu-id="358ab-202">ProvisioningError collection</span></span>| <span data-ttu-id="358ab-203">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="358ab-203">Not nullable.</span></span>            |
|<span data-ttu-id="358ab-204">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="358ab-204">securityComplianceNotificationMails</span></span>|<span data-ttu-id="358ab-205">String コレクション</span><span class="sxs-lookup"><span data-stu-id="358ab-205">String collection</span></span>||
|<span data-ttu-id="358ab-206">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="358ab-206">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="358ab-207">String コレクション</span><span class="sxs-lookup"><span data-stu-id="358ab-207">String collection</span></span>||
|<span data-ttu-id="358ab-208">state</span><span class="sxs-lookup"><span data-stu-id="358ab-208">state</span></span>|<span data-ttu-id="358ab-209">String</span><span class="sxs-lookup"><span data-stu-id="358ab-209">String</span></span>| <span data-ttu-id="358ab-210">組織の住所の都道府県名</span><span class="sxs-lookup"><span data-stu-id="358ab-210">State name of the address for the organization</span></span> |
|<span data-ttu-id="358ab-211">street</span><span class="sxs-lookup"><span data-stu-id="358ab-211">street</span></span>|<span data-ttu-id="358ab-212">String</span><span class="sxs-lookup"><span data-stu-id="358ab-212">String</span></span>| <span data-ttu-id="358ab-213">組織の住所の番地</span><span class="sxs-lookup"><span data-stu-id="358ab-213">Street name of the address for organization</span></span> |
|<span data-ttu-id="358ab-214">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="358ab-214">technicalNotificationMails</span></span>|<span data-ttu-id="358ab-215">String コレクション</span><span class="sxs-lookup"><span data-stu-id="358ab-215">String collection</span></span>| <span data-ttu-id="358ab-216">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="358ab-216">Not nullable.</span></span> |
|<span data-ttu-id="358ab-217">telephoneNumber</span><span class="sxs-lookup"><span data-stu-id="358ab-217">telephoneNumber</span></span>|<span data-ttu-id="358ab-218">String</span><span class="sxs-lookup"><span data-stu-id="358ab-218">String</span></span>| <span data-ttu-id="358ab-219">組織の電話番号</span><span class="sxs-lookup"><span data-stu-id="358ab-219">Telephone number for the organization</span></span> |
|<span data-ttu-id="358ab-220">verifiedDomains</span><span class="sxs-lookup"><span data-stu-id="358ab-220">verifiedDomains</span></span>|<span data-ttu-id="358ab-221">[VerifiedDomain](verifieddomain.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="358ab-221">[VerifiedDomain](verifieddomain.md) collection</span></span>|<span data-ttu-id="358ab-p112">このテナントに関連付けられているドメインのコレクション。null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="358ab-p112">The collection of domains associated with this tenant. Not nullable.</span></span>            |

## <a name="relationships"></a><span data-ttu-id="358ab-224">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="358ab-224">Relationships</span></span>
<span data-ttu-id="358ab-225">| 拡張子 |[拡張](extension.md)のコレクション。組織のリソースに対して定義されている、開いている拡張機能のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="358ab-225">|extensions|[extension](extension.md) collection|The collection of open extensions defined for the organization resource.</span></span> <span data-ttu-id="358ab-226">Null 許容型です |。</span><span class="sxs-lookup"><span data-stu-id="358ab-226">Nullable.|</span></span>

## <a name="json-representation"></a><span data-ttu-id="358ab-227">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="358ab-227">JSON representation</span></span>

<span data-ttu-id="358ab-228">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="358ab-228">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="358ab-229">関連項目</span><span class="sxs-lookup"><span data-stu-id="358ab-229">See also</span></span>

- [<span data-ttu-id="358ab-230">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="358ab-230">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="358ab-231">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="358ab-231">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="358ab-232">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="358ab-232">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
