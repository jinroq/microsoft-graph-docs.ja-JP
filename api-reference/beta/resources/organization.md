---
title: 組織リソースの種類
description: 'Azure Active Directory のテナント型を表します。 '
ms.openlocfilehash: 0dc7b55053ba70272c4e639dba4b62160f58f435
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069144"
---
# <a name="organization-resource-type"></a><span data-ttu-id="be4fe-103">組織リソースの種類</span><span class="sxs-lookup"><span data-stu-id="be4fe-103">organization resource type</span></span>

> <span data-ttu-id="be4fe-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="be4fe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be4fe-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be4fe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="be4fe-106">Azure Active Directory のテナント型を表します。</span><span class="sxs-lookup"><span data-stu-id="be4fe-106">Represents an Azure Active Directory tenant.</span></span> 

<span data-ttu-id="be4fe-107">このリソースでは、[拡張機能](/graph/extensibility-overview)を使用してカスタム プロパティに独自のデータを追加することができます。</span><span class="sxs-lookup"><span data-stu-id="be4fe-107">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

<span data-ttu-id="be4fe-108">のみ、読み取りおよび更新操作がサポートされてのテナントです。作成および削除はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be4fe-108">Only the read and update operations are supported on tenants; create and delete are not supported.</span></span> <span data-ttu-id="be4fe-109">[directoryObject](directoryobject.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="be4fe-109">Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="be4fe-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="be4fe-110">Methods</span></span>

