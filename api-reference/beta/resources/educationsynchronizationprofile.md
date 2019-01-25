---
title: educationSynchronizationProfile リソースの種類
description: 教育エンティティと、ソース ディレクトリから Azure Active directory (AD の Azure) の名簿の情報を同期するために使用する構成のセットを表します。 このリソースは、学校のデータの同期で使用されるプログラムの表現を提供します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: e1b81ff14aca2b0f81a7f50e01aed6281d03d14d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523464"
---
# <a name="educationsynchronizationprofile-resource-type"></a><span data-ttu-id="85726-104">educationSynchronizationProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="85726-104">educationSynchronizationProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85726-105">教育エンティティと、ソース ディレクトリから Azure Active directory (AD の Azure) の名簿の情報を同期するために使用する構成のセットを表します。</span><span class="sxs-lookup"><span data-stu-id="85726-105">Represents a set of configurations used to synchronize education entities and roster information from a source directory to Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="85726-106">このリソースは、[学校のデータの同期](https://sds.microsoft.com)で使用されるプログラムの表現を提供します。</span><span class="sxs-lookup"><span data-stu-id="85726-106">This resource provides a programmatic representation used in [School Data Sync](https://sds.microsoft.com).</span></span>

## <a name="methods"></a><span data-ttu-id="85726-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="85726-107">Methods</span></span>

