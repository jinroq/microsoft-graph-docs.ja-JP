---
title: educationSynchronizationProfile リソースの種類
description: 教育機関のエンティティおよび名簿の情報をソースディレクトリから azure Active directory (azure AD) に同期するために使用される構成のセットを表します。 このリソースは、School Data Sync で使用されるプログラム的な表現を提供します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 1926c591a679bd4fd97ceeeb7fab542af9e02544
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334045"
---
# <a name="educationsynchronizationprofile-resource-type"></a><span data-ttu-id="043d3-104">educationSynchronizationProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="043d3-104">educationSynchronizationProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="043d3-105">教育機関のエンティティおよび名簿の情報をソースディレクトリから azure Active directory (azure AD) に同期するために使用される構成のセットを表します。</span><span class="sxs-lookup"><span data-stu-id="043d3-105">Represents a set of configurations used to synchronize education entities and roster information from a source directory to Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="043d3-106">このリソースは、 [School Data Sync](https://sds.microsoft.com)で使用されるプログラム的な表現を提供します。</span><span class="sxs-lookup"><span data-stu-id="043d3-106">This resource provides a programmatic representation used in [School Data Sync](https://sds.microsoft.com).</span></span>

## <a name="methods"></a><span data-ttu-id="043d3-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="043d3-107">Methods</span></span>

