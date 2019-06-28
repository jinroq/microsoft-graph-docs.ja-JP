---
title: プロビジョニングオブジェクトサマリーリソースの種類
description: Azure AD プロビジョニングサービスとそれに関連付けられているプロパティによって実行される処理を表します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 26c217720692b0d36cfa0acf7537b757c92399ac
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349414"
---
# <a name="provisioningobjectsummary-resource-type"></a><span data-ttu-id="16636-103">プロビジョニングオブジェクトサマリーリソースの種類</span><span class="sxs-lookup"><span data-stu-id="16636-103">provisioningObjectSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16636-104">Azure AD プロビジョニングサービスとそれに関連付けられているプロパティによって実行される処理を表します。</span><span class="sxs-lookup"><span data-stu-id="16636-104">Represents an action performed by the Azure AD Provisioning service and its associated properties.</span></span> 

## <a name="methods"></a><span data-ttu-id="16636-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="16636-105">Methods</span></span>

| <span data-ttu-id="16636-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="16636-106">Method</span></span>       | <span data-ttu-id="16636-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="16636-107">Return Type</span></span> | <span data-ttu-id="16636-108">説明</span><span class="sxs-lookup"><span data-stu-id="16636-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="16636-109">リストのプロビジョニングオブジェクトの概要</span><span class="sxs-lookup"><span data-stu-id="16636-109">List provisioningObjectSummary</span></span>](../api/provisioningobjectsummary-list.md) | [<span data-ttu-id="16636-110">/プロビジョニングオブジェクトの概要</span><span class="sxs-lookup"><span data-stu-id="16636-110">provisioningObjectSummary</span></span>](provisioningobjectsummary.md) | <span data-ttu-id="16636-111">テナントで発生したすべてのプロビジョニングイベントの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="16636-111">Get a list of all provisioning events that occurred in your tenant.</span></span> |


## <a name="properties"></a><span data-ttu-id="16636-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16636-112">Properties</span></span>