| <span data-ttu-id="85726-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="85726-108">Method</span></span> | <span data-ttu-id="85726-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="85726-109">Return Type</span></span> | <span data-ttu-id="85726-110">説明</span><span class="sxs-lookup"><span data-stu-id="85726-110">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="85726-111">同期プロファイルのリスト</span><span class="sxs-lookup"><span data-stu-id="85726-111">List synchronization profiles</span></span>](../api/educationsynchronizationprofile-list.md) | <span data-ttu-id="85726-112">**educationSynchronizationProfile**コレクション</span><span class="sxs-lookup"><span data-stu-id="85726-112">**educationSynchronizationProfile** collection</span></span> | <span data-ttu-id="85726-113">テナント内のすべての同期プロファイルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="85726-113">Get a list of all the synchronization profiles in the tenant.</span></span> |
| [<span data-ttu-id="85726-114">同期プロファイルを取得します。</span><span class="sxs-lookup"><span data-stu-id="85726-114">Get synchronization profile</span></span>](../api/educationsynchronizationprofile-get.md) | <span data-ttu-id="85726-115">**educationSynchronizationProfile**</span><span class="sxs-lookup"><span data-stu-id="85726-115">**educationSynchronizationProfile**</span></span> | <span data-ttu-id="85726-116">プロファイル識別子を指定した特定のプロファイルを取得します。</span><span class="sxs-lookup"><span data-stu-id="85726-116">Retrieve a specific profile given the profile identifier.</span></span> |
| [<span data-ttu-id="85726-117">同期プロファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="85726-117">Create synchronization profile</span></span>](../api/educationsynchronizationprofile-post.md) | <span data-ttu-id="85726-118">なし</span><span class="sxs-lookup"><span data-stu-id="85726-118">None</span></span> | <span data-ttu-id="85726-119">新しい同期プロファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="85726-119">Create a new synchronization profile.</span></span> |
| [<span data-ttu-id="85726-120">同期プロファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="85726-120">Delete synchronization profile</span></span>](../api/educationsynchronizationprofile-delete.md) | <span data-ttu-id="85726-121">**educationSynchronizationProfile**</span><span class="sxs-lookup"><span data-stu-id="85726-121">**educationSynchronizationProfile**</span></span> | <span data-ttu-id="85726-122">プロファイル識別子を指定した特定のプロファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="85726-122">Delete a specific profile given the profile identifier.</span></span> |
| [<span data-ttu-id="85726-123">進行中の同期を一時停止します。</span><span class="sxs-lookup"><span data-stu-id="85726-123">Pause an ongoing sync</span></span>](../api/educationsynchronizationprofile-pause.md) | <span data-ttu-id="85726-124">なし</span><span class="sxs-lookup"><span data-stu-id="85726-124">None</span></span> | <span data-ttu-id="85726-125">実行中の同期を一時停止します。</span><span class="sxs-lookup"><span data-stu-id="85726-125">Pause an ongoing synchronization.</span></span> |
| [<span data-ttu-id="85726-126">一時停止中の同期を再開します。</span><span class="sxs-lookup"><span data-stu-id="85726-126">Resume a paused sync</span></span>](../api/educationsynchronizationprofile-resume.md) | <span data-ttu-id="85726-127">なし</span><span class="sxs-lookup"><span data-stu-id="85726-127">None</span></span> | <span data-ttu-id="85726-128">一時停止中の同期を再開します。</span><span class="sxs-lookup"><span data-stu-id="85726-128">Resume a paused synchronization.</span></span> |
| [<span data-ttu-id="85726-129">同期をリセットします。</span><span class="sxs-lookup"><span data-stu-id="85726-129">Reset a sync</span></span>](../api/educationsynchronizationprofile-reset.md) | <span data-ttu-id="85726-130">なし</span><span class="sxs-lookup"><span data-stu-id="85726-130">None</span></span> | <span data-ttu-id="85726-131">プロファイルの状態をリセットし、同期を再開します。</span><span class="sxs-lookup"><span data-stu-id="85726-131">Reset the state of the profile and restart synchronization.</span></span> |
| [<span data-ttu-id="85726-132">アップロードされたファイルの同期を開始します。</span><span class="sxs-lookup"><span data-stu-id="85726-132">Start sync for uploaded files</span></span>](../api/educationsynchronizationprofile-start.md) | <span data-ttu-id="85726-133">[educationFileSynchronizationVerificationMessage](educationfilesynchronizationverificationmessage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="85726-133">[educationFileSynchronizationVerificationMessage](educationfilesynchronizationverificationmessage.md) collection</span></span>| <span data-ttu-id="85726-134">アップロードされたソース ファイルを確認し、同期を開始します。</span><span class="sxs-lookup"><span data-stu-id="85726-134">Verify the uploaded source files and start synchronization.</span></span> <span data-ttu-id="85726-135">データ プロバイダーが[educationCsvDataProvider](educationcsvdataprovider.md)が場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="85726-135">Applies only when the data provider is [educationCsvDataProvider](educationcsvdataprovider.md).</span></span> |
| [<span data-ttu-id="85726-136">アップロード先の URL を取得します。</span><span class="sxs-lookup"><span data-stu-id="85726-136">Get an upload URL</span></span>](../api/educationsynchronizationprofile-uploadurl.md) | <span data-ttu-id="85726-137">string</span><span class="sxs-lookup"><span data-stu-id="85726-137">string</span></span> | <span data-ttu-id="85726-138">CSV データ ファイルをアップロードするのには短時間の URL を返します。</span><span class="sxs-lookup"><span data-stu-id="85726-138">Return the short-lived URL to upload CSV data files.</span></span> <span data-ttu-id="85726-139">データ プロバイダーが[educationCsvDataProvider](educationcsvdataprovider.md)が場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="85726-139">Applies only when the data provider is [educationCsvDataProvider](educationcsvdataprovider.md).</span></span> |
| [<span data-ttu-id="85726-140">同期のステータスを取得します。</span><span class="sxs-lookup"><span data-stu-id="85726-140">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | [<span data-ttu-id="85726-141">status</span><span class="sxs-lookup"><span data-stu-id="85726-141">status</span></span>](educationsynchronizationprofilestatus.md) | <span data-ttu-id="85726-142">特定の同期プロファイルの状態を返します。</span><span class="sxs-lookup"><span data-stu-id="85726-142">Return the status of a specific synchronization profile.</span></span> |
| [<span data-ttu-id="85726-143">同期エラーが発生をします。</span><span class="sxs-lookup"><span data-stu-id="85726-143">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="85726-144">[educationSynchronizationError](educationsynchronizationerror.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="85726-144">[educationSynchronizationError](educationsynchronizationerror.md) collection</span></span>| <span data-ttu-id="85726-145">同期処理中に生成されたすべてのエラーを取得します。</span><span class="sxs-lookup"><span data-stu-id="85726-145">Get all the errors generated during synchronization.</span></span> |

## <a name="properties"></a><span data-ttu-id="85726-146">プロパティ</span><span class="sxs-lookup"><span data-stu-id="85726-146">Properties</span></span>

| <span data-ttu-id="85726-147">プロパティ</span><span class="sxs-lookup"><span data-stu-id="85726-147">Property</span></span> | <span data-ttu-id="85726-148">型</span><span class="sxs-lookup"><span data-stu-id="85726-148">Type</span></span> | <span data-ttu-id="85726-149">説明</span><span class="sxs-lookup"><span data-stu-id="85726-149">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="85726-150">**displayName**</span><span class="sxs-lookup"><span data-stu-id="85726-150">**displayName**</span></span> | <span data-ttu-id="85726-151">string</span><span class="sxs-lookup"><span data-stu-id="85726-151">string</span></span> |  <span data-ttu-id="85726-152">アイデンティティの同期の構成プロファイルの名前。</span><span class="sxs-lookup"><span data-stu-id="85726-152">Name of the configuration profile for syncing identities.</span></span>         |
| <span data-ttu-id="85726-153">**データプロバイダー**</span><span class="sxs-lookup"><span data-stu-id="85726-153">**dataProvider**</span></span> | [<span data-ttu-id="85726-154">educationSynchronizationDataProvider</span><span class="sxs-lookup"><span data-stu-id="85726-154">educationSynchronizationDataProvider</span></span>](educationsynchronizationdataprovider.md) |  <span data-ttu-id="85726-155">プロファイルに使用するデータ プロバイダーです。</span><span class="sxs-lookup"><span data-stu-id="85726-155">The data provider used for the profile.</span></span>         |
| <span data-ttu-id="85726-156">**identitySynchronizationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="85726-156">**identitySynchronizationConfiguration**</span></span> | [<span data-ttu-id="85726-157">educationIdentitySynchronizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="85726-157">educationIdentitySynchronizationConfiguration</span></span>](educationidentitysynchronizationconfiguration.md) | <span data-ttu-id="85726-158">アイデンティティの[作成](educationidentitycreationconfiguration.md)時または[一致する](educationidentitymatchingconfiguration.md)構成です。</span><span class="sxs-lookup"><span data-stu-id="85726-158">Identity [creation](educationidentitycreationconfiguration.md) or [matching](educationidentitymatchingconfiguration.md) configuration .</span></span>        |
| <span data-ttu-id="85726-159">**licensesToAssign**</span><span class="sxs-lookup"><span data-stu-id="85726-159">**licensesToAssign**</span></span> | <span data-ttu-id="85726-160">[educationSynchronizationLicenseAssignment](educationsynchronizationlicenseassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="85726-160">[educationSynchronizationLicenseAssignment](educationsynchronizationlicenseassignment.md) collection</span></span>|  <span data-ttu-id="85726-161">セットアップ構成を使用します。</span><span class="sxs-lookup"><span data-stu-id="85726-161">License setup configuration.</span></span>        |
| <span data-ttu-id="85726-162">**state**</span><span class="sxs-lookup"><span data-stu-id="85726-162">**state**</span></span> | <span data-ttu-id="85726-163">educationSynchronizationProfileState</span><span class="sxs-lookup"><span data-stu-id="85726-163">educationSynchronizationProfileState</span></span> |  <span data-ttu-id="85726-164">プロファイルの状態です。</span><span class="sxs-lookup"><span data-stu-id="85726-164">The state of the profile.</span></span> <span data-ttu-id="85726-165">可能な値は、`provisioning`、`provisioned`、`provisioningFailed`、`deleting`、`deletionFailed` です。</span><span class="sxs-lookup"><span data-stu-id="85726-165">Possible values are: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`.</span></span>          |

## <a name="relationships"></a><span data-ttu-id="85726-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="85726-166">Relationships</span></span>

| <span data-ttu-id="85726-167">プロパティ</span><span class="sxs-lookup"><span data-stu-id="85726-167">Property</span></span> | <span data-ttu-id="85726-168">型</span><span class="sxs-lookup"><span data-stu-id="85726-168">Type</span></span> | <span data-ttu-id="85726-169">説明</span><span class="sxs-lookup"><span data-stu-id="85726-169">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="85726-170">**errors**</span><span class="sxs-lookup"><span data-stu-id="85726-170">**errors**</span></span> | <span data-ttu-id="85726-171">[educationSynchronizationError](educationsynchronizationerror.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="85726-171">[educationSynchronizationError](educationsynchronizationerror.md) collection</span></span>| <span data-ttu-id="85726-172">この同期プロファイルに関連付けられているすべてのエラー。</span><span class="sxs-lookup"><span data-stu-id="85726-172">All errors associated with this synchronization profile.</span></span> |
| <span data-ttu-id="85726-173">**profileStatus**</span><span class="sxs-lookup"><span data-stu-id="85726-173">**profileStatus**</span></span> | [<span data-ttu-id="85726-174">educationSynchronizationProfileStatus</span><span class="sxs-lookup"><span data-stu-id="85726-174">educationSynchronizationProfileStatus</span></span>](educationsynchronizationprofilestatus.md) | <span data-ttu-id="85726-175">同期の状態です。</span><span class="sxs-lookup"><span data-stu-id="85726-175">The synchronization status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="85726-176">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="85726-176">JSON representation</span></span>
<span data-ttu-id="85726-177">**EducationSynchronizationProfile**リソースの JSON の形式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="85726-177">The following is a JSON representation of the **educationSynchronizationProfile** resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationProfile"
}-->

```json
{
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationprofile.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