| <span data-ttu-id="043d3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="043d3-108">Method</span></span> | <span data-ttu-id="043d3-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="043d3-109">Return Type</span></span> | <span data-ttu-id="043d3-110">説明</span><span class="sxs-lookup"><span data-stu-id="043d3-110">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="043d3-111">同期プロファイルの一覧表示</span><span class="sxs-lookup"><span data-stu-id="043d3-111">List synchronization profiles</span></span>](../api/educationsynchronizationprofile-list.md) | <span data-ttu-id="043d3-112">**educationSynchronizationProfile**コレクション</span><span class="sxs-lookup"><span data-stu-id="043d3-112">**educationSynchronizationProfile** collection</span></span> | <span data-ttu-id="043d3-113">テナント内のすべての同期プロファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="043d3-113">Get a list of all the synchronization profiles in the tenant.</span></span> |
| [<span data-ttu-id="043d3-114">同期プロファイルを取得する</span><span class="sxs-lookup"><span data-stu-id="043d3-114">Get synchronization profile</span></span>](../api/educationsynchronizationprofile-get.md) | <span data-ttu-id="043d3-115">**educationSynchronizationProfile**</span><span class="sxs-lookup"><span data-stu-id="043d3-115">**educationSynchronizationProfile**</span></span> | <span data-ttu-id="043d3-116">プロファイル識別子を指定して、特定のプロファイルを取得します。</span><span class="sxs-lookup"><span data-stu-id="043d3-116">Retrieve a specific profile given the profile identifier.</span></span> |
| [<span data-ttu-id="043d3-117">同期プロファイルの作成</span><span class="sxs-lookup"><span data-stu-id="043d3-117">Create synchronization profile</span></span>](../api/educationsynchronizationprofile-post.md) | <span data-ttu-id="043d3-118">なし</span><span class="sxs-lookup"><span data-stu-id="043d3-118">None</span></span> | <span data-ttu-id="043d3-119">新しい同期プロファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="043d3-119">Create a new synchronization profile.</span></span> |
| [<span data-ttu-id="043d3-120">同期プロファイルの削除</span><span class="sxs-lookup"><span data-stu-id="043d3-120">Delete synchronization profile</span></span>](../api/educationsynchronizationprofile-delete.md) | <span data-ttu-id="043d3-121">**educationSynchronizationProfile**</span><span class="sxs-lookup"><span data-stu-id="043d3-121">**educationSynchronizationProfile**</span></span> | <span data-ttu-id="043d3-122">プロファイル識別子を指定して、特定のプロファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="043d3-122">Delete a specific profile given the profile identifier.</span></span> |
| [<span data-ttu-id="043d3-123">進行中の同期を一時停止する</span><span class="sxs-lookup"><span data-stu-id="043d3-123">Pause an ongoing sync</span></span>](../api/educationsynchronizationprofile-pause.md) | <span data-ttu-id="043d3-124">なし</span><span class="sxs-lookup"><span data-stu-id="043d3-124">None</span></span> | <span data-ttu-id="043d3-125">進行中の同期を一時停止します。</span><span class="sxs-lookup"><span data-stu-id="043d3-125">Pause an ongoing synchronization.</span></span> |
| [<span data-ttu-id="043d3-126">一時停止した同期を再開する</span><span class="sxs-lookup"><span data-stu-id="043d3-126">Resume a paused sync</span></span>](../api/educationsynchronizationprofile-resume.md) | <span data-ttu-id="043d3-127">なし</span><span class="sxs-lookup"><span data-stu-id="043d3-127">None</span></span> | <span data-ttu-id="043d3-128">一時停止した同期を再開します。</span><span class="sxs-lookup"><span data-stu-id="043d3-128">Resume a paused synchronization.</span></span> |
| [<span data-ttu-id="043d3-129">同期をリセットする</span><span class="sxs-lookup"><span data-stu-id="043d3-129">Reset a sync</span></span>](../api/educationsynchronizationprofile-reset.md) | <span data-ttu-id="043d3-130">なし</span><span class="sxs-lookup"><span data-stu-id="043d3-130">None</span></span> | <span data-ttu-id="043d3-131">プロファイルの状態をリセットし、同期を再開します。</span><span class="sxs-lookup"><span data-stu-id="043d3-131">Reset the state of the profile and restart synchronization.</span></span> |
| [<span data-ttu-id="043d3-132">アップロードしたファイルの同期を開始する</span><span class="sxs-lookup"><span data-stu-id="043d3-132">Start sync for uploaded files</span></span>](../api/educationsynchronizationprofile-start.md) | <span data-ttu-id="043d3-133">[educationFileSynchronizationVerificationMessage](educationfilesynchronizationverificationmessage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="043d3-133">[educationFileSynchronizationVerificationMessage](educationfilesynchronizationverificationmessage.md) collection</span></span>| <span data-ttu-id="043d3-134">アップロードしたソースファイルを確認し、同期を開始します。</span><span class="sxs-lookup"><span data-stu-id="043d3-134">Verify the uploaded source files and start synchronization.</span></span> <span data-ttu-id="043d3-135">データプロバイダーが[educationCsvDataProvider](educationcsvdataprovider.md)の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="043d3-135">Applies only when the data provider is [educationCsvDataProvider](educationcsvdataprovider.md).</span></span> |
| [<span data-ttu-id="043d3-136">アップロード URL を取得する</span><span class="sxs-lookup"><span data-stu-id="043d3-136">Get an upload URL</span></span>](../api/educationsynchronizationprofile-uploadurl.md) | <span data-ttu-id="043d3-137">string</span><span class="sxs-lookup"><span data-stu-id="043d3-137">string</span></span> | <span data-ttu-id="043d3-138">CSV データファイルをアップロードするための短時間の URL を返します。</span><span class="sxs-lookup"><span data-stu-id="043d3-138">Return the short-lived URL to upload CSV data files.</span></span> <span data-ttu-id="043d3-139">データプロバイダーが[educationCsvDataProvider](educationcsvdataprovider.md)の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="043d3-139">Applies only when the data provider is [educationCsvDataProvider](educationcsvdataprovider.md).</span></span> |
| [<span data-ttu-id="043d3-140">同期の状態を取得する</span><span class="sxs-lookup"><span data-stu-id="043d3-140">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | [<span data-ttu-id="043d3-141">status</span><span class="sxs-lookup"><span data-stu-id="043d3-141">status</span></span>](educationsynchronizationprofilestatus.md) | <span data-ttu-id="043d3-142">特定の同期プロファイルの状態を返します。</span><span class="sxs-lookup"><span data-stu-id="043d3-142">Return the status of a specific synchronization profile.</span></span> |
| [<span data-ttu-id="043d3-143">同期エラーを取得する</span><span class="sxs-lookup"><span data-stu-id="043d3-143">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="043d3-144">[educationSynchronizationError](educationsynchronizationerror.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="043d3-144">[educationSynchronizationError](educationsynchronizationerror.md) collection</span></span>| <span data-ttu-id="043d3-145">同期中に生成されたすべてのエラーを取得します。</span><span class="sxs-lookup"><span data-stu-id="043d3-145">Get all the errors generated during synchronization.</span></span> |

## <a name="properties"></a><span data-ttu-id="043d3-146">プロパティ</span><span class="sxs-lookup"><span data-stu-id="043d3-146">Properties</span></span>

| <span data-ttu-id="043d3-147">プロパティ</span><span class="sxs-lookup"><span data-stu-id="043d3-147">Property</span></span> | <span data-ttu-id="043d3-148">型</span><span class="sxs-lookup"><span data-stu-id="043d3-148">Type</span></span> | <span data-ttu-id="043d3-149">説明</span><span class="sxs-lookup"><span data-stu-id="043d3-149">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="043d3-150">**displayName**</span><span class="sxs-lookup"><span data-stu-id="043d3-150">**displayName**</span></span> | <span data-ttu-id="043d3-151">string</span><span class="sxs-lookup"><span data-stu-id="043d3-151">string</span></span> |  <span data-ttu-id="043d3-152">id を同期するための構成プロファイルの名前。</span><span class="sxs-lookup"><span data-stu-id="043d3-152">Name of the configuration profile for syncing identities.</span></span>         |
| <span data-ttu-id="043d3-153">**プロバイダー**</span><span class="sxs-lookup"><span data-stu-id="043d3-153">**dataProvider**</span></span> | [<span data-ttu-id="043d3-154">educationSynchronizationDataProvider</span><span class="sxs-lookup"><span data-stu-id="043d3-154">educationSynchronizationDataProvider</span></span>](educationsynchronizationdataprovider.md) |  <span data-ttu-id="043d3-155">プロファイルに使用されるデータプロバイダー。</span><span class="sxs-lookup"><span data-stu-id="043d3-155">The data provider used for the profile.</span></span>         |
| <span data-ttu-id="043d3-156">**id の同期構成**</span><span class="sxs-lookup"><span data-stu-id="043d3-156">**identitySynchronizationConfiguration**</span></span> | [<span data-ttu-id="043d3-157">educationIdentitySynchronizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="043d3-157">educationIdentitySynchronizationConfiguration</span></span>](educationidentitysynchronizationconfiguration.md) | <span data-ttu-id="043d3-158">id の[作成](educationidentitycreationconfiguration.md)または[一致する](educationidentitymatchingconfiguration.md)構成。</span><span class="sxs-lookup"><span data-stu-id="043d3-158">Identity [creation](educationidentitycreationconfiguration.md) or [matching](educationidentitymatchingconfiguration.md) configuration .</span></span>        |
| <span data-ttu-id="043d3-159">**licensestoassign**</span><span class="sxs-lookup"><span data-stu-id="043d3-159">**licensesToAssign**</span></span> | <span data-ttu-id="043d3-160">[educationSynchronizationLicenseAssignment](educationsynchronizationlicenseassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="043d3-160">[educationSynchronizationLicenseAssignment](educationsynchronizationlicenseassignment.md) collection</span></span>|  <span data-ttu-id="043d3-161">ライセンスのセットアップ構成。</span><span class="sxs-lookup"><span data-stu-id="043d3-161">License setup configuration.</span></span>        |
| <span data-ttu-id="043d3-162">**state**</span><span class="sxs-lookup"><span data-stu-id="043d3-162">**state**</span></span> | <span data-ttu-id="043d3-163">educationSynchronizationProfileState</span><span class="sxs-lookup"><span data-stu-id="043d3-163">educationSynchronizationProfileState</span></span> |  <span data-ttu-id="043d3-164">プロファイルの状態。</span><span class="sxs-lookup"><span data-stu-id="043d3-164">The state of the profile.</span></span> <span data-ttu-id="043d3-165">可能な値は、`provisioning`、`provisioned`、`provisioningFailed`、`deleting`、`deletionFailed` です。</span><span class="sxs-lookup"><span data-stu-id="043d3-165">Possible values are: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`.</span></span>          |

## <a name="relationships"></a><span data-ttu-id="043d3-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="043d3-166">Relationships</span></span>

| <span data-ttu-id="043d3-167">プロパティ</span><span class="sxs-lookup"><span data-stu-id="043d3-167">Property</span></span> | <span data-ttu-id="043d3-168">型</span><span class="sxs-lookup"><span data-stu-id="043d3-168">Type</span></span> | <span data-ttu-id="043d3-169">説明</span><span class="sxs-lookup"><span data-stu-id="043d3-169">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="043d3-170">**errors**</span><span class="sxs-lookup"><span data-stu-id="043d3-170">**errors**</span></span> | <span data-ttu-id="043d3-171">[educationSynchronizationError](educationsynchronizationerror.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="043d3-171">[educationSynchronizationError](educationsynchronizationerror.md) collection</span></span>| <span data-ttu-id="043d3-172">この同期プロファイルに関連付けられているすべてのエラー。</span><span class="sxs-lookup"><span data-stu-id="043d3-172">All errors associated with this synchronization profile.</span></span> |
| <span data-ttu-id="043d3-173">**profilestatus**</span><span class="sxs-lookup"><span data-stu-id="043d3-173">**profileStatus**</span></span> | [<span data-ttu-id="043d3-174">educationSynchronizationProfileStatus</span><span class="sxs-lookup"><span data-stu-id="043d3-174">educationSynchronizationProfileStatus</span></span>](educationsynchronizationprofilestatus.md) | <span data-ttu-id="043d3-175">同期の状態。</span><span class="sxs-lookup"><span data-stu-id="043d3-175">The synchronization status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="043d3-176">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="043d3-176">JSON representation</span></span>
<span data-ttu-id="043d3-177">次に示すのは、 **educationSynchronizationProfile**リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="043d3-177">The following is a JSON representation of the **educationSynchronizationProfile** resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationSynchronizationProfile"
}-->

```json
{
    "id": "String",
    "displayName": "String",
    "state": { "@odata.type": "microsoft.graph.educationSynchronizationProfileState" },
    "profileStatus": {"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"},
    "errors": [{"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus" }],
    "dataProvider": { "@odata.type": "microsoft.graph.educationCsvDataProvider" },
    "identitySynchronizationConfiguration": { "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration" },
    "licensesToAssign": [{"@odata.type":"microsoft.graph.educationSynchronizationLicenseAssignment"}],
    "handleSpecialCharacterConstraint": "Boolean"
}
```