| <span data-ttu-id="16636-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16636-113">Property</span></span>     | <span data-ttu-id="16636-114">型</span><span class="sxs-lookup"><span data-stu-id="16636-114">Type</span></span>        | <span data-ttu-id="16636-115">説明</span><span class="sxs-lookup"><span data-stu-id="16636-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="16636-116">action</span><span class="sxs-lookup"><span data-stu-id="16636-116">action</span></span>|<span data-ttu-id="16636-117">String</span><span class="sxs-lookup"><span data-stu-id="16636-117">String</span></span>|<span data-ttu-id="16636-118">アクティビティ名または操作名 (たとえば、Create user、group にメンバーを追加) を示します。</span><span class="sxs-lookup"><span data-stu-id="16636-118">Indicates the activity name or the operation name (for example, Create user, Add member to group).</span></span> <span data-ttu-id="16636-119">ログに記録されたアクティビティの一覧については、「Azure AD activity list」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="16636-119">For a list of activities logged, refer to Azure AD activity list.</span></span>|
|<span data-ttu-id="16636-120">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="16636-120">activityDateTime</span></span>|<span data-ttu-id="16636-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16636-121">DateTimeOffset</span></span>|<span data-ttu-id="16636-p102">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="16636-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="16636-124">changeId</span><span class="sxs-lookup"><span data-stu-id="16636-124">changeId</span></span>|<span data-ttu-id="16636-125">String</span><span class="sxs-lookup"><span data-stu-id="16636-125">String</span></span>|<span data-ttu-id="16636-126">このサイクルでのこの変更の一意の ID です。</span><span class="sxs-lookup"><span data-stu-id="16636-126">Unique ID of this change in this cycle.</span></span>|
|<span data-ttu-id="16636-127">cycleId</span><span class="sxs-lookup"><span data-stu-id="16636-127">cycleId</span></span>|<span data-ttu-id="16636-128">String</span><span class="sxs-lookup"><span data-stu-id="16636-128">String</span></span>|<span data-ttu-id="16636-129">ジョブ反復ごとの一意の ID。</span><span class="sxs-lookup"><span data-stu-id="16636-129">Unique ID per job iteration.</span></span>|
|<span data-ttu-id="16636-130">durationInMilliseconds</span><span class="sxs-lookup"><span data-stu-id="16636-130">durationInMilliseconds</span></span>|<span data-ttu-id="16636-131">Int32</span><span class="sxs-lookup"><span data-stu-id="16636-131">Int32</span></span>|<span data-ttu-id="16636-132">このプロビジョニングアクションが終了するのにかかった時間を示します。</span><span class="sxs-lookup"><span data-stu-id="16636-132">Indicates how long this provisioning action took to finish.</span></span> <span data-ttu-id="16636-133">ミリ秒単位で測定します。</span><span class="sxs-lookup"><span data-stu-id="16636-133">Measured in milliseconds.</span></span>|
|<span data-ttu-id="16636-134">id</span><span class="sxs-lookup"><span data-stu-id="16636-134">id</span></span>|<span data-ttu-id="16636-135">String</span><span class="sxs-lookup"><span data-stu-id="16636-135">String</span></span>| <span data-ttu-id="16636-136">アクティビティの一意の ID を示します。</span><span class="sxs-lookup"><span data-stu-id="16636-136">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="16636-137">これは読み取り専用の GUID です。</span><span class="sxs-lookup"><span data-stu-id="16636-137">This is a read-only GUID.</span></span>|
|<span data-ttu-id="16636-138">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="16636-138">initiatedBy</span></span>|[<span data-ttu-id="16636-139">開始者</span><span class="sxs-lookup"><span data-stu-id="16636-139">initiator</span></span>](initiator.md)|<span data-ttu-id="16636-140">このプロビジョニングを開始したユーザーの詳細。</span><span class="sxs-lookup"><span data-stu-id="16636-140">Details of who initiated this provisioning.</span></span>|
|<span data-ttu-id="16636-141">jobId</span><span class="sxs-lookup"><span data-stu-id="16636-141">jobId</span></span>|<span data-ttu-id="16636-142">String</span><span class="sxs-lookup"><span data-stu-id="16636-142">String</span></span>|<span data-ttu-id="16636-143">プロビジョニングジョブ全体の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="16636-143">The unique ID for the whole provisioning job.</span></span>|
|<span data-ttu-id="16636-144">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="16636-144">modifiedProperties</span></span>|<span data-ttu-id="16636-145">[modifiedProperty](modifiedproperty.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="16636-145">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="16636-146">このプロビジョニングアクションでこのオブジェクトに対して変更された各プロパティの詳細。</span><span class="sxs-lookup"><span data-stu-id="16636-146">Details of each property that was modified in this provisioning action on this object.</span></span>|
|<span data-ttu-id="16636-147">説明手順</span><span class="sxs-lookup"><span data-stu-id="16636-147">provisioningSteps</span></span>|<span data-ttu-id="16636-148">指定[手順](provisioningstep.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="16636-148">[provisioningStep](provisioningstep.md) collection</span></span>|<span data-ttu-id="16636-149">プロビジョニングの各ステップの詳細。</span><span class="sxs-lookup"><span data-stu-id="16636-149">Details of each step in provisioning.</span></span>|
|<span data-ttu-id="16636-150">sourceIdentity</span><span class="sxs-lookup"><span data-stu-id="16636-150">sourceIdentity</span></span>|[<span data-ttu-id="16636-151">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="16636-151">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="16636-152">準備されているソースオブジェクトの詳細。</span><span class="sxs-lookup"><span data-stu-id="16636-152">Details of source object being provisioned.</span></span>|
|<span data-ttu-id="16636-153">sourceSystem</span><span class="sxs-lookup"><span data-stu-id="16636-153">sourceSystem</span></span>|[<span data-ttu-id="16636-154">説明</span><span class="sxs-lookup"><span data-stu-id="16636-154">provisioningSystemDetails</span></span>](provisioningsystemdetails.md)|<span data-ttu-id="16636-155">準備中のオブジェクトのソースシステムの詳細。</span><span class="sxs-lookup"><span data-stu-id="16636-155">Details of source system of the object being provisioned.</span></span>|
|<span data-ttu-id="16636-156">statusInfo</span><span class="sxs-lookup"><span data-stu-id="16636-156">statusInfo</span></span>|[<span data-ttu-id="16636-157">statusBase</span><span class="sxs-lookup"><span data-stu-id="16636-157">statusBase</span></span>](statusbase.md)|<span data-ttu-id="16636-158">プロビジョニング状態の詳細。</span><span class="sxs-lookup"><span data-stu-id="16636-158">Details of provisioning status.</span></span>|
|<span data-ttu-id="16636-159">targetIdentity</span><span class="sxs-lookup"><span data-stu-id="16636-159">targetIdentity</span></span>|[<span data-ttu-id="16636-160">provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="16636-160">provisionedIdentity</span></span>](provisionedidentity.md)|<span data-ttu-id="16636-161">準備されているターゲットオブジェクトの詳細。</span><span class="sxs-lookup"><span data-stu-id="16636-161">Details of target object being provisioned.</span></span>|
|<span data-ttu-id="16636-162">targetSystem</span><span class="sxs-lookup"><span data-stu-id="16636-162">targetSystem</span></span>|[<span data-ttu-id="16636-163">説明</span><span class="sxs-lookup"><span data-stu-id="16636-163">provisioningSystemDetails</span></span>](provisioningsystemdetails.md)|<span data-ttu-id="16636-164">プロビジョニング対象のオブジェクトのターゲットシステムの詳細。</span><span class="sxs-lookup"><span data-stu-id="16636-164">Details of target system of the object being provisioned.</span></span>|
|<span data-ttu-id="16636-165">tenantId</span><span class="sxs-lookup"><span data-stu-id="16636-165">tenantId</span></span>|<span data-ttu-id="16636-166">String</span><span class="sxs-lookup"><span data-stu-id="16636-166">String</span></span>|<span data-ttu-id="16636-167">一意の Azure AD テナント ID。</span><span class="sxs-lookup"><span data-stu-id="16636-167">Unique Azure AD tenant ID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="16636-168">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="16636-168">Relationships</span></span>

<span data-ttu-id="16636-169">なし。</span><span class="sxs-lookup"><span data-stu-id="16636-169">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="16636-170">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="16636-170">JSON representation</span></span>

<span data-ttu-id="16636-171">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="16636-171">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningObjectSummary",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "action": "String",
  "activityDateTime": "String (timestamp)",
  "changeId": "String",
  "cycleId": "String",
  "durationInMilliseconds": 1024,
  "id": "String (identifier)",
  "initiatedBy": {"@odata.type": "microsoft.graph.initiator"},
  "jobId": "String",
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}],
  "provisioningSteps": [{"@odata.type": "microsoft.graph.provisioningStep"}],
  "sourceIdentity": {"@odata.type": "microsoft.graph.provisionedIdentity"},
  "sourceSystem": {"@odata.type": "microsoft.graph.provisioningSystemDetails"},
  "statusInfo": {"@odata.type": "microsoft.graph.statusBase"},
  "targetIdentity": {"@odata.type": "microsoft.graph.provisionedIdentity"},
  "targetSystem": {"@odata.type": "microsoft.graph.provisioningSystemDetails"},
  "tenantId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningObjectSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