| <span data-ttu-id="be4fe-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="be4fe-111">Method</span></span>       | <span data-ttu-id="be4fe-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="be4fe-112">Return Type</span></span>  |<span data-ttu-id="be4fe-113">説明</span><span class="sxs-lookup"><span data-stu-id="be4fe-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="be4fe-114">組織を取得する</span><span class="sxs-lookup"><span data-stu-id="be4fe-114">Get organization</span></span>](../api/organization-get.md) | [<span data-ttu-id="be4fe-115">organization</span><span class="sxs-lookup"><span data-stu-id="be4fe-115">organization</span></span>](organization.md) |<span data-ttu-id="be4fe-116">組織オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="be4fe-116">Read properties and relationships of organization object.</span></span>|
|[<span data-ttu-id="be4fe-117">Update</span><span class="sxs-lookup"><span data-stu-id="be4fe-117">Update</span></span>](../api/organization-update.md) | [<span data-ttu-id="be4fe-118">organization</span><span class="sxs-lookup"><span data-stu-id="be4fe-118">organization</span></span>](organization.md)  |<span data-ttu-id="be4fe-119">organization オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="be4fe-119">Update organization object.</span></span> <span data-ttu-id="be4fe-120">更新できるプロパティは、**marketingNotificationMails**、**technicalNotificationMails**、**securityComplianceNotificationMails**、**securityComplianceNotificationPhones**、**privacyProfile** のみです。</span><span class="sxs-lookup"><span data-stu-id="be4fe-120">The only properties that can be updated are: **marketingNotificationMails**, **technicalNotificationMails**, **securityComplianceNotificationMails**, **securityComplianceNotificationPhones** and **privacyProfile**.</span></span> |
|<span data-ttu-id="be4fe-121">**オープン拡張機能**</span><span class="sxs-lookup"><span data-stu-id="be4fe-121">**Open extensions**</span></span>| | |
|[<span data-ttu-id="be4fe-122">オープン拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="be4fe-122">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="be4fe-123">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="be4fe-123">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="be4fe-124">オープン拡張機能を作成し、新規または既存のリソースにカスタム プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="be4fe-124">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="be4fe-125">オープン拡張機能を取得する</span><span class="sxs-lookup"><span data-stu-id="be4fe-125">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="be4fe-126">[openTypeExtension](opentypeextension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="be4fe-126">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="be4fe-127">拡張機能の名前で識別されるオープン拡張機能を取得します。</span><span class="sxs-lookup"><span data-stu-id="be4fe-127">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="be4fe-128">**スキーマ拡張機能**</span><span class="sxs-lookup"><span data-stu-id="be4fe-128">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="be4fe-129">スキーマ拡張機能の値を追加する</span><span class="sxs-lookup"><span data-stu-id="be4fe-129">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="be4fe-130">スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。</span><span class="sxs-lookup"><span data-stu-id="be4fe-130">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|

## <a name="properties"></a><span data-ttu-id="be4fe-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be4fe-131">Properties</span></span>
| <span data-ttu-id="be4fe-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be4fe-132">Property</span></span>     | <span data-ttu-id="be4fe-133">型</span><span class="sxs-lookup"><span data-stu-id="be4fe-133">Type</span></span>   |<span data-ttu-id="be4fe-134">説明</span><span class="sxs-lookup"><span data-stu-id="be4fe-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be4fe-135">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="be4fe-135">assignedPlans</span></span>|<span data-ttu-id="be4fe-136">[assignedPlan](assignedplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="be4fe-136">[assignedPlan](assignedplan.md) collection</span></span>|<span data-ttu-id="be4fe-p104">テナントに関連付けられているサービス プランのコレクション。null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="be4fe-p104">The collection of service plans associated with the tenant. Not nullable.</span></span>            |
|<span data-ttu-id="be4fe-139">city</span><span class="sxs-lookup"><span data-stu-id="be4fe-139">city</span></span>|<span data-ttu-id="be4fe-140">String</span><span class="sxs-lookup"><span data-stu-id="be4fe-140">String</span></span>| <span data-ttu-id="be4fe-141">組織の住所の市区町村名</span><span class="sxs-lookup"><span data-stu-id="be4fe-141">City name of the address for the organization</span></span> |
|<span data-ttu-id="be4fe-142">companyLastDirSyncTime</span><span class="sxs-lookup"><span data-stu-id="be4fe-142">companyLastDirSyncTime</span></span>|<span data-ttu-id="be4fe-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be4fe-143">DateTimeOffset</span></span>|<span data-ttu-id="be4fe-p105">テナントがオンプレミスのディレクトリと最後に同期した日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="be4fe-p105">The time and date at which the tenant was last synced with the on-premise directory.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="be4fe-146">country</span><span class="sxs-lookup"><span data-stu-id="be4fe-146">country</span></span>|<span data-ttu-id="be4fe-147">String</span><span class="sxs-lookup"><span data-stu-id="be4fe-147">String</span></span>| <span data-ttu-id="be4fe-148">組織の住所の国/地域名</span><span class="sxs-lookup"><span data-stu-id="be4fe-148">Country/region name of the address for the organization</span></span> |
|<span data-ttu-id="be4fe-149">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="be4fe-149">countryLetterCode</span></span>|<span data-ttu-id="be4fe-150">String</span><span class="sxs-lookup"><span data-stu-id="be4fe-150">String</span></span>| <span data-ttu-id="be4fe-151">組織の国/地域の略称</span><span class="sxs-lookup"><span data-stu-id="be4fe-151">Country/region abbreviation for the organization</span></span> |
|<span data-ttu-id="be4fe-152">deletionTimestamp</span><span class="sxs-lookup"><span data-stu-id="be4fe-152">deletionTimestamp</span></span>|<span data-ttu-id="be4fe-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be4fe-153">DateTimeOffset</span></span>|<span data-ttu-id="be4fe-p106">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="be4fe-p106">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="be4fe-156">dirSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="be4fe-156">dirSyncEnabled</span></span>|<span data-ttu-id="be4fe-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="be4fe-157">Boolean</span></span>|<span data-ttu-id="be4fe-158">このオブジェクトがオンプレミスのディレクトリから同期される場合は **true**。このオブジェクトが最初にオンプレミスのディレクトリから同期されていて、今後は同期されない場合は **false**。このオブジェクトがオンプレミスのディレクトリから一度も同期されたことがない場合は **null** (既定値)。</span><span class="sxs-lookup"><span data-stu-id="be4fe-158">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default).</span></span>|
|<span data-ttu-id="be4fe-159">displayName</span><span class="sxs-lookup"><span data-stu-id="be4fe-159">displayName</span></span>|<span data-ttu-id="be4fe-160">String</span><span class="sxs-lookup"><span data-stu-id="be4fe-160">String</span></span>|<span data-ttu-id="be4fe-161">テナントの表示名。</span><span class="sxs-lookup"><span data-stu-id="be4fe-161">The display name for the tenant.</span></span>|
|<span data-ttu-id="be4fe-162">id</span><span class="sxs-lookup"><span data-stu-id="be4fe-162">id</span></span>|<span data-ttu-id="be4fe-163">String</span><span class="sxs-lookup"><span data-stu-id="be4fe-163">String</span></span>|<span data-ttu-id="be4fe-p107">テナントの一意識別子。[directoryObject](directoryobject.md) から継承されます。キー。null 許容ではありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="be4fe-p107">The unique identifier for the tenant. Inherited from [directoryObject](directoryobject.md). Key. Not nullable. Read-only.</span></span>|
|<span data-ttu-id="be4fe-169">isMultipleDataLocationsForServicesEnabled</span><span class="sxs-lookup"><span data-stu-id="be4fe-169">isMultipleDataLocationsForServicesEnabled</span></span>|<span data-ttu-id="be4fe-170">ブール値</span><span class="sxs-lookup"><span data-stu-id="be4fe-170">Boolean</span></span>|<span data-ttu-id="be4fe-171">**true の**場合組織は、複数地域で有効になっています。複数地域が有効な場合は**false**の組織ではありません。**null**(既定値)。</span><span class="sxs-lookup"><span data-stu-id="be4fe-171">**true** if organization is Multi-Geo enabled; **false** if organization is not Multi-Geo enabled; **null** (default).</span></span> <span data-ttu-id="be4fe-172">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="be4fe-172">Read-only.</span></span> <span data-ttu-id="be4fe-173">詳細については、[オンラインの複数の地域 OneDrive](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be4fe-173">For more information, see [OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).</span></span>|
|<span data-ttu-id="be4fe-174">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="be4fe-174">marketingNotificationEmails</span></span>|<span data-ttu-id="be4fe-175">String コレクション</span><span class="sxs-lookup"><span data-stu-id="be4fe-175">String collection</span></span>| <span data-ttu-id="be4fe-176">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="be4fe-176">Not nullable.</span></span>            |
|<span data-ttu-id="be4fe-177">objectType</span><span class="sxs-lookup"><span data-stu-id="be4fe-177">objectType</span></span>|<span data-ttu-id="be4fe-178">String</span><span class="sxs-lookup"><span data-stu-id="be4fe-178">String</span></span>|<span data-ttu-id="be4fe-p109">オブジェクトの種類を識別する文字列です。テナントの場合、値は常に「会社」です。</span><span class="sxs-lookup"><span data-stu-id="be4fe-p109">A string that identifies the object type. For tenants the value is always “Company”.</span></span> |
|<span data-ttu-id="be4fe-181">postalCode</span><span class="sxs-lookup"><span data-stu-id="be4fe-181">postalCode</span></span>|<span data-ttu-id="be4fe-182">String</span><span class="sxs-lookup"><span data-stu-id="be4fe-182">String</span></span>| <span data-ttu-id="be4fe-183">組織の住所の郵便番号</span><span class="sxs-lookup"><span data-stu-id="be4fe-183">Postal code of the address for the organization</span></span> |
|<span data-ttu-id="be4fe-184">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="be4fe-184">preferredLanguage</span></span>|<span data-ttu-id="be4fe-185">String</span><span class="sxs-lookup"><span data-stu-id="be4fe-185">String</span></span>| <span data-ttu-id="be4fe-186">組織の優先言語。</span><span class="sxs-lookup"><span data-stu-id="be4fe-186">The preferred language for the organization.</span></span> <span data-ttu-id="be4fe-187">ISO 639-1 コードに従う必要があります (例: "en")。</span><span class="sxs-lookup"><span data-stu-id="be4fe-187">Should follow ISO 639-1 Code; for example "en".</span></span> |
|<span data-ttu-id="be4fe-188">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="be4fe-188">privacyProfile</span></span>|[<span data-ttu-id="be4fe-189">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="be4fe-189">privacyProfile</span></span>](privacyprofile.md)| <span data-ttu-id="be4fe-190">組織のプライバシー プロファイル。</span><span class="sxs-lookup"><span data-stu-id="be4fe-190">The privacy profile of an organization.</span></span>            |
|<span data-ttu-id="be4fe-191">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="be4fe-191">provisionedPlans</span></span>|<span data-ttu-id="be4fe-192">[ProvisionedPlan](provisionedplan.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="be4fe-192">[ProvisionedPlan](provisionedplan.md) collection</span></span>| <span data-ttu-id="be4fe-193">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="be4fe-193">Not nullable.</span></span>            |
|<span data-ttu-id="be4fe-194">provisioningErrors</span><span class="sxs-lookup"><span data-stu-id="be4fe-194">provisioningErrors</span></span>|<span data-ttu-id="be4fe-195">ProvisioningError コレクション</span><span class="sxs-lookup"><span data-stu-id="be4fe-195">ProvisioningError collection</span></span>| <span data-ttu-id="be4fe-196">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="be4fe-196">Not nullable.</span></span>            |
|<span data-ttu-id="be4fe-197">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="be4fe-197">securityComplianceNotificationMails</span></span>|<span data-ttu-id="be4fe-198">String コレクション</span><span class="sxs-lookup"><span data-stu-id="be4fe-198">String collection</span></span>||
|<span data-ttu-id="be4fe-199">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="be4fe-199">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="be4fe-200">String コレクション</span><span class="sxs-lookup"><span data-stu-id="be4fe-200">String collection</span></span>||
|<span data-ttu-id="be4fe-201">state</span><span class="sxs-lookup"><span data-stu-id="be4fe-201">state</span></span>|<span data-ttu-id="be4fe-202">String</span><span class="sxs-lookup"><span data-stu-id="be4fe-202">String</span></span>| <span data-ttu-id="be4fe-203">組織の住所の都道府県名</span><span class="sxs-lookup"><span data-stu-id="be4fe-203">State name of the address for the organization</span></span> |
|<span data-ttu-id="be4fe-204">street</span><span class="sxs-lookup"><span data-stu-id="be4fe-204">street</span></span>|<span data-ttu-id="be4fe-205">String</span><span class="sxs-lookup"><span data-stu-id="be4fe-205">String</span></span>| <span data-ttu-id="be4fe-206">組織の住所の番地</span><span class="sxs-lookup"><span data-stu-id="be4fe-206">Street name of the address for organization</span></span> |
|<span data-ttu-id="be4fe-207">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="be4fe-207">technicalNotificationMails</span></span>|<span data-ttu-id="be4fe-208">String コレクション</span><span class="sxs-lookup"><span data-stu-id="be4fe-208">String collection</span></span>| <span data-ttu-id="be4fe-209">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="be4fe-209">Not nullable.</span></span> |
|<span data-ttu-id="be4fe-210">telephoneNumber</span><span class="sxs-lookup"><span data-stu-id="be4fe-210">telephoneNumber</span></span>|<span data-ttu-id="be4fe-211">String</span><span class="sxs-lookup"><span data-stu-id="be4fe-211">String</span></span>| <span data-ttu-id="be4fe-212">組織の電話番号</span><span class="sxs-lookup"><span data-stu-id="be4fe-212">Telephone number for the organization</span></span> |
|<span data-ttu-id="be4fe-213">verifiedDomains</span><span class="sxs-lookup"><span data-stu-id="be4fe-213">verifiedDomains</span></span>|<span data-ttu-id="be4fe-214">[VerifiedDomain](verifieddomain.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="be4fe-214">[VerifiedDomain](verifieddomain.md) collection</span></span>|<span data-ttu-id="be4fe-p111">このテナントに関連付けられているドメインのコレクション。null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="be4fe-p111">The collection of domains associated with this tenant. Not nullable.</span></span>            |

## <a name="relationships"></a><span data-ttu-id="be4fe-217">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="be4fe-217">Relationships</span></span>
<span data-ttu-id="be4fe-218">| 拡張子 |[拡張](extension.md)のコレクション。組織のリソースに対して定義されている、開いている拡張機能のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="be4fe-218">|extensions|[extension](extension.md) collection|The collection of open extensions defined for the organization resource.</span></span> <span data-ttu-id="be4fe-219">Null 許容型です |。</span><span class="sxs-lookup"><span data-stu-id="be4fe-219">Nullable.|</span></span>

## <a name="json-representation"></a><span data-ttu-id="be4fe-220">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="be4fe-220">JSON representation</span></span>

<span data-ttu-id="be4fe-221">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="be4fe-221">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="be4fe-222">関連項目</span><span class="sxs-lookup"><span data-stu-id="be4fe-222">See also</span></span>

- [<span data-ttu-id="be4fe-223">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="be4fe-223">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="be4fe-224">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="be4fe-224">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="be4fe-225">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="be4fe-225">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
